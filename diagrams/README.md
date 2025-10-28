All supporting visuals (PNG, JPG, PDF, SVG)


## Recommended naming strategy
diagram-type]_[descriptive-title]-[slug/ID].[filetype]

### Supporting
Descriptive clarity for humans and search indexing
Stable, structured naming for machine parsing or embedding
Optional versioning (-v1) or timestamping (-20250122) for traceability

Examples:
diagram_sdlc-loop-v1.png
diagram_deploy-strategies-v2.pdf
diagram_operating-feedback-loop.png


Avoid:
UUID-like codes or timestamps only (diagram_86123.png) – unreadable, unsearchable
Spaces or camelCase – inconsistent across systems and breaks in some renderers


## Referencing in Markdown
In your .md files, link diagrams using relative paths and clear alt text for accessibility and searchability:
![SDLC Loop Diagram](../diagrams/diagram_sdlc-loop-v1.png)
