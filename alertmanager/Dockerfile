FROM prom/alertmanager

VOLUME [ "/etc/alertmanager", "alertmanager-data:/data" ]

COPY alertmanager.yml /etc/alertmanager/config

EXPOSE 9093

