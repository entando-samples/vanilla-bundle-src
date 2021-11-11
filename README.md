# A Vanilla example to deploy a bundle to the Entando Platform 

This is an ent ready project that allows to deploy a bundle to the enatndo platform:
it contains:
1. one MS (you can check the code there: https://github.com/entando-samples/kc-microservice)
2. a single MFE (you can check the code there: https://github.com/entando-samples/react-app-wc-umd)

## To install the bundle to the entando platform 

connect ent to the platform installation then

1. ent prj init

2. ent prj pbs-init

3. ent prj fe-push (--force)

4. ent prj generate-cr | ent kubectl apply -n entando -f - then manually install the bundle using app builder or 
ent prj deploy and ent prj install (--conflict-strategy=OVERRIDE) 


### Notes
swagger ui can be reached at:
MS-INGRESS-URL/swagger-ui.html
