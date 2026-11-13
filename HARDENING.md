<!-- markdownlint-disable -->

# Hardening Report: t3chguy--wait-on-check-action/18541021811b56544d90e0f073401c2b99e249d6

> This file was generated automatically by the hardening agent.

**Policy SHA:** `d636be7e43ef829af6e853da6b3c7566db9f72fe`

**Test Policy SHA:** `843adf9e4b8f85d0c08b27b9d0b09dd094b54702`

**Harden Agent Version:** `2`

Action **t3chguy--wait-on-check-action/18541021811b56544d90e0f073401c2b99e249d6** was hardened automatically. 1 finding(s) were identified and resolved across 1 iteration(s).

## Findings Fixed

### unpinned-uses (severity: high)

action.yml has composite-step uses: refs pinned to mutable tags instead of 40-character commit SHAs: 'uses: ruby/setup-ruby@v1' and 'uses: actions/cache@v3'.

Locations:

- `action.yml:49`
- `action.yml:54`

## Iteration Notes

### Iteration 1

**Fixes applied:** unpinned-uses

**Notes:**

Pinned ruby/setup-ruby@v1 -> b3aaceaef7e0ee231b499e7b5f49c03fc1d32199 and actions/cache@v3 -> 6f8efc29b200d32929f49075959781ed54ec270c in action.yml, keeping tag comments.

