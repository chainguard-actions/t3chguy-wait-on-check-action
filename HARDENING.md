<!-- markdownlint-disable -->

# Hardening Report: t3chguy--wait-on-check-action/18541021811b56544d90e0f073401c2b99e249d6

> This file was generated automatically by the hardening agent.

**Policy SHA:** `d636be7e43ef829af6e853da6b3c7566db9f72fe`

**Test Policy SHA:** `843adf9e4b8f85d0c08b27b9d0b09dd094b54702`

**Harden Agent Version:** `2`

Action **t3chguy--wait-on-check-action/18541021811b56544d90e0f073401c2b99e249d6** was hardened automatically. 1 finding(s) were identified and resolved across 1 iteration(s).

## Findings Fixed

### unpinned-uses (severity: high)

action.yml has composite steps that reference actions by a mutable tag instead of a full 40-character commit SHA: 'uses: ruby/setup-ruby@v1' and 'uses: actions/cache@v3'. Pin both to commit SHAs.

Locations:

- `action.yml:49`
- `action.yml:54`

## Iteration Notes

### Iteration 1

**Fixes applied:** unpinned-uses

**Notes:**

Pinned ruby/setup-ruby@v1 to f9c4492e86def3e644ab32a0ef185eda5b0c20d0 and actions/cache@v3 to 6f8efc29b200d32929f49075959781ed54ec270c in action.yml, with tag comments.

