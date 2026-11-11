# Contributing

Thanks for helping keep the AAPL expiration tracker up to date.

## Adding weekly data

1. Pull fresh AAPL company snapshot and option chain data from Yahoo Finance.
2. Create one tracking issue per expiration date (in date order): title `Expiry YYYY-MM-DD`.
3. Each issue should include: ATM strike, highest-open-interest call strike, highest-open-interest put strike, and the share price used.
4. On a feature branch, add `expirations.md` at the repo root with the company snapshot, full expiration list, and a per-expiration stats table.
5. Open a pull request from the feature branch into the default branch.
6. Once the PR is open, add a minimal `CONTRIBUTING.md` to the default branch and update the PR branch with the default branch so it picks up that commit.
7. Add a minimal manual (workflow_dispatch) workflow to the default branch, trigger it once, note how long it runs, then delete that run's logs so the repo stays tidy.
8. Check the repository's discussion categories and report what you find.
