# docker-elf

## Containers
* Dummy App

Dummy app generates the sample logs
```
app_1            | {"app": 0.2, "foo": "bar"}
app_1            | {"keydiff": "dummy", "fooss": "bar"}
app_1            |  INFO: {"app": "dummy", "foo": "bar"}
app_1            | Info: Unstructured log
app_1            | {"app": 0.2, "foo": "bar"}
app_1            | {"keydiff": "dummy", "fooss": "bar"}
app_1            |  INFO: {"app": "dummy", "foo": "bar"}
app_1            | Info: Unstructured log
app_1            | {"app": 0.2, "foo": "bar"}
app_1            | {"keydiff": "dummy", "fooss": "bar"}
app_1            |  INFO: {"app": "dummy", "foo": "bar"}
app_1            | Info: Unstructured log
app_1            | {"app": 0.2, "foo": "bar"}
app_1            | {"keydiff": "dummy", "fooss": "bar"}
app_1            |  INFO: {"app": "dummy", "foo": "bar"}
app_1            | Info: Unstructured log
app_1            | {"app": 0.2, "foo": "bar"}
app_1            | {"keydiff": "dummy", "fooss": "bar"}
app_1            |  INFO: {"app": "dummy", "foo": "bar"}
app_1            | Info: Unstructured log
app_1            | {"app": 0.2, "foo": "bar"}
app_1            | {"keydiff": "dummy", "fooss": "bar"}
app_1            |  INFO: {"app": "dummy", "foo": "bar"}
```
* Elasticsearch

This is used for ingestion via filebeat and digestion by Kibana 
* Filebeat

This mounts the /var/lib/docker/containers as readonly to access the logs generated by docker containers. Igest all type of logs structured non-structured
* Kibana

This brings up the kibana dashboard

## Accessing Dashboard
```
$ docker-compose up --build
$ #go to browser open up localhost:5601
```
