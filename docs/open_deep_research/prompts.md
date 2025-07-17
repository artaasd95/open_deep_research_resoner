# Prompts

## Overview

`prompts.py` contains template strings for various stages of the research process. These are used to guide language models in tasks like clarification, supervision, research, compression, and report generation.

## Key Prompts

### Clarification
- `clarify_with_user_instructions`: Guides user interaction for topic refinement.

### Research Topic Transformation
- `transform_messages_into_research_topic_prompt`: Converts messages to a research brief.

### Lead Researcher
- `lead_researcher_prompt`: Instructions for supervising research units.

### Researcher
- `research_system_prompt`: Directs the research assistant in tool usage and reasoning.

### Compression
- `compress_research_system_prompt`: Cleans up research findings.
- `compress_research_simple_human_message`: Simple prompt for compression.

### Final Report
- `final_report_generation_prompt`: Structures the final report.

### Webpage Summarization
- `summarize_webpage_prompt`: Summarizes web content.

## Connections

These prompts are formatted and used in `deep_researcher.py` with models from the configuration, ensuring consistent agent behavior.