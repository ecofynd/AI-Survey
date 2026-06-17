# AI Effectiveness Survey

A self-hosted team survey for measuring AI maturity — with a live admin dashboard.

## 🚀 Deploy in 3 steps (GitHub Pages — free)

1. **Fork or upload** this repository to your GitHub account
2. Go to **Settings → Pages → Source → Deploy from branch → `main` → `/ (root)`**
3. Your survey is live at: `https://YOUR-USERNAME.github.io/REPO-NAME/`

## 📋 What's inside

- **Team survey** — 26 scored questions across 5 sections (Usage, Prompt Management, Quality, Efficiency, Advanced)
- **Instant score report** — each respondent sees their AI maturity score + band + 30-day action plan immediately after submitting
- **Admin dashboard** — charts, KPIs, per-person drill-down, CSV export

## 🔐 Accessing the dashboard

The dashboard is protected by a password. Default: **`admin123`**

To change it, open `index.html` and find this line near the top of the `<script>` section:

```js
const ADMIN_PASSWORD = 'admin123';
```

Replace `admin123` with your own password and save.

## 📊 Dashboard features

| Feature | Details |
|---|---|
| KPI cards | Total responses, average score, power users, beginners needing training |
| Score distribution | Bar chart of how scores are spread |
| Maturity bands | Doughnut chart (Beginner → Expert) |
| Section radar | Team average % per section |
| Department breakdown | Horizontal bar by team |
| Response table | Searchable, with per-person score bars and band pills |
| Detail view | Click any row to see section scores, best prompt submitted, and action plan |
| CSV export | Download all responses for further analysis |

## 📁 How data is stored

Survey responses are saved in the **browser's localStorage** of whoever takes the survey — on the same device/browser as the dashboard viewer.

> This means the survey works with **zero backend** — no server, no database, no cost.
> **Limitation:** responses taken on other devices won't appear in your dashboard automatically.

### For team-wide collection (recommended workflow):
1. Share the `index.html` URL with your team
2. Ask each team member to take the survey
3. For the dashboard, use the CSV export from each machine — or host on a shared device / internal server

## 🎨 Customise

- **Company name:** Search `AI Effectiveness Survey` in `index.html` and replace
- **Password:** See above
- **Sections/questions:** Edit the `SECTIONS` array in the `<script>` block
- **Admin-only Manager Evaluation questions:** Can be added as a separate section

## 📄 License

Free to use and modify for internal team purposes.
