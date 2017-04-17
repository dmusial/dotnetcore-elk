FROM kibana:5.3.0

RUN apt-get update && apt-get install -y netcat dos2unix

COPY entrypoint.sh /entrypoint.sh
COPY config/kibana.yml /opt/kibana/config/

RUN dos2unix /entrypoint.sh

RUN chmod +x /entrypoint.sh

CMD ["/entrypoint.sh"]
