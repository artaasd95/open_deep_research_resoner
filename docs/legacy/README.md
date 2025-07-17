# Legacy Implementation

## Overview

The legacy module contains older implementations of the research agent, including graph-based workflows and multi-agent systems for report generation. These are preserved in `src/legacy` for reference or potential reuse.

Key components:
- `graph.py`: StateGraph for report generation workflow.
- `multi_agent.py`: Multi-agent orchestration.
- `prompts.py`: Legacy prompt templates.
- `state.py`: Legacy state models.
- `utils.py`: Legacy utilities for search and configuration.

## Component Details

- [Graph Workflow](./graph.md)
- [Multi-Agent System](./multi_agent.md)
- [Prompts](./prompts.md)
- [State Management](./state.md)
- [Utilities](./utils.md)

This module uses LangGraph and supports multiple search APIs, but is superseded by the current implementation.