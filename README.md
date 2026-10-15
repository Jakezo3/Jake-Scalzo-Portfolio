# Jake Scalzo Portfolio

Interactive personal portfolio website, built as a single-page site for GitHub Pages.

## Folder guide — drop your stuff here

- `assets/images/headshot.png` — your headshot (site already references this exact path)
- `assets/images/vision-board.jpg` — vision board image, used as a subtle background texture in the hero section
- `assets/resume/` — resume PDF (optional, for a "Download Resume" link later)
- `assets/projects/` — any writeups, extra project files, links doc

Once files are in, let me know what's there and I'll wire it into the site.

## Note on source material

The SAP "End of Rotation" deck used to build this site's content is marked
INTERNAL / NDA. Jake has authorized use of the summary metrics already published
on his own resume (banner ad count, video stats, nurture email lifts). No internal
dashboards, org charts, teammate names, or confidential performance data from
the deck are included on the site.

## Campaign Pipeline dashboard

`campaign-dashboard/index.html` is a standalone, interactive dashboard for forward-looking campaigns
(served at `/campaign-dashboard/` on GitHub Pages). It ships with **no campaigns** — add them in the UI.

- **Fields** (modeled on the Upcoming Campaigns exec summary): name, description, LoB, type
  (Campaign / Event-in-a-box / Activation Kit, or custom), New vs. Refresh, segment (Corporate / Enterprise),
  motion (Net New / Install Base), status (Planning / In Progress / Live), estimated launch date or target
  window (Q1–Q4, H1/H2), language versions, owner, free-form tags, notes.
- **Toggles** for every LoB, segment, motion, New/Refresh, type, status and tag; plus search and a launch-date window.
- **KPIs, launch timeline and by-LoB chart** all follow the active toggles.
- **Data**: edits are saved in the viewer's browser (localStorage). Use *Data → Export backup* to save a `.json`.
  To publish a shared starting set for everyone, commit that export as `campaign-dashboard/campaigns.json`
  — first-time visitors load it automatically, and *Data → Reload shared campaigns.json* pulls it in later.
