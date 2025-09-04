---
title: "ClaudeKit"
description: "A structured workflow system for Claude Code that leverages plan mode, slash commands, and systematic task management to enhance productivity and code quality."
date: "May 18 2025"
repoURL: "https://www.github.com/anthony-langham/claudeKit"
---

## Overview

ClaudeKit provides a sprint-based workflow for managing complex development tasks with Claude Code. It uses:

Plan Mode for thoughtful project planning
Custom Slash Commands for workflow automation
Versioned Plans for tracking iterations
Systematic TODO Management for task execution
Start Planning

Press Shift + Tab twice to enter plan mode
Describe your project requirements
Claude will create a detailed plan
Execute the Workflow

/project:makePlan # Save the plan
/project:makeTODOS # Convert to actionable tasks
/project:nextTODO # Work through tasks one by one
/project:finishPlan # Complete and commit

## Workflow Commands

/project:makePlan
Saves Claude's current plan to a versioned file (plan-v001.md, plan-v002.md, etc.) with timestamps.

/project:makeTODOS
Converts the latest plan into an actionable TODO list with checkboxes for tracking progress.

/project:nextTODO
Finds the first unchecked task
Implements the task
Marks it complete
Repeat until all tasks are done
/project:finishPlan
Reviews all changes
Adds any missing tasks
Creates a comprehensive commit message
Finalizes the sprint

## Best Practices

Always Start with Plan Mode - Think before coding
Break Down Complex Tasks - Use subtasks in your TODOs
Review Before Committing - Use finishPlan to ensure completeness
Version Your Plans - Keep track of iterations
Update CLAUDE.md - Document project-specific conventions

## Advanced Features

### Leveraging Claude Code Capabilities

Subagents: Use specialized agents for complex tasks
TodoWrite Tool: Built-in task management
MultiEdit: Batch file modifications
WebSearch: Research during implementation

### Custom Commands

Create your own slash commands by adding markdown files to .claude/commands/ with:

Command description
Allowed tools
Step-by-step instructions

## Tips

Use plan mode (Shift + Tab twice) for complex features
Run /project:nextTODO repeatedly to work through tasks
Keep CLAUDE.md updated with project-specific instructions
Leverage Claude Code's built-in tools effectively
