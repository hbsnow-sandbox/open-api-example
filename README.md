# open-api-sample

OpenAPI に入門してみた。

## OpenAPI generator

- https://openapi-generator.tech/
- https://openapi-generator.tech/docs/generators.html
- https://github.com/OpenAPITools/openapi-generator

### API clients

```
docker run --rm -v ${PWD}:/local openapitools/openapi-generator-cli generate \
  -i /local/app/swagger.yml \
  -g typescript-fetch \
  -o /local/app/typescript
```

### Server stubs

```
docker run --rm -v ${PWD}:/local openapitools/openapi-generator-cli generate \
  -i /local/app/swagger.yml \
  -g nodejs-express-server \
  -o /local/app/stub
```
