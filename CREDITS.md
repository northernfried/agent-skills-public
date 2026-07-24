# Credits

Sources, specifications, and people whose work enriched the skills in this repo, with links back to the specific files that cite them.

## Systems Thinking & Management Theory

### The Systems Thinker
**https://thesystemsthinker.com/systems-thinking-what-why-when-where-and-how/**
Source for the Iceberg Framework (Events → Patterns → Structure → Mental Models) and the "no perfect solutions" framing.
- [`skills/product/systems-thinking-and-domain-driven-design.md`](skills/product/systems-thinking-and-domain-driven-design.md)

### MIT Open Learning
**https://openlearning.mit.edu/news/ask-mit-professor-what-system-thinking-and-why-it-important**
Edward Crawley's systems-as-entities-and-relationships framing ("the cognitive skill of the 21st century").
- [`skills/product/systems-thinking-and-domain-driven-design.md`](skills/product/systems-thinking-and-domain-driven-design.md)

### Wikipedia — Systems Thinking
**https://en.wikipedia.org/wiki/Systems_thinking**
Source for reinforcing/balancing feedback loops, stocks and flows, emergence, causal loop diagrams, and Donella Meadows' leverage-points hierarchy.
- [`skills/product/systems-thinking-and-domain-driven-design.md`](skills/product/systems-thinking-and-domain-driven-design.md)

### Domain Language (Eric Evans)
**https://www.domainlanguage.com/ddd/**
Primary source for Domain-Driven Design's ubiquitous language, strategic design, and context mapping.
- [`skills/product/systems-thinking-and-domain-driven-design.md`](skills/product/systems-thinking-and-domain-driven-design.md)

### Wikipedia — Domain-Driven Design
**https://en.wikipedia.org/wiki/Domain-driven_design**
Source for DDD's three pillars, tactical patterns, and the nine Context Mapping patterns (Partnership, Shared Kernel, Customer/Supplier, Conformist, Anticorruption Layer, Open-Host Service, Published Language, Separate Ways, Big Ball of Mud).
- [`skills/product/systems-thinking-and-domain-driven-design.md`](skills/product/systems-thinking-and-domain-driven-design.md)

