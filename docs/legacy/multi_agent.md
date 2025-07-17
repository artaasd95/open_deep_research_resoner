# Multi-Agent System (Legacy)

## Overview

`multi_agent.py` implements a multi-agent system for report generation, using supervisor and researcher agents with tool bindings.

## Key Functions

- `supervisor`: Orchestrates the overall workflow.
- `supervisor_tools`: Processes tool calls for questions, sections, introduction, conclusion.
- `research_agent`: Handles research tasks.
- `research_agent_tools`: Manages tool invocations for research.
- State update functions like `supervisor_should_continue`, `research_agent_should_continue`.

## Logic

- Uses Pydantic models for structured outputs (e.g., `Sections`, `Introduction`).
- Builds LangGraph graphs for supervisor and researcher workflows.
- Supports dynamic tool loading, including MCP tools.

## Connections

- Integrates with `prompts.py` for instructions.
- Uses `state.py` for state management.
- Relies on `utils.py` for search and configuration.