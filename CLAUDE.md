# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a **research and specification repository** (not a software project). It contains clinical protocol specifications for an AI agent specializing in **Geriatric Rehabilitation Protocol Validation**.

The primary language is **Portuguese (Brazilian)**.

## Key File

- **AGENTS.md** — Defines the agent persona ("Especialista em Validação de Protocolos de Reabilitação Geriátrica") and its operational guidelines for validating rehabilitation protocols across 20 comorbidities commonly seen in geriatric rehabilitation centers.

## Domain Context

- **Field:** Geriatric Physical Therapy / Evidence-Based Practice (PBE)
- **Goal:** Validate the most efficient "Protocol #1" for each of 20 comorbidities, prioritizing clinical outcomes, patient safety, and reduction of care-related risks
- **Guiding Principle:** "Start low, go slow, but reach the goal"
- **Evidence Standard:** Level A evidence aligned with international guidelines (IASP, AGS, WHO)
- **Protocol Structure:** Three phases — Acute/Protected, Subacute/Strengthening, Advanced/Functional
- **Mandatory Baseline Assessments:** TUG, SPPB, Manual Dynamometry

## Working in This Repository

- There is no build system, test suite, or linting. This is purely a documentation/specification project.
- New content should follow the existing structure in AGENTS.md: clinical rigor, evidence-based, and in Portuguese.
- Protocol outputs must classify interventions by: Therapeutic Modality, Manual Therapy, Kinesiotherapy, and Outcome Indicators.