### DDD Crew
**https://github.com/ddd-crew**
Source for the practical, fillable DDD templates.
- [`skills/product/systems-thinking-and-domain-driven-design.md`](skills/product/systems-thinking-and-domain-driven-design.md) — [Bounded Context Canvas](https://github.com/ddd-crew/bounded-context-canvas), [Aggregate Design Canvas](https://github.com/ddd-crew/aggregate-design-canvas), [DDD Starter Modelling Process](https://github.com/ddd-crew/ddd-starter-modelling-process)

### The W. Edwards Deming Institute
**https://deming.org/**
Primary source for the entire `Management/` skillset.
- [`skills/Management/system-of-profound-knowledge.md`](skills/Management/system-of-profound-knowledge.md) — [Deming the Man](https://deming.org/deming-the-man/), [SoPK](https://deming.org/explore/sopk/)
- [`skills/Management/fourteen-points-for-management.md`](skills/Management/fourteen-points-for-management.md) — [Fourteen Points](https://deming.org/explore/fourteen-points/)
- [`skills/Management/seven-deadly-diseases.md`](skills/Management/seven-deadly-diseases.md) — [Seven Deadly Diseases](https://deming.org/explore/seven-deadly-diseases/)
- [`skills/Management/pdsa-improvement-cycle.md`](skills/Management/pdsa-improvement-cycle.md) — [PDSA](https://deming.org/explore/pdsa/)
- [`skills/Management/red-bead-experiment.md`](skills/Management/red-bead-experiment.md) — [Red Bead Experiment](https://deming.org/explore/red-bead-experiment/)
- [`skills/Management/funnel-experiment.md`](skills/Management/funnel-experiment.md) — [The Funnel Experiment](https://deming.org/explore/the-funnel-experiment/)

## Specifications & Standards

### OpenAPI Specification
**https://swagger.io/specification/**
Primary source for the OpenAPI/Swagger document-mechanics sub-recipes.
- [`skills/platform/api-builder.md`](skills/platform/api-builder.md)
- [`skills/recipes/api-builder-document-structure-recipe.md`](skills/recipes/api-builder-document-structure-recipe.md) — [`#openapi-object`](https://swagger.io/specification/#openapi-object), [`#info-object`](https://swagger.io/specification/#info-object)
- [`skills/recipes/api-builder-paths-operations-recipe.md`](skills/recipes/api-builder-paths-operations-recipe.md) — [`#paths-object`](https://swagger.io/specification/#paths-object), [`#operation-object`](https://swagger.io/specification/#operation-object)
- [`skills/recipes/api-builder-schemas-recipe.md`](skills/recipes/api-builder-schemas-recipe.md) — [`#components-object`](https://swagger.io/specification/#components-object), [`#schema-object`](https://swagger.io/specification/#schema-object)
- [`skills/recipes/api-builder-security-recipe.md`](skills/recipes/api-builder-security-recipe.md) — [`#security-scheme-object`](https://swagger.io/specification/#security-scheme-object), [`#security-requirement-object`](https://swagger.io/specification/#security-requirement-object)
- [`skills/recipes/api-builder-webhooks-examples-recipe.md`](skills/recipes/api-builder-webhooks-examples-recipe.md) — [`#callback-object`](https://swagger.io/specification/#callback-object), [`#example-object`](https://swagger.io/specification/#example-object)

### Google API Design Guide (AIPs)
**https://docs.cloud.google.com/apis/design** (canonical home: **https://google.aip.dev/**)
Source for resource-oriented design, standard methods, pagination, and error-model guidance.
- [`skills/platform/api-builder.md`](skills/platform/api-builder.md)
- [`skills/recipes/api-builder-google-resource-naming-recipe.md`](skills/recipes/api-builder-google-resource-naming-recipe.md) — [AIP-121](https://google.aip.dev/121) (resource-oriented design), [AIP-122](https://google.aip.dev/122) (resource names), [AIP-190](https://google.aip.dev/190) (naming conventions)
- [`skills/recipes/api-builder-google-standard-methods-recipe.md`](skills/recipes/api-builder-google-standard-methods-recipe.md) — [AIP-130](https://google.aip.dev/130) (standard methods), [AIP-131](https://google.aip.dev/131) (Get), [AIP-132](https://google.aip.dev/132) (List), [AIP-133](https://google.aip.dev/133) (Create), [AIP-134](https://google.aip.dev/134) (Update), [AIP-135](https://google.aip.dev/135) (Delete), [AIP-136](https://google.aip.dev/136) (custom methods), [AIP-193](https://google.aip.dev/193) (errors)

### LeSS (Large-Scale Scrum)
**https://less.works/**
- [`skills/delivery/less-delivery-guidance.md`](skills/delivery/less-delivery-guidance.md) — [framework/introduction](https://less.works/less/framework/introduction), [principles](https://less.works/less/principles/index), [rules](https://less.works/less/rules)

### SAFe (Scaled Agile Framework)
**https://scaledagile.com/** / **https://framework.scaledagile.com/**
- [`skills/delivery/scaled-agile-delivery-guidance.md`](skills/delivery/scaled-agile-delivery-guidance.md) — [Lean-Agile principles](https://framework.scaledagile.com/safe-lean-agile-principles/), [Big Picture](https://framework.scaledagile.com/#big-picture)

### Prioritization Frameworks (WSJF and related)
- [`skills/Refinement/future-workstream-prioritization-wsjf-and-techniques.md`](skills/Refinement/future-workstream-prioritization-wsjf-and-techniques.md) — [SAFe WSJF](https://framework.scaledagile.com/wsjf/), [Fibery: Agile Prioritization Techniques](https://fibery.com/blog/product-management/agile-prioritization-techniques/), [Atlassian: Prioritization Framework](https://www.atlassian.com/agile/product-management/prioritization-framework)

### PCI-DSS v4.0
Publicly published payment-card industry data security standard (PCI Security Standards Council). No specific clause URL is cited in-file; referenced by requirement number.
- [`skills/domains/pci-dss-req-3-4.md`](skills/domains/pci-dss-req-3-4.md) — Requirement 3.4

### SMART Goals
- [`skills/Strategy/annual-goals-and-quarterly-objectives.md`](skills/Strategy/annual-goals-and-quarterly-objectives.md) — [Atlassian: How to write SMART goals](https://www.atlassian.com/blog/productivity/how-to-write-smart-goals), [SNHU: What are SMART goals](https://www.snhu.edu/about-us/newsroom/education/what-are-smart-goals), [UCOP: How to write SMART Goals (PDF)](https://www.ucop.edu/local-human-resources/_files/performance-appraisal/How+to+write+SMART+Goals+v2.pdf), [Harvard Health: Get SMART about your goals](https://www.health.harvard.edu/blog/get-smart-about-your-goals-this-strategy-can-help-you-stay-focused-and-on-track-at-any-age-2017090112113).

### INVEST (User Story / Initiative Quality Checklist)
Originated by Bill Wake (2003); reference definition via the Agile Alliance glossary.
- [`skills/Strategy/annual-goals-and-quarterly-objectives.md`](skills/Strategy/annual-goals-and-quarterly-objectives.md) — [Agile Alliance: INVEST](https://agilealliance.org/glossary/invest/)

## People

### Anthropic / Claude Code Docs
Several platform, delivery, and governance skills are adapted from or attributed to Anthropic's own Claude Code documentation and guidance.
- [`skills/platform/claude-md-configuration.md`](skills/platform/claude-md-configuration.md)
- [`skills/platform/context-management.md`](skills/platform/context-management.md)
- [`skills/platform/session-management-and-failure-patterns.md`](skills/platform/session-management-and-failure-patterns.md)
- [`skills/platform/tooling-and-mcp-servers.md`](skills/platform/tooling-and-mcp-servers.md)
- [`skills/governance/permissions-and-safety.md`](skills/governance/permissions-and-safety.md)
- [`skills/governance/verification-and-self-checking.md`](skills/governance/verification-and-self-checking.md)
- [`skills/delivery/prompting-precision.md`](skills/delivery/prompting-precision.md)
- [`skills/delivery/explore-plan-code-commit.md`](skills/delivery/explore-plan-code-commit.md)

### Kari Hytoenen
Credited as the originating author of the rich-context-input technique.
- [`skills/delivery/rich-context-input.md`](skills/delivery/rich-context-input.md)

## Internal Authorship (non-external, listed for completeness)

Several skills carry a generic internal-team byline rather than a named external source — these were authored in-house rather than adapted from a public source, so there's no external link to credit:

- "Workspace Delivery Skills", "Workspace Strategy Skills", "Workspace Refinement Skills", "Workspace Governance Skills" — internal authoring placeholders across `skills/delivery/`, `skills/Strategy/`, `skills/Refinement/`, `skills/governance/`
- "PM Team" — `skills/product/competitor-analysis-synthesizer.md`, `skills/delivery/jira-epic-builder.md`, `skills/governance/defect-triage-assistant.md`

---

*If you contributed a source, technique, or correction to a skill in this repo and aren't credited here, please open an issue or PR.*
