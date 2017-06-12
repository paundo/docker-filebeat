# docker-filebeat
I use filebeat for monitoring server.log file from Payara or Glassfish

Into filebeat.yml change IP address and port where your logstash ip and port or graylog ip and port.

chmod +x docker-entrypoint.sh

docker build -t filebeat-paundo:v01 .

docker run -d --name filebeat-paun -v DataVolume:/mnt/ filebeat-paundo:v01
