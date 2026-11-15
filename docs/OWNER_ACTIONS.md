# Owner action checklist — what GitHub access cannot do

This checklist identifies items the repository maintainer must authorize or
configure in their own provider accounts. Never paste tokens, passwords,
private keys or credentials into chat, commit messages or README files.

## Immediate: rotate exposed credentials

### Newly identified: Vision Zero Insights credentials

- [ ] URGENT: Rotate the publicly exposed PostgreSQL DATABASE_URL password and verify the old account cannot connect.
- [ ] Replace all formerly committed ADMIN_TOKEN values, invalidate old access, and keep admin tokens out of frontend bundles.
- [ ] Restrict or reissue the hardcoded Mapbox token if it is still valid.
- [ ] Review database and hosting access logs, forks, clones and repository snapshots; current-file deletion does not erase history.


- [ ] **Book-inventory-API:** rotate the PostgreSQL password that existed in
  a previously committed .env file. Audit database connections and reduce privileges.
- [ ] **AAWCL Banking:** rotate Azure SQL credentials and the JWT signing
  secret that were previously hardcoded. Invalidate old signed sessions/tokens.
- [ ] **Process-Pilot:** revoke or restrict any Google/provider API key that
  was committed historically, even though the tracked file was removed.
- [ ] Review provider audit logs, Git history and public forks/clones. Deleting
  a file from the current branch cannot revoke a secret or remove every copy.

## Vercel deployment permission

- [ ] Approve the Vercel team-level authorization request for the existing
  project, scope bobbyleiscool-3272.
- [ ] Inspect the failed IceBrAIker deployment and verify its Next.js root
  directory is my-nextjs-app after reading the actual build logs.
- [ ] Verify production/preview URL and sample interactions; keep provider
  research mode visibly unavailable until backend sources are tested.
- [ ] Approve any billing, custom domain or DNS changes separately.

## Firebase and Google services

- [ ] Connect an owned Firebase project for VAIcation (not the old public
  tutorial project) and set up Firestore security rules with genuine user
  authentication and per-user ownership.
- [ ] Add only Firebase **public client configuration** to the appropriate
  Vite environment; keep server secrets entirely server-side.
- [ ] Restrict Google Places browser API keys by HTTP referrer and allowed
  API. Configure authorized Google OAuth origins and redirect URLs.
- [ ] Move Gemini generation to a server-side authenticated endpoint with
  quotas/rate limits before using a production key. VITE_* keys are visible
  in browser bundles and must never hold valuable private API secrets.

## Integrations that require separate evidence

- [ ] Confirm which of the remaining LinkedIn project entries match real
  repositories, archived files or code running on another account.
- [ ] Verify authorship/credit for team projects and select representative
  projects for a concise resume.
- [ ] Update the actual LinkedIn profile using verified text. The currently
  available LinkedIn lookup tool does not edit profile entries.
- [ ] Supply any missing project sources through an authorized repository or
  project attachment if code cannot be recovered from GitHub.

## Deployment acceptance rules

Passing unit tests does not prove a production deployment is running.
Do not call a tool production-ready unless the actual hosted URL works,
critical flows and access controls have been tested, and secrets are secure.
Do not claim measured performance improvements without reproducible data.

## Local portfolio demos and deployment

- [ ] 3D Portfolio: check the default test1 branch and 3D asset licenses. For Vercel, use root my-portfolio and production branch test1, then verify the live URL before advertising it.
- [ ] Cyber Defense Lab: generate a new local JWT_SECRET_KEY and use SQLite or disposable local Docker Postgres; do not expose demo servers publicly.
