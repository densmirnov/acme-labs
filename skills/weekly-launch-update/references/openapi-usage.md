# OpenAPI Usage in Skill Packages

OpenAPI files are optional. Include an OpenAPI specification only when the skill needs to call, document, or reason about an external API.

## Include OpenAPI when

- launch data comes from a project-management API;
- risks come from an incident tracker;
- customer signals come from CRM or support systems;
- decisions are pulled from an internal status service;
- the agent needs a schema for structured API calls.

## Do not include OpenAPI when

- the skill only uses uploaded documents;
- the skill only uses local files;
- the skill receives context manually from the user;
- API access is not part of the workflow.

## In this package

`../openapi/acme-launch-data.openapi.yaml` is an optional example. It is included to show where an OpenAPI schema belongs when the skill is connected to structured launch data. The core skill works without it.
