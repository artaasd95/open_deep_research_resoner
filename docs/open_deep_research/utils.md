# Utilities

## Overview

`utils.py` provides utility functions for search operations and Model Context Protocol (MCP) integration.

## Search Utilities

### Tavily Search
- `tavily_search`: Asynchronous search using Tavily API.
- `summarize_webpage`: Summarizes webpage content using a configured model.

## MCP Utilities

### Token Management
- Functions for token counting and management.

### Authentication
- Utilities for MCP authentication.

### Tool Loading
- `load_mcp_tools`: Loads tools from MCP server.

## Connections

These utilities are used in `deep_researcher.py` for:
- Retrieving information from the web.
- Integrating with external models via MCP.
- Managing token usage for efficient operation.

They connect with the `Configuration` model for API keys and settings.