# Portfolio production handoff — December 9, 2026

Owner: Daniel Barletta. Prepared November 17, 2026. Target: hiring-team-ready production sites by December 9. Smithsonian application submitted, per Daniel. This document is a release plan, not evidence of deployment or passing checks.

## Outcome
A hiring visitor can understand Daniel's science/software/teaching background in 30 seconds, open a conventional resume, inspect two substantial scientific projects, and experience one complete educational interaction. Existing author and world experiences remain coherent. Private code remains private; no speculative claims about deployments or employment.

## Operating agreement for every VS Code agent
1. Read the repository's AGENTS.md and existing instructions. Inspect pwd, git remote -v, branch, status, recent commits, manifest, lockfile, deployment config and existing PRs before editing. Never print secret values.
2. Do not assume the VS Code folder matches the task. Record actual repository, branch, commit, and target domain. Determine the real production branch; default branch is not proof of deployment branch.
3. Preserve dirty/untracked work. Do not reset, clean, force-push, delete branches, change visibility, archive repositories, or overwrite existing work. Use a separate worktree where appropriate; do not switch another agent's shared checkout.
4. One owner per worktree and task. Run independent tasks concurrently only in isolated worktrees; coordinate shared styles, content and lockfiles. Stop duplicate implementation when an existing PR already addresses the task.
5. Work in small reviewable changes. Resolve reliability, broken journeys and evidence gaps before adding visual effects. Read relevant official framework/security guidance before dependency migrations. Never apply forced dependency fixes blindly.
6. Discover actual scripts before running commands. A missing test/lint script is an explicit gap, not a pass. Capture command, commit, environment, result and evidence. Prior reports are not fresh verification.
7. Production target is authorized, but verify exact host/domain/directory and create a recoverable backup before deployment. If access or destination is ambiguous, prepare code/staging and report the precise missing configuration. Do not guess an FTP path or modify unrelated domains.
8. Never place credentials in reports, repository files, screenshots or command output. Put only variable names in .env.example. Verify browser bundles exclude server credentials and sensitive source data.
9. Keep one RELEASE_STATUS.md in each project: baseline commit; scope; blocker; owner; next action; acceptance evidence; deployed commit/URL/time; rollback. Use confirmed / reported / unverified labels.
10. Every handoff ends with files changed, checks run, checks not run, remaining blockers, deploy state, and one next bounded task. Never call a project done because it builds.

## Verified discovery baseline (November 17)
- DCB: DanielBarletta81/dcbarletta.comv1.1, public, default seo-driven; Next 14.2.5 / React 18.2.0; scripts dev/build/start/lint. Timeline PR #2 is open and unpublished according to PR description. Inspect before duplicating.
- NOAA: DanielBarletta81/noaa-signals-lab, public, default main; open draft PR stack #2, #3, #4, #5. Recorded test results belong to particular commits, not necessarily main or production. PR #5 documents shared unauthenticated SQLite archive, persistent disk requirements, and no backup.
- Microsat: DanielBarletta81/microsat-atlas, public, default master; Next 14.2.5 / React 18.2.0. Manifest has dev/build/start/coast but no test or lint scripts. Synthetic samples; spatial neighbor heuristic is not a population genetics test.
- Tethys: DanielBarletta81/world-of-tethys-2026, private, default main. README describes Next 16 / React 19; inspect real manifest before executing. Earlier public world-of-tethys-next is archived.
- Discovery: two private repositories, tethys-discovery (small inventory) and tethysdiscovery (larger inventory). README.md and package.json requests at the latter root returned 404. This does not prove missing source or a Node app: inspect root tree and local remote. Determine canonical repo rather than renaming or deleting either.
- Profile README currently links private Tethys source. Draft profile PR #1 offers a correction; review live URLs before merging.

## Assignments
### Discovery release owner — first priority
Identify actual repository/root and current local changes. Establish separate document root for tethysdiscovery.com; recent setup reported a shared public_html root, not a verified resolved configuration. Confirm domain mapping, TLS, deployment user landing directory and destination with non-secret evidence. Test using a harmless staging marker before synchronization; never use a deletion sync against an unverified root.
Choose one complete activity as the featured release. Verify start, instructions, interaction, success, reset, keyboard, touch and recovery. Check mobile widths 320/375/768 and desktop, readable text, contrast, focus and reduced motion. Keep scientific claims age-appropriate and defensible. Keep unfinished activities out of normal navigation or label them clearly. Verify children-facing analytics and data collection actually match the published privacy policy; do not introduce accounts or new tracking for this release. Record final repo, branch, commit, deploy path identifier, URL and evidence.

### DCB portfolio owner — hiring front door
Inspect timeline PR #2 and existing author-specialist instructions. Coordinate shared layout with author owner. Preserve book/author paths. Ensure a direct Portfolio path, 30-second overview, conventional resume download, contact, NOAA and Microsat case studies, and public demonstrations for private projects. Do not link hiring visitors to inaccessible private source. Keep a factual claim ledger with source/date/status; reconcile dates before changing credentials. Show independent/unpaid development accurately; BA Biology, incomplete graduate degree. Do not label draft SQL work as deployed. Test English and Indonesian routes, navigation, metadata, redirects, downloads and external project links. Public release should follow domain and deployment verification.

