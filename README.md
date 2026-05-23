# `$test` ontology — Homoiconic plugin testing TBox

> **Status:** Phase 0.5 bootstrap (2026-05-23) — root asset only.
> **Scope:** Will grow during Phase 1 of RFC `aaaa2dea-abf3-4601-b800-286111b15ec2` with `test__TestCase`, `test__CommandUnderTest`, `test__ExpectedAssetResult`, `test__ParamBinding`, `test__InheritanceRuleStub` classes + properties + named individuals.

## Purpose

This repo is the **TBox** (terminological box — class + property declarations) for the `test__` namespace used by Exocortex's homoiconic plugin testing strategy. Test cases live as ABox assets in `kitelev/exocortex-ems-commands-test` (sibling repo, created in Phase 2).

## Wiring

Cloned as a git submodule into:
- `vault-2025/assetspaces/test/` *(if pilot becomes generally available)*
- `vault-exodev/assetspaces/test/` *(infrastructure vault — Phase 0.5 Task 0.5.2)*

`$test` ontology URL: `https://exocortex.my/ontology/test#`

## Conventions

- All TBox assets are UUID-named (filename = `<exo__Asset_uid>.md`) per RFC-004 UUID-canon (2026-05-16).
- `exo__Asset_isDefinedBy` of every class/property points to the root `$test` asset (`31cd13c5-e878-4cfa-a741-73a8e7a0bb9b`).

## References

- Parent RFC: [RFC v2: Гомоиконичное тестирование плагинов Exocortex](https://github.com/kitelev/vault-exodev) — vault asset `aaaa2dea-abf3-4601-b800-286111b15ec2`
- Project: vault asset `6f509984-6cb5-4e10-be97-0e15e58b7dd7`
- CLI determinism contract (Phase 0 closure): vault asset `3ee48571-2b07-4ea7-aa54-6a3154625dc0`

## Peer repositories

- `kitelev/exocortex-ems-ontology` — Effort Management System TBox
- `kitelev/exocortex-pmbok-ontology` — PMBOK TBox
- `kitelev/exocortex-aiknow-ontology` — aiKnow memory TBox
- `kitelev/exocortex-exocmd-ontology` — UI plugin command bindings TBox
