---
title: "Care Engineering"
description: "Ambient Scribe and Decision Support SaMD."
date: "June 18 2025"
demoURL: "https://www.care.engineering"
repoURL: "https://github.com/anthony-langham"
---

Live transcription tool that predicts likely diagnoses and prompts the next 3 most relevant follow up questions to narrow further.

![Care Engineering](/AmbientScribePlus.png)

A React-based medical assistant application that uses OpenAI's realtime API for voice interactions and provides clinical note extraction, diagnostic suggestions, and structured medical documentation.

## Project Structure

Frontend: React SPA with Vite build system
Backend: Express.js server with OpenAI realtime API integration
Deployment: AWS SST framework
Database: DynamoDB (via SST)
Authentication: JWT-based with bcrypt password hashing
