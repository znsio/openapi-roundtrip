# OpenAPI CodeGen and DocGen Demo

Clean up
```shell
rm -rf app
rm generated.yaml
```

Generate the server code from the OpenAPI Spec using the following command
```shell
openapi-generator generate -i spec.yaml -g spring -o app
```
Start the server using the following command
```shell
cd app
mvn spring-boot:run
```
Download the OpenAPI Spec from the following URL
```shell
curl http://localhost:8080/v3/api-docs.yaml -o generated.yaml
```
