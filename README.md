# Codex Reset scheduler

Calls the authenticated collection endpoint for https://codex.yeartea.xyz every 15 minutes, at minutes 7, 22, 37 and 52 UTC. GitHub may delay scheduled jobs. The website and the owner's computer do not need to be open.

Only scheduling configuration and public health counts are stored here. The collector secret is in GitHub Actions Secrets; announcement data is stored in the site's private Vercel Blob store. No X credentials or cookies are used.

The collector reads Tibo's public X profile and relevant original threads, preserves prior records on failure, and separates scheduled announcements from explicit completion. Ambiguous text requires interpretation and never becomes a confirmed new reset automatically.

A successful health summary is committed once per day or when counts change. This supplies a public operational record and keeps the scheduled workflow active. See Actions for each run's exact result. The schedule can be paused in Actions.
