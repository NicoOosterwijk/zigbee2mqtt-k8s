# Zigbee2MQTT kustomization K8s

```
apiVersion: fleet.cattle.io/v1alpha1
kind: GitRepo
metadata:
  name: zigbee2mqtt
  namespace: fleet-default
  labels:
    zigbee2mqtt: enabled
spec:
  branch: main
  repo: https://github.com/NicoOosterwijk/zigbee2mqtt-k8s.git
  targets:
    - clusterGroup: zigbee2mqtt
```