# State Management

## Overview

`state.py` defines Pydantic models and TypedDict classes for structured outputs and state management in the research workflow.

## Structured Output Models

- `ConductResearch`: Triggers research on a subtopic.
- `ResearchComplete`: Marks research completion.
- `Summary`: For summarizing content.
- `ClarifyWithUser`: Handles user clarification requests.
- `ResearchQuestion`: Defines research questions.

## State Classes

- `AgentInputState`: Initial input state.
- `AgentState`: General agent state with messages.
- `SupervisorState`: Manages supervision with research units and findings.
- `ResearcherState`: Tracks researcher progress with task and findings.

## Connections

These states are used in LangGraph workflows in `deep_researcher.py` to maintain context across nodes, integrating with prompts and utilities for seamless execution.