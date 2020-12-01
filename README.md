
### **Welcome to the monitoringtools wiki!**

**Grafana, Prometheus, Node exporter**

Install Docker and Docker-Compose
https://docs.docker.com/compose/install/
https://docs.docker.com/get-docker/

mkdir monitoring
cd monitoring

curl -o docker-compose.yaml https://gist.githubusercontent.com/VegasCompany/712d65d41778e5a0a4350d94d02239dc/raw/ad1ccaaf45c22666e4a5c3d4af6c4403dde8e8d1/docker-compose.yaml

mkdir prometheus

curl -o "prometheus/prometheus.yml" https://gist.githubusercontent.com/VegasCompany/90e7419051a1418184579ec9a1ed4838/raw/fedbbd6d0684b51d8146019cb9f60a14e863427f/prometheus.yml

mkdir grafana

curl -o "grafana/datasource.yml"https://gist.githubusercontent.com/VegasCompany/60a4b1f0e476e403d0756c0ddcbb462d/raw/48f35a14223e4799a8b2ed190524d16a57983f40/datasource.yml

docker-compose up -d

curl localhost:9100/metrics

### **Open**

http://localhost:9090
http://localhost:3000

