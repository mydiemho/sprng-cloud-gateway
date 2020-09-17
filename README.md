# Overview

Spring cloud gate way app to demonstrate how to route traffic to microservices.

App created by following this [guide](https://docs.microsoft.com/en-us/learn/modules/azure-spring-cloud-workshop/5-build-gateway)

## Instruction

```bash
## make sure you're at root of app
./mvnw clean package -DskipTests -Pcloud
az spring-cloud app deploy -n gateway --jar-path target/demo-0.0.1-SNAPSHOT.jar
# stream logs
az spring-cloud app logs -n gateway --lines 100 -f
```
