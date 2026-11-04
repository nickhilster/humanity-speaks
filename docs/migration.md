# Existing website → GitHub source migration

## Known baseline (2026-11-04)

- Existing production URL: https://humanityspeaks.teambotics.app/
- Existing Vercel project: `humanity-speaks` (`prj_eG9zeUOh8nTB90jk5Z7z2fExhEq2`)
- Existing team: `team_OWwjnhbor7MbYnw2kUlbr28r`
- A Vercel deployment file-tree inspection showed a `src/index.html` and individual speaker directories containing `index.html`.
- The current collection has been described as 33 speakers; validate the complete route manifest during source recovery.
- The new GitHub repository is initially documentation-only.

## Migration gates

1. **Recover** the existing Vercel deployment source or its originating local project. Deployment file listings alone do not guarantee recoverable original source.
2. **Inventory** the 33 speaker routes, home page, assets, CSS, scripts, redirects, and metadata. Compare against the live website.
3. **Commit** the recovered code to a migration branch, preserving the current UI and URLs.
4. **Preview** on Vercel without replacing the current production domain.
5. **Test** homepage, every speaker route, mobile behavior, keyboard navigation, outbound links, and indexing metadata.
6. **Connect** the GitHub production branch to the existing Vercel project or perform a controlled migration; do not create a duplicate production domain unintentionally.
7. **Verify** the live domain and rollback path after cutover.

## Content work

Add verified primary-text records incrementally. Separate copyright/public-domain evaluation from source verification and from UI implementation. Existing speaker pages should remain available throughout.

## Explicitly not done

- No source-code recovery completed
- No new transcript publication
- No Git-to-Vercel production connection
- No domain change or production deployment
