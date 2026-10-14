# ServerDock Agent Upstream Policy

`serverdock-agent` is a RustDesk-derived project distributed under the AGPL.

## Branches

- `master` tracks the imported RustDesk upstream history and is not used for
  ServerDock product changes.
- `serverdock/customization` starts from the recorded upstream baseline and
  contains focused ServerDock Agent changes.
- The baseline for this branch is
  `fada664df7a294d1d1a9ca3e7cd3637069122f17` with `libs/hbb_common` at
  `229b904508364c8997aad0fb5af57effac859f60`.

## Upstream Synchronization

1. Fetch `upstream` and identify the exact candidate commit.
2. Build and test the candidate on the pinned platform matrix before merging it
   into `master`.
3. Rebase or merge `serverdock/customization` onto the validated `master` and
   resolve conflicts in small, reviewable commits.
4. Record the root and submodule revisions, build inputs and test results for
   every candidate release.
5. Keep modification notices and corresponding-source instructions current.

Never push to `upstream`. Do not flatten, rewrite or remove upstream history.
