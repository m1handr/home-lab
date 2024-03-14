## Environments variables

* `POSTGRES_USER` the default value is **postgres**
* `POSTGRES_PASSWORD` the default value is **changeme**
* `PGADMIN_PORT` the default value is **5050**
* `PGADMIN_DEFAULT_EMAIL` the default value is **pgadmin4@pgadmin.org**
* `PGADMIN_DEFAULT_PASSWORD` the default value is **admin**

## Logging

There are no easy way to configure pgadmin log verbosity and it can be overwhelming at times. It is possible to disable pgadmin logging on the container level.

Add the following to `pgadmin` service in the `compose.yml`:

```
logging:
  driver: "none"
```
