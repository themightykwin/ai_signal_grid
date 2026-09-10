# SignalGrid

SignalGrid is a lightweight static editorial site tracking the intersection of AI and ecommerce.

## Structure

- `index.html` — frontend, filters, search, brief selector, and styling
- `data/briefs.json` — editorial content source
- `favicon.svg` — site icon

There is no database or build step. The frontend fetches `data/briefs.json` at runtime, which keeps editorial updates simple and makes the site easy to deploy on Vercel or any static host.

## Updating the grid

Add a new brief to `data/briefs.json` with:

- `date`
- `headline`
- `lead`
- `items[]`

Each signal should include `id`, `category`, `title`, `source`, `url`, `summary`, `tags`, `significance`, and `publishedAt`.

Recommended categories:

- `agentic-commerce`
- `ai-merchandising`
- `marketing-automation`
- `ai-foundations`

Recommended significance levels: `high`, `medium`, `low`.

Keep summaries short and useful to an ecommerce operator. The editorial goal is signal over generic AI news: prioritize launches, product changes, protocols, models, and retailer implementations that have a practical implication for commerce teams.
