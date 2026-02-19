# Baseflow Documentation

This repository contains the official documentation for [Baseflow](https://usebaseflow.com), the documentation platform for product teams.

## Structure

```
baseflow-docs/
├── docs.json                  # Site configuration, navigation, and theming
├── logo/                      # Logo files (light/dark SVG)
├── images/                    # Images referenced in docs
├── index.mdx                  # Landing page
├── quickstart.mdx             # 5-minute getting started guide
├── key-concepts.mdx           # Core concepts overview
├── writing-content/           # Guides on authoring docs
├── components/                # MDX component reference
├── project-structure/         # Config and navigation setup
├── customization/             # Branding, themes, domains, SEO
├── workflows/                 # Git, visual editor, review, collaboration
└── advanced/                  # API docs, versioning, analytics, AI
```

## Local Preview

1. Push this repo to GitHub
2. Connect it to a Baseflow project in the [dashboard](https://app.usebaseflow.com)
3. Every push to `main` automatically deploys to your docs site

For local development, the Baseflow docs renderer runs at `localhost:4201`.

## Writing Docs

- All pages are `.mdx` files (Markdown + JSX components)
- Navigation is defined in `docs.json`
- Assets go in `images/` and `logo/` — they're automatically synced to the CDN
- Use frontmatter (`title`, `description`) at the top of each page

## Adding a New Page

1. Create a `.mdx` file in the appropriate directory
2. Add the path to `docs.json` under the right navigation group
3. Commit and push — the page appears automatically

## Available Components

Baseflow supports these MDX components out of the box:

| Component                                             | Usage                                      |
| ----------------------------------------------------- | ------------------------------------------ |
| `<Card>`                                              | Linked cards with title, description, icon |
| `<CardGroup>`                                         | Grid layout for cards                      |
| `<Tabs>` / `<Tab>`                                    | Tabbed content                             |
| `<CodeGroup>`                                         | Tabbed code blocks by language             |
| `<Accordion>`                                         | Collapsible sections                       |
| `<AccordionGroup>`                                    | Grouped accordions                         |
| `<Steps>` / `<Step>`                                  | Numbered step-by-step guides               |
| `<Callout>`                                           | Info, warning, success, error callouts     |
| `<Note>`, `<Warning>`, `<Tip>`, `<Check>`, `<Danger>` | Callout aliases                            |
| `<Frame>`                                             | Image frames with captions                 |
| `<Tooltip>`                                           | Hover tooltips                             |
| `<Badge>`                                             | Inline badges                              |
| `<Icon>`                                              | Lucide icons                               |
| `<ParamField>`                                        | API parameter documentation                |
| `<ResponseField>`                                     | API response documentation                 |
| `<Expandable>`                                        | Collapsible property details               |

## License

Copyright © 2026 Baseflow. All rights reserved.
