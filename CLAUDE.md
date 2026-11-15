# CLAUDE.md: legal and licensing rules for this repository

This is an **unofficial modified fork** of MetalRender by Pebbles_boon. It is NOT an
Official Release. Follow these rules in every session. They come from the licensing
audit done on 2026-11-15. This is a working summary, not legal advice.

## Provenance (facts)

- Upstream: https://github.com/webblepebbles/metalrender
- Base: upstream commit `b29e12a` (branch `actual_work_here`, 2026-10-21).
- Licence received: "Pebbles-boon Licence" in `LICENSE.md`.
  SHA-256 `7c0cdf06f47e238be720fbcc7531dab487cc2ed58e445ca288dfc531a7799689`.
- Upstream commits before `4690ecc` (2026-09-06) were Apache-2.0 (`c76c44e`).
- Restrictive terms (Discord approval for unmodified redistribution) first appear in
  `4006579` (2026-10-23), AFTER the base. They do not apply to what we received.
- Remotes: `myrepo` = our fork (push here). `origin` = upstream (never push, never merge).

## Never do

1. Never modify `LICENSE.md`, or remove or alter copyright or attribution notices.
2. Never rewrite history (no rebase, amend of pushed commits, force-push, filter-branch).
3. Never merge, cherry-pick, pull or fetch upstream commits after `b29e12a`, and never
   `git pull origin`. Those carry the newer, more restrictive licence.
4. Never copy or closely paraphrase code from newer upstream commits, branches, PRs or
   issue-comment snippets. Fix bugs from the issue description and this tree only.
5. Never contact the upstream developer or post on the upstream repo (issues, PRs,
   comments, Discord).
6. Never add the newer licence text or Discord-approval process to this repo.
7. Never present this project as an Official Release or as endorsed by Pebbles_boon.
8. Never add third-party code or assets without recording their licence in
   `THIRD_PARTY_NOTICES.md`.

## Always do

1. In every file you modify, add a short modification notice in that file's comment
   syntax: `Modified by HoneyShard fork, YYYY-MM-DD: <what>. Not an Official Release.`
   (licence section 2(a)).
2. Add each change to "Changes from the upstream version" in `NOTICE.md`.
3. Keep the unofficial-fork banner in `README.md` and keep `NOTICE.md` accurate.
4. Ship `LICENSE.md` with every distribution, including the jar (`build.gradle`
   already bundles it). Add no further restrictions on recipients.
5. Publish corresponding source with any binary (licence section 2(d)).
6. Use a different product name for binaries (not "MetalRender"). Factual references
   to the original name are allowed (section 3). Rename the mod id and display name
   in `src/main/resources/fabric.mod.json` before the first release.
7. Fix the stale `"license"` field in `fabric.mod.json` when it is next edited.
8. In commit messages for fixes, state "Independent fix; no upstream code copied."

## Termination clause (section 6)

A written notice of violation starts a 30-day cure period from the date it is SENT,
whether or not it is read. If a notice arrives (email, issue, GitHub, DMCA):
stop, record the date and channel, tell the user, and do not reply on their behalf.
Cure any real gap (labelling, branding, missing notices) inside the 30 days.

## Open items

- Verify that `src/main/resources/libmetalrender*.dylib` rebuild from `src/main/resources/native/`.
- Confirm the origin and licence of the PNG assets under `src/main/resources/assets/`.
- Check each dependency's licence and the Gradle wrapper's licence.
- Third-party contributors (`smolgigan`, `MarioMastr`, `Samalando`) own their
  contributions. Do not assume the upstream owner can relicense them.
- UNCERTAIN: upstream's removed `AGENTS.md` claimed AI-assisted processing is not
  licensed. LICENSE.md contains no such restriction, but the risk is unresolved.
  Tell the user if this comes up.

## When unsure

If a task touches licensing, attribution, upstream code, or distribution and these
rules don't clearly cover it, stop and ask the user. Do not guess.
