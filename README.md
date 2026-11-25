# Teacher Hub

One page that links to every classroom and grading tool. Published at
`https://ap-csa-java.github.io/hub/`. Each tool opens in its own tab; nothing is copied or moved.

| Tile | Opens |
|------|-------|
| Roll Call | `ap-csa-java.github.io/roll-call/` |
| Roll Call Teams: Race Day | `ap-csa-java.github.io/roll-call/teams.html` |
| Check for Understanding | the quiz Google Sheet (link saved in your browser) and the course site |
| 40-Question Final (MCQ Exam) | `ap-csa-java.github.io/frq-toolkit/mcq.html` |
| FRQ Writer | `ap-csa-java.github.io/frq-toolkit/` |
| FRQ Grader | `ap-csa-java.github.io/csa-java-grader/` |

To add, remove or rename a tile, edit the `<a class="tile">` blocks in `index.html`
(GitHub web editor is fine). Each tile is one self-contained block.

## Color theme

The gear (⚙️) offers Roll Call's six themes. The choice is saved in the browser key `rc_theme`, which
Roll Call and Race Day also use, so all three match. It works because every tool is served from
`ap-csa-java.github.io`, and pages on the same address share browser storage.
The theme is saved per computer, so student laptops keep their own look.

## Quiz Sheet link

The Sheet link is **not** in this repo (the repo and site are public). Open the gear, paste the link,
Save. It's stored in that browser only, so do this once on each computer you use.

## Keep this repository code-only

No answer keys, rosters or student data here. Anyone can read a public repo.

## If something breaks

- **The hub looks wrong:** it's a single file. Revert `index.html` to an earlier version
  (repo > `index.html` > History > pick a version > copy it back).
- **A tile goes to the wrong place:** fix that tile's `href`.
- **Theme stuck or odd:** in the browser console, `localStorage.removeItem('rc_theme')`, then reload.
  Every tool falls back to Forest Green.

---
ap-csa-java
