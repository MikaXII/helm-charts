# [Peertube](https://github.com/Chocobozzz/PeerTube) on kubernetes

Federated (ActivityPub) video streaming platform using P2P (BitTorrent) directly in the web browser with WebTorrent.

---

## Before deploy

Currently if you want use persistent volume you need to create persistent volume and persistent volume claim

## Installing the chart

`$ helm install --name my-release peertube`

Specify each parameter using the --set key=value[,key=value] argument to helm install. For example,

```
$ helm install --name my-release \
  --set environment.hostname=new.domain.tld,\
  postgresql.postgresPassword=secretpassword \
  peertube
```

Alternatively, a YAML file that specifies the values for the parameters can be provided while installing the chart. For example,

`$ helm install --name my-release -f values.yaml peertube`

## Status : WIP

- [x] Run
- [x] Persist perrtube data (redis and postgresql to)
- [ ] Improve readme for deployment

