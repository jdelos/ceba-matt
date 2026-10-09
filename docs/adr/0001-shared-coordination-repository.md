# ADR-0001: Coordinate two source repositories through one GitHub repository

- Status: accepted
- Date: 2026-02-12

## Decision

Keep `jdelos/vsc-protocol` and `jdelos/ceba-dapp-clean` as independent Git repositories. Use `jdelos/ceba-matt` as shared coordination repository for cross-repo issues, architecture docs, glossary, ADRs, audits, and iteration plans.

## Why

A user-visible DApp capability can require contract, deployment artifact, and UI changes. Independent issue queues lose dependency context. A coordination issue and linked implementation issues preserve ownership while keeping source histories clean.

## Delivery rule

No cross-repo feature starts without compatibility acceptance criteria and explicit blocking edges. Contract changes land with fresh artifacts and DApp validation evidence.
