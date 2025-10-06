---
title: "Care Engineering"
description: "Ambient Scribe"
date: "June 18 2025"
demoURL: "https://www.care.engineering"
repoURL: "https://github.com/anthony-langham"
---

A POC medical ambient voice technology (AVT) system that

- transcribes consultations,
- formats into notes,
- predicts likely diagnoses,
- and suggests the next question to ask.

![Care Engineering](/AmbientScribePlus.png)

## Project Structure

- Frontend: React SPA with Vite build system
- Backend: Express.js server
- APIs: OpenAI realtime & GPT4o
- Deployment: AWS SST framework
- Database: DynamoDB (via SST)
- Authentication: JWT-based with bcrypt password hashing
