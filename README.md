# Pretty alertmanager notify Slack massage
**W.I.P**

Synagy to [prometheus-boshrelease](https://github.com/bosh-prometheus/prometheus-boshrelease)

## usage
```
git clone https://github.com/dohq/alertmanager-slack-template-boshrelease

bosh upload-release https://github.com/dohq/alertmanager-slack-template-boshrelease/releases/download/1.0.0/alertmanager-slack-template-1.0.0.tgz

e.g.
bosh -d prometheus deploy manifests/prometheus.yml \
  -o manifests/operators/alertmanager-slack-receiver.yml \
  -o alertmanager-slack-template-boshrelease/operations/prometheus-alertmanager-template.yml \
  --vars-store tmp/deployment-vars.yml
```
