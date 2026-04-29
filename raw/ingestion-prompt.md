# Raw Data Ingestion Prompt

## Goal
Transform raw, unstructured input (notes, clips, thoughts) into a structured format compatible with the Neural-Anchor 3-Layer Architecture.

## Instructions
1. **Analyze Input**: Identify if the content is a fundamental principle (Reading), an active project/idea (Working), or a system-level configuration (System).
2. **Route Content**:
   - **Reading**: Extract CORE THESIS and STRUCTURAL PILLARS.
   - **Working**: Identify RESEARCH QUESTIONS and ACTION ITEMS.
   - **System**: Identify SYSTEM BOUNDARY shifts or CONFIGURATION changes.
3. **Format**: Output as a clean Markdown note with appropriate tags.

## Output Template
- **Source**: {{source}}
- **Layer**: [Reading | Working | System]
- **Core Thesis**: {{one_sentence_summary}}
- **Details**: {{structured_content}}
- **Next Action**: {{next_step}}