### NOAA reliability owner — strongest technical evidence
Inspect PR #2–#5 and their exact base/head ancestry before edits. Do not blindly merge the stack or reuse old merge SHAs. Determine whether #5 resolves the root manifest blocker and whether the retired LocationData component remains. Reconcile overlapping README claims with final code. First create an integrated release candidate without destroying source branches. Re-run server/client tests, lint, build and relevant security checks at the exact candidate. Add hosted CI for reproducible checks where absent.
Verify missing vs zero, bad timestamps, duplicates, empty data vs upstream no-data ambiguity, timeout, upstream failure, rate limits and successful recovery. Verify snapshot save/reopen/restart, transactional rollback, archive capacity and shared-archive disclosure. Do not introduce accounts merely to expand scope. Public deployment requires persistent writable SQLite disk, backup/restore procedure, permitted origins, proxy settings and bounded resource use. If these cannot be provided, deploy the validated live-observation subset with snapshot UI explicitly unavailable; do not pretend persistence works on ephemeral hosting. Screen-reader verification and browser checks must be explicit, not inferred from axe.

### Microsat scientific interface owner
Read real parser, map and data flow. Add documented input schema and downloadable synthetic sample with provenance. Test malformed CSV/TSV, missing coordinates, out-of-range coordinates, quoted fields, blank assignments, duplicate records and an empty dataset. Preserve raw input versus exclusions and show an actionable explanation. Validate geographic rendering against sourced geometry; do not invent boundaries. Ensure map, site composition and table selection agree. Explain neighbor heuristic, sampling bias and uncertainty without implying genetic inference. Add meaningful parser/interaction checks using the smallest appropriate tooling. Make a working demo and screen-reader-accessible table. Verify data stays local before advertising privacy.

### Tethys platform owner — bounded production scope
Confirm actual production branch and domain separation from DCB and Discovery. Inventory routes and services as verified / optional / mocked / unfinished. Choose atlas or another existing complete journey for hiring demonstration. Remove dead-end calls to action from public paths. Test CMS failures, unavailable media and unauthorized API use. Keep server-only keys out of bundles. Avoid deploying unverified auth, payments, AI spending endpoints or player persistence merely because route files exist. Run actual lint/typecheck/test/world validation/build scripts; inspect failures rather than bypassing checks. Verify real-world science and fictional world content remain distinguishable.

## Calendar and scope control
- Nov 17–20: inventory, protect working changes, resolve Discovery deployment ownership, repair hiring-entry links. Establish release status in every priority repo.
- Nov 21–27: Discovery release; DCB career presentation; NOAA integrated candidate and CI. Start Microsat input validation.
- Nov 28–Dec 3: deploy verified scientific demonstrations, finish two case studies, consolidate Tethys public journey.
- Dec 4–6: cross-site acceptance sweep with a clean browser and mobile checks; verify resume download and contact delivery with controlled testing.
- Dec 7: feature freeze. Only release blockers, factual corrections and broken journeys.
- Dec 8: final production smoke tests, screenshots and rollback rehearsal.
- Dec 9: verify every production URL and document exact deployed versions; ready for hiring-team review.
These are targets, not assumed completed milestones. Omit unfinished optional features rather than publishing a misleading or fragile release.

## Release acceptance checklist
- Correct domain, canonical repo/branch, recorded deploy commit; TLS works.
- Home, portfolio, resume, contact and featured journeys work without an account.
- No placeholder links, fabricated outcomes, inaccessible private-source calls to action or unfinished features represented as shipped.
- Fresh install/build and relevant tests at the deployed commit; repeatable CI where applicable.
- Keyboard, mobile, focus, reduced motion, legible contrast and meaningful text alternatives checked; disclose remaining assistive-technology gaps.
- Loading, empty, error and retry states checked; useful behavior if external services fail.
- Scientific source attribution, units/time zone, missing-data handling and synthetic/observed distinctions are explicit.
- No credentials or sensitive research data exposed; only necessary analytics; privacy statements accurate.
- Data persistence and backups verified where promised; smoke test after deployment; prior release recoverable.
- Actual screenshots and a short walkthrough; case study states problem, Daniel's contribution, design decisions, validation and remaining limits.

## First message to paste into each Claude agent
Read this master handoff and your repo instructions. Inspect the local remote, branch, dirty state, project tree, package scripts and deployment configuration. Do not change files yet. Report the canonical repo/domain, existing work/PRs to preserve, the single highest-risk release blocker, and one small implementation task with acceptance checks. Then implement that reversible task in an isolated branch/worktree, run relevant checks, and update RELEASE_STATUS.md. Work toward the December 9 release; finish primary journeys before optional enhancements. Do not report any test, deployment, accessibility certification or scientific result without evidence. If production access or the target directory is unknown, stop only the deployment step and continue code/staging preparation.
