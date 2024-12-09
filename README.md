# Form specification

An OpenAPI specification to describe forms. This spec has been created with HTTP requests in mind, but can be applied to other contexts.

# "Why did you create this?"

I prefer for forms in my web projects to originate from the server, acting as a source of truth. As requirements change, the web forms update dynamically. Libraries already exist for this, but I wasn't happy with the options out there. I created this spec to describe the form structure I tend to use in my own projects - and as a nice OpenAPI specification exercise.

# The specification file(s)

Depending on your preferences, you can use the single-file or multi-file spec. The single-file spec is located in the **bundles** directory. The multi-file spec is located in the **openapi** directory.

# Redocly

This specification was built and linted using [Redocly CLI](https://redocly.com/docs/cli). Using this tool is not strictly required to view or bundle the specification.

## Known issues

[Redocly's OpenAPI VS Code extension](https://redocly.com/docs/redocly-openapi) correctly displays the `description` property for each `Field` schema. However, the CLI `preview-docs` command does not. Similar issues have already been reported:

* <https://github.com/Redocly/redocly-cli/issues/1329>
* <https://github.com/Redocly/redoc/issues/1458>

# Version notes

## 1.0.0

* Initial specification publication

# Future plans

* Add more fields and field attributes, based on my needs in other projects
* Add a schema to describe available CRUD operations
* Add properties for choice fields which call endpoints to search for values
* Add a schema which describes form structure changes based on the values of certain fields
