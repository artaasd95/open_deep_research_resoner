# Deep Researcher Logic

## Overview

`deep_researcher.py` defines the core workflows for the deep research agent using LangGraph. It handles user intent clarification, research brief creation, supervision, research execution, result compression, and final report generation.

## Key Functions and Logic

### Clarify User Intent
- `clarify_with_user`: Interacts with the user to refine the research topic if needed.
- Uses `clarify_with_user_instructions` prompt and structured output `ClarifyWithUser`.

### Write Research Brief
- `write_research_brief`: Transforms user messages into a clear research topic.
- Employs `transform_messages_into_research_topic_prompt`.

### Lead Researcher (Supervisor)
- `lead_researcher`: Supervises the research process, deciding on next actions.
- Binds tools like `conduct_research` and uses `lead_researcher_prompt`.

### Researcher
- `researcher`: Performs actual research using tools.
- `researcher_tools`: Handles tool invocations, compressing results if needed.
- Utilizes `research_system_prompt` and compression prompts.

### Final Report Generation
- `final_report_generation`: Synthesizes findings into a report.
- Uses `final_report_generation_prompt`.

## Workflow Connections
- State managed via `SupervisorState` and `ResearcherState`.
- Integrates with utilities for search (e.g., `tavily_search`) and MCP tools.
- Configurable via `Configuration` model for models, iterations, etc.

This file orchestrates the entire research process, connecting prompts, states, and utilities.