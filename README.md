# Nussknacker secondary env example
The purpose of this repository is to quickly present the needed configuration and behaviour of the remote environment feature

## Start Nussknacker designers from docker compose
```bash
docker compose up -d
```

## Addresses
* [Designer env1](http://localhost:8080) - credentials admin/admin
* [Designer env2](http://localhost:8081) - credentials admin/admin

## Notes
* The provided docker compose starts NU designers:
    * in request-response mode - in this mode NU deploys scenarios as REST endpoints
    * with embedded hsql db - each Designer instance owns its own hsql instance

## Secondary env configuration
* required configuration is provided under `secondaryEnvironment` object in `application.conf` and parametrized using env variables per docker container
* the meaning of individual parameters is described in the [Nussknacker documentation](https://nussknacker.io/documentation/docs/installation_configuration_guide/DesignerConfiguration/#environment-configuration)
