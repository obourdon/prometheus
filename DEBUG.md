gvm use go1.14
GOOS=linux GOARCH=amd64 make build && GOOS=linux GOARCH=amd64 make common-docker && docker tag prom/prometheus-linux-amd64:tag-v2.28.1 obourdon/prometheus:v2.28.1 && docker push obourdon/prometheus:v2.28.1
