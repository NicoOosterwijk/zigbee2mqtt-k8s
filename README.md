# Zigbee2MQTT kustomization K8s

```
apiVersion: fleet.cattle.io/v1alpha1
kind: GitRepo
metadata:
  name: home-assistant
  namespace: fleet-default
  labels:
    home-assistant: enabled
spec:
  branch: main
  clientSecretName: auth-hp48c
  repo: https://github.com/NicoOosterwijk/zigbee2mqtt.git
  targets:
    - clusterGroup: zigbee2mqtt
```