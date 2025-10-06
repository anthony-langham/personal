---
title: "NoteParser"
description: "An explainable parsing tool for AVT outputs."
date: "June 10 2025"
demoURL: "https://www.noteparser.uk"
repoURL: "https://github.com/anthony-langham/noteparser"
---

An intelligent clinical decision support system that provides structured, auditable clinical recommendations.

![NoteParser](/NoteParser.png)

## Overview

The system ingests clinical notes, which could be typed or generated from an AVT (ambient voice technology). These notes are parsed to provide explainable, repeatable treatment plans with precise medication dosing calculations. This avoids concerns regarding hallucinations associated with LLM systems.

## 🎯 Core Features

- **Clinical Note Parsing:** Extracts structured patient data from unstructured text
- **Condition Identification:** Matches symptoms and assessments to medical conditions
- **Medication Dosing:** Calculates weight-based doses with safety constraints
- **Treatment Planning:** Generates comprehensive, evidence-based treatment plans
- **Audit Trail:** Provides transparent, reproducible clinical reasoning

## 🏥 Supported Conditions

- Paediatric Croup
- Adult Acute Asthma
- Acute Exacerbation of COPD
- Community-Acquired Pneumonia (CAP)
- Paediatric Gastroenteritis

## Why MCP-like over RAG?

- Deterministic Results: Medical decisions require reproducible, auditable outputs
- Structured Validation: Medical data needs strict input/output validation
- Performance: Direct tool calls are faster than semantic search
  Safety: Explicit logic is safer than AI interpretation for medical calculations
- Transparency: Clear reasoning chain for clinical decisions

## Why JSON Files over Database?

- Simplicity: No database setup/configuration for MVP
- Version Control: Clinical data tracked in git with code
- Performance: Fast file reads from Lambda filesystem
- Cost: No database costs for MVP
- Development Speed: Instant data updates without deployment
