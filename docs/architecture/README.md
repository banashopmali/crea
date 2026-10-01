# CREA Architecture Documentation

This directory contains the executable architecture documentation for CREA.

## Purpose

The architecture documentation records the system boundaries, major technical decisions, integration contracts, and architecture constraints that must remain aligned with the ratified project governance.

## System Boundaries

CREA is organized around five primary system boundaries:

1. CREA Mobile
2. CREA Platform
3. CREA Money
4. CREA Trust
5. CREA Cloud

## Architecture Principles

- Flutter is the primary mobile client.
- The platform is API-first.
- The initial backend is a Laravel modular monolith.
- CREA Money is isolated as the financial authority.
- Entitlements are separate from payment confirmation.
- Premium media is private by default.
- Direct object-storage upload patterns require explicit authorization and controls.
- Production, staging, and development environments must remain separated.
- Microservices must not be introduced without measured operational justification.

## Authority

Architecture decisions ratified in CREA governance documentation are authoritative.

This repository contains the executable implementation and evidence corresponding to those decisions.

## Change Control

Material architecture changes require:

- documented rationale,
- impact analysis,
- appropriate ADR,
- review according to risk class,
- updated evidence where required.

Architecture must not silently drift from ratified decisions.
