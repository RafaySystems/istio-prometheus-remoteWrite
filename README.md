remote_write and remote_read for the prometheus that comes with istio 1.5.6

#helm3 install command helm install install/kubernetes/helm/istio --set global.tag="1.5.6" --set prometheus.enabled=true --set prometheus.global.remote_write.url="<influxdb_domainname>/api/v1/prom/write?db=&rp=shortterm&u=username&p=” --set prometheus.global.remote_read.url="<influxdb_domainname>/api/v1/prom/read?db=&rp=shortterm&u=username&p=” --namespace
