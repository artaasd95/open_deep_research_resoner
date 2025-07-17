# State Management (Legacy)

## Overview

`state.py` defines Pydantic models and TypedDict classes for the legacy report generation process.

## Structured Models

- `Section`, `Sections`: For report sections.
- `SearchQuery`, `Queries`: For search queries.
- `Feedback`: For evaluation feedback.

## State Classes

- `ReportStateInput`, `ReportStateOutput`, `ReportState`: Manage overall report state.
- `SectionState`, `SectionOutputState`: Handle individual section states.

## Connections

Used in `graph.py` and `multi_agent.py` for state persistence and workflow routing in the legacy system.