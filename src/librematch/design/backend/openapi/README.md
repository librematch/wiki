# OpenAPI

## Documentation Generation

FastAPI will take care of generating the documentation page. [We can choose from different UIs](https://fastapi.tiangolo.com/features/#automatic-docs):

1. ** [ReDoc](https://github.com/Rebilly/ReDoc) **\
   with a [CLI](https://github.com/Redocly/redocly-cli) that lints our OpenAPI spec
1. ** [SwaggerUI](https://github.com/swagger-api/swagger-ui) **

**ReDoc** has premium services and we need to check if although it looks more beautiful it's worth to opt in to their free stage or if **SwaggerUI** is enough.

## API first principle

We follow the API first principle. Meaning that we define our API first, before generating the backend stub and coding its implementation.

Our OpenAPI spec acts like a **single source of truth (SSOT)**. Test cases are generated from the OpenAPI spec and the backend implementation needs to adhere to them.

Our design follows a few different design guidelines:

1. [Zalando RESTful API Guidelines](https://opensource.zalando.com/restful-api-guidelines/)
1. [Microsoft API Design Best Practices](https://docs.microsoft.com/en-us/azure/architecture/best-practices/api-design)
1. [Web API Checklist by Mathieu Fenniak](https://mathieu.fenniak.net/the-api-checklist/)

## Deviations from Guidelines

1. We don't use **kebab case** and **snake case** instead as the dash can easily introduce bugs as it can be interpreted as a minus sign.
1. We might want to use [CalVer](https://calver.org/) ([Read github notes](https://docs.github.com/en/rest/overview/api-versions?apiVersion=2022-11-28))

## Assigning Scopes

https://opensource.zalando.com/restful-api-guidelines/#105
