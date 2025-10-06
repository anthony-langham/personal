---
title: "Care GraphRAG"
description: "POC: A knowledge graph database by scraping NICE Guidelines, enabling LLM enhanced explainable node/edge-based queries with traceable paths"
date: "Mar 26 2025"
---

An explainable, low-cost LLM/GraphRAG system for UK NICE Clinical Knowledge Summary (CKS) on Hypertension.

![GraphRAG](/GraphRAG.png)

## 🎯 Current Capabilities

**Enhanced Data Pipeline:**
NICE Guidelines → Advanced Medical Knowledge Graph → Hybrid Retrieval → QA Chain

**Clinical Question Answering:**
GPT-4o-mini powered QA with medical safety prompting

**Hybrid Retrieval:**
Graph-first approach with intelligent vector search fallback

**Source Attribution:**
Complete provenance tracking with confidence scoring

**Performance Monitoring:**
Track retrieval latency, costs, and usage patterns

**Cost Tracking:**
Token-based estimation for OpenAI API usage

**Interactive Graph Visualization:**
Neo4j-style network explorer with color-coded entities and relationships

**Clinical Decision Trees:**
Age-based, ethnicity-based, and conditional treatment pathways

**Graph Storage:**
Persistent medical knowledge graphs in MongoDB

**Management Scripts:**
Comprehensive suite for graph building, data management, and analysis
