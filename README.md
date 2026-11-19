# Google PMS Dashboard (Demo)

Static, no-build Performance Management System dashboard. Toggle **Google (Global) / Google America / Google India**; roles **Admin / Manager / Employee**.
All people and content are **fictional demo data**. No real Google employee or performance data is included.

## Deploy on GitHub Pages
1. Create a new GitHub repo (e.g. `google-pms`).
2. Upload `index.html`, `.nojekyll`, `README.md` to the repo root (or `git push`).
3. Repo -> Settings -> Pages -> Source: "Deploy from a branch" -> Branch: `main`, folder `/ (root)` -> Save.
4. Site goes live at `https://<your-username>.github.io/google-pms/` in about a minute.

## Maintain / update
- Edit in the browser: data saves to that browser's localStorage. Use **Export** to back up JSON and **Import** to restore or share.
- Add/replace employees: edit the `EMP` array in `index.html`. Region logic (KPIs, weights, guidance, rewards) lives in `CT`; role families and KPI templates in `FAM`.
- Roles are a UI demo only (no authentication). For real use, add a backend with SSO and server-side access control (e.g. Google Workspace SSO, Firestore/Cloud SQL) and keep HR data private.
- Never publish real performance data on a public GitHub Pages site.
