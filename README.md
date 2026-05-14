# Analytics Agent – Model Performance Dashboard

Live dashboard: **https://analytics-agent-coupa.github.io**

## How to update data

1. Edit `data/v44x.csv` or `data/v43x.csv` directly on GitHub (pencil icon).
2. Commit to `main` — the dashboard redeploys automatically within ~1 minute.

## CSV columns

| Column | Description |
|---|---|
| Version | e.g. `v44.x` or `v43.x` |
| Date | `YYYY-MM-DD` |
| Dataset | Dataset name |
| Accuracy | Accuracy % (0–100) |
| Avg_Time_per_Query | Average query time in seconds |
| GPT_Model | Model name e.g. `gpt-4o-mini` |
| Hard_Accuracy | Hard accuracy % (optional) |

## Adding a new version

Create `data/v45x.csv` with the same columns, then add it to `index.html`:

```js
const FILES = ['data/v44x.csv','data/v43x.csv','data/v45x.csv'];
```
