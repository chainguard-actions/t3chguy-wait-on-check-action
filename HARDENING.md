<!-- markdownlint-disable -->

# Hardening Report: t3chguy--wait-on-check-action/18541021811b56544d90e0f073401c2b99e249d6

> This file was generated automatically by the hardening agent.

**Policy SHA:** `d636be7e43ef829af6e853da6b3c7566db9f72fe`

**Test Policy SHA:** `843adf9e4b8f85d0c08b27b9d0b09dd094b54702`

**Harden Agent Version:** `2`

Action **t3chguy--wait-on-check-action/18541021811b56544d90e0f073401c2b99e249d6** was hardened automatically. 1 finding(s) were identified and resolved across 2 iteration(s).

## Findings Fixed

### unpinned-uses (severity: high)

The composite action in action.yml pulls in two other actions by version tag instead of a full 40-character commit SHA: `uses: ruby/setup-ruby@v1` and `uses: actions/cache@v3`. Whoever controls those tags can change the code that runs.

Locations:

- `action.yml:48`
- `action.yml:53`

## Iteration Notes

### Iteration 1

**Fixes applied:** unpinned-uses

**Notes:**

Pinned ruby/setup-ruby@v1 to de492cf36cbab201753d720ce4f4e336cd688c94 and actions/cache@v3 to 6f8efc29b200d32929f49075959781ed54ec270c in action.yml. Each pin keeps its tag in a trailing comment.

### Iteration 2

**Fixes applied:** unpinned-uses

**Notes:**

Pinned actions/cache@v3 to 6f8efc29b200d32929f49075959781ed54ec270c # v3 in action.yml.

