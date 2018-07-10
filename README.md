# com-stouffcapital-odoo

## docker image
add `unzip` to manually install modules

## kubernetes deployment

1. create secret `kubectl create secret generic odoo --from-literal=postgres-password=<secret>`
1. deploy pvc `odoo-pvc.yaml` (db, web, addons)
1. deploy db `odoo-db.yaml`
1. deploy frontend `odoo-frontend.yaml`
1. deploy ingress rule
