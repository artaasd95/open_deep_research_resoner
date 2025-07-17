# Utilities (Legacy)

## Overview

`utils.py` provides legacy utility functions for configuration handling, search operations, and result processing.

## Key Functions

- `get_config_value`, `get_search_params`: Handle configuration values.
- `deduplicate_and_format_sources`: Processes and formats search results.
- `format_sections`: Formats report sections.
- Asynchronous search functions: `tavily_search_async`, `azureaisearch_search_async`, `perplexity_search`, `exa_search`, `arxiv_search_async`, `pubmed_search_async`, `linkup_search`, `google_search_async`.
- Additional utilities like `scrape_pages`, `select_and_execute_search`, `summarize_webpage`, `split_and_rerank_search_results`, `stitch_documents_by_url`, `get_today_str`, `load_mcp_server_config`.

## Connections

These utilities support search integrations in `graph.py` and `multi_agent.py`, handling multiple APIs and result formatting for the legacy workflow.