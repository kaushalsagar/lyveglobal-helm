# Dependency 


dependencies:
- name: levy-mongodb
  version: "1.2.3"
  repository: "file://charts/levy-mongodb"

#Command to view the complete yaml
#helm template levy-nodejs -f levy-nodesj/values.yaml ./levy-nodejs/


#Command to install the chart.

#helm install node-mongo-chart levy-nodejs/ -f levy-nodejs/values.yaml -n default
