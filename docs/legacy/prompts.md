# Prompts (Legacy)

## Overview

`prompts.py` contains prompt templates for the legacy report generation system, guiding agents in planning, querying, writing, and grading.

## Key Prompts

- `SUPERVISOR_INSTRUCTIONS`: Strict workflow for supervisor (clarify, background, sections, assemble).
- `RESEARCH_INSTRUCTIONS`: Guides researcher through strategic research process.
- `SUMMARIZATION_PROMPT`: For summarizing webpages with structured JSON output.
- Prompts for report planning, query writing, section writing, and grading.

## Connections

These prompts are used in `graph.py` and `multi_agent.py` to instruct models, ensuring structured and high-quality outputs in the legacy workflow.