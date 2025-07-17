# Open Deep Research Module

## Overview

This module contains the core implementation of the deep research agent. It uses LangGraph for state management and orchestrates research through clarification, briefing, supervision, research execution, compression, and final report generation.

Key components:
- `deep_researcher.py`: Main logic for agent workflows.
- `configuration.py`: Pydantic model for configurable parameters.
- `prompts.py`: Prompt templates used in the agent.
- `state.py`: State management models.
- `utils.py`: Utility functions for search and MCP integration.

## Component Details

- [Deep Researcher Logic](./deep_researcher.md)
- [Configuration](./configuration.md)
- [Prompts](./prompts.md)
- [State Management](./state.md)
- [Utilities](./utils.md)

This module connects with search APIs and models to perform iterative research.