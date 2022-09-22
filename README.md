# Hello World - CAP deployed by Github Actions

# Check application running:
https://e51034c8trial-dev-helloworld-srv.cfapps.us10-001.hana.ondemand.com/say/hello(to='yourNAme')


## Tips:

Add in you mta.yaml file:

```
build-parameters:
  before-all:
   - builder: custom
     commands:
      - npm install --production
      - npx -p @sap/cds-dk cds build --production
      - npx rimraf gen/db/src/gen/data
```

## Learn More

Learn more at 
- https://cap.cloud.sap/docs/get-started/.
- https://developers.sap.com/tutorials/btp-app-cap-mta-deployment.html
- https://cap.cloud.sap/docs/guides/deployment/to-cf#cf-cli
- https://developers.sap.com/tutorials
- https://github.com/Guerric-P/cf-cli-action
- https://github.com/citizen-of-planet-earth/cf-cli-action

