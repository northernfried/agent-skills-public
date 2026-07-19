# Recipes

Use this category for reusable procedure-style guidance with strong implementation instructions and control requirements.

Initial planned migrations:

- `payment-processing-recipe.md`

API Builder sub-recipes (used by `../platform/api-builder.md`):

Based on the [OpenAPI Specification](https://swagger.io/specification/) (document mechanics):

- `api-builder-document-structure-recipe.md` — root object, info, servers, tags
- `api-builder-paths-operations-recipe.md` — paths, operations, parameters, request bodies, responses
- `api-builder-schemas-recipe.md` — components/schemas, composition, discriminators
- `api-builder-security-recipe.md` — security schemes and requirements
- `api-builder-webhooks-examples-recipe.md` — callbacks, webhooks, examples, links

Based on [Google's API design guide](https://docs.cloud.google.com/apis/design) (resource-oriented design):

- `api-builder-google-resource-naming-recipe.md` — resource-oriented design, resource/collection naming, resource name format
- `api-builder-google-standard-methods-recipe.md` — Get/List/Create/Update/Delete HTTP mapping, pagination, error model
