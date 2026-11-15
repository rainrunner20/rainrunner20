# LinkedIn project descriptions — evidence-based drafts

These are ready to adapt on LinkedIn after checking the scope of your personal
contribution, especially for collaborative projects. This file is a portfolio
reconciliation log, not an assertion that LinkedIn has already been edited.

## Verified engineering milestones

### IceBrAIker — Networking conversation-starter prototype

Built a Next.js/TypeScript interface and Flask API for creating conversation
starters from profile information. Added input validation, typed browser
responses, a responsive dark-mode UI, and an offline fictional demo. Automated
Python API checks and frontend builds verify the demo path. The older provider
integrations still require separate end-to-end verification.

Repository: https://github.com/rainrunner20/IceBrAIker

### ProcessPilot — CPU scheduling simulator

Built a deterministic FCFS and Round Robin simulator with process-level
turnaround, waiting, response, and CPU utilization metrics. Fixed Round
Robin arrival ordering, added strict input validation and clear API errors,
and introduced regression tests and a reproducible sample workload.

Repository: https://github.com/rainrunner20/Process-Pilot

### TweetInsights — Social topic analytics

Developed a Python batch analytics pipeline for exported social posts.
It validates timestamps and duplicate IDs, compares hashtag activity
across adjacent UTC windows, and exports JSON and a standalone HTML dashboard.
The included sample is synthetic; live X/Twitter ingestion is not implemented.

Repository: https://github.com/rainrunner20/TweetInsights

### Nature's Call — NYC bathroom locator (team project)

Collaborated on a React, Express, and PostgreSQL application for browsing and
reviewing NYC public bathrooms. The source includes account and map features,
and subsequent API maintenance tightened authorization checks on bathroom and
review changes. The live deployment and external APIs need separate verification.

Repository: https://github.com/rainrunner20/Natures-Call

### Sensor forecasting — Research benchmark

Created a reproducible five-minute sensor forecasting benchmark using Pandas,
scikit-learn and Ridge regression. Used a chronological holdout and compared
each model result against a persistence baseline. Added per-sensor MAE,
regression tests, and an HTML report. This predicts sensor readings, not
verified NYC flood events.

Repository: https://github.com/rainrunner20/flood-prediction-nyc-

## LinkedIn project inventory (20 entries)

| Listed project | GitHub repository or verification status |
| --- | --- |
| IceBrAIker | Verified: rainrunner20/IceBrAIker |
| NYC OpenData Reprojector | Code exists: rainrunner20/NYC-DOT-OpenData-Coordinate-Reprojector; needs independent build/deployment test |
| VacAItion | Code exists: rainrunner20/VAIcation; no CI verified in audit |
| AAWCL Banking | Code exists: rainrunner20/AAWCL-Banking; **LinkedIn JavaFX/SQLite description conflicts with Angular/Python repo** |
| AutoDriveAI | No exact repository match verified |
| LibraryMart | No exact repository match verified; do not assume Book-inventory-API is the same project |
| ProcessPilot | Verified: rainrunner20/Process-Pilot |
| CovidCurrent | No exact repository match verified; CovidFlowCast may be related, but this has not been established |
| FlowF1 | No exact repository match verified |
| Taxeez | No exact repository match verified |
| TweetInsights | Verified offline MVP: rainrunner20/TweetInsights |
| Nature's Call | Existing team code: rainrunner20/Natures-Call; staging verification still needed |
| PlAIsticOps | No exact repository match verified |
| DracoVault | No exact repository match verified |
| Cardfia | No exact repository match verified; Mafia-III-Card-App may be related |
| SnapMap | Existing code: rainrunner20/SnapMap; verify current branch/entrypoint |
| DataSnake | No exact repository match verified |
| DiaBeat | Existing model/backend code: rainrunner20/DiaBeat; verification pending |
| Advanced Rocket Dynamics Simulator | No exact repository match verified |
| AeroC++ | No exact repository match verified |

## Rules before publishing claims

- Do not claim a production deployment just because a deploy URL is in a README.
- Do not call offline demos real AI, streaming analytics, or live social-data collection.
- Only mention metrics when there is reproducible benchmark evidence.
- Distinguish original team work from later individual maintenance.
- Keep real commits and PR history; do not backdate or fabricate engineering work.
- Do not include source code that uses another person's private data without permission.

Remaining projects should be individually mapped and tested before their
LinkedIn copy is described as finished.
