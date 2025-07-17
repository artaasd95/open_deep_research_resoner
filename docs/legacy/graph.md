# Graph Workflow (Legacy)

## Overview

`graph.py` defines a LangGraph `StateGraph` for generating reports through planning, feedback, query generation, web search, section writing, and compilation.

## Key Nodes

- `plan_report`: Plans report structure.
- `human_feedback`: Incorporates human input.
- `generate_queries`: Creates search queries.
- `search_web`: Performs web searches.
- `write_section`: Generates section content.
- `write_final_sections`: Evaluates and refines sections.
- `compile_final_report`: Assembles the report.

## Workflow Logic

- Uses conditional edges for iteration based on feedback.
- Manages state with `ReportState`.
- Integrates with models for structured outputs like `Sections` and `Queries`.

## Connections

- Relies on prompts from `prompts.py`.
- Uses utilities for search.
- Part of the legacy report generation pipeline.