# Configuration

## Overview

`configuration.py` defines the `Configuration` Pydantic model, which centralizes all configurable parameters for the research agent.

## Key Sections

### General Settings
- `max_structured_output_retries`: Retries for structured output.
- `allow_clarification`: Enables user clarification.
- `max_concurrent_research_units`: Limits concurrent research tasks.

### Research Settings
- `search_api`: Specifies search provider (e.g., tavily, google).
- `max_researcher_iterations`: Maximum iterations per researcher.
- `max_react_tool_calls`: Limits tool calls in ReAct loop.

### Model Configurations
- Models for summarization, research, compression, final report (e.g., `research_model`, `final_report_model`).
- Each with `max_tokens` for output control.

### MCP Settings
- `mcp_server_url`, `mcp_server_api_key` for Model Context Protocol integration.

## Usage

The configuration is passed to agent functions to customize behavior, ensuring flexibility for different research scenarios.

Connects to `deep_researcher.py` for model initialization and workflow control.