FROM kibana:5.3.0

RUN apt-get update && apt-get install -y netcat

COPY entrypoint.sh /entrypoint.sh
COPY config/kibana.yml /opt/kibana/config/

RUN chmod +x /entrypoint.sh

CMD ["/entrypoint.sh"]
