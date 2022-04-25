Run Command -> helm create lyve-nodejsapp
Run Command -> helm create lyve-mongodb

Edit deployments,service,ingress in each chart


Run Command -> cd lyve-nodejsapp
add below line in Chart.yaml
dependencies:
- name: lyve-mongodb
  version: "1.0.0"
  repository: "file://../lyve-mongodb"
  

Run Command -> helm dependency build
Run Command -> helm dependency list

Run Command -> helm install nodejsapp-mongo .

