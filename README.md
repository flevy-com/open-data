# Flevy Open‑Data Hub 🗂️

**Flevy is the leading marketplace for business best‑practice templates, consulting frameworks, and management toolkits.**  
To foster research and AI experimentation, we publish periodic CSV snapshots of our most‑downloaded resources (e.g. consulting frameworks, PPT templates, financial models, etc.) and trending management topics under an open license.

---

## 📊 Datasets

| File | Rows | What it contains |
|------|------|------------------|
| `top_strategy.csv` | 500 | The 500 highest‑downloaded best practice documents categorized under strateg, transformation, & innovation |
| `top_digital.csv` | 500 | The 500 highest‑downloaded best practice documents categorized under digital transformation |
| `top_opex.csv` | 500 | The 500 highest‑downloaded best practice documents categorized under operational excellence |
| `top_organization.csv` | 500 | The 500 highest‑downloaded best practice documents categorized under organization, change, & HR |
| `top_consulting.csv` | 500 | The 500 highest‑downloaded management consulting frameworks |
| `top_finmod.csv` | 400 | The 400 highest‑downloaded financial models |
| `top_powerpoint.csv` | 50 | The 50 highest‑downloaded PowerPoint template sets |
| `topics.csv` | 500 | Top 500 trending management topics |

### Field glossary
| Column | Description |
|--------|-------------|
| `title` | Full document title |
| `topic` | Primary management topic (e.g. *Strategic Planning*) |
| `url` | Full page URL |
| `category` | Primary functional category (e.g. *Operational Excellence*) |
| `filetype` | `PowerPoint`, `Excel`, `ZIP`, etc. |
| `slide_count` | Number of slides/pages (if applicable) |
| `publishing_consultancy` | Source firm or author |

---

## 🚀 Quick‑start (Python)

```python
import pandas as pd
df = pd.read_csv(
    "https://raw.githubusercontent.com/flevy-com/open-data/main/datasets/top_strategy.csv"
)
print(df.head())
