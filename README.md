# Supermodel OpenAPI Specification

[![npm](https://img.shields.io/npm/v/@supermodeltools/openapi-spec)](https://www.npmjs.com/package/@supermodeltools/openapi-spec)
[![OpenAPI](https://img.shields.io/badge/OpenAPI-3.0-green)](https://spec.openapis.org/oas/v3.0.0)

OpenAPI 3.0 specification for the [Supermodel API](https://docs.supermodeltools.com) - code graphing and static analysis.

## Install

```bash
npm install @supermodeltools/openapi-spec
```

The spec is available at `node_modules/@supermodeltools/openapi-spec/openapi.yaml`.

## Endpoints

| Method | Path | Description |
|--------|------|-------------|
| POST | `/v1/graphs/dependency` | File-level dependency graph |
| POST | `/v1/graphs/call` | Function-level call graph |
| POST | `/v1/graphs/domain` | Domain model classification |
| POST | `/v1/graphs/parse` | AST parse tree relationships |
| POST | `/v1/graphs/supermodel` | Full Supermodel IR bundle |

All endpoints accept a zipped repository snapshot and return graph data as JSON.

## Authentication

Requests require an API key via `X-Api-Key` header. Get your key from the [Supermodel Dashboard](https://dashboard.supermodeltools.com).

## Links

- [API Documentation](https://docs.supermodeltools.com)
- [API Terms of Service](https://supermodeltools.com/legal/api-terms)
