# agentic-notebooks

Create Jupyter notebooks for scientific analysis using generative AI and agentic coding.

## What this repository provides

- A minimal, runnable starter notebook: `notebooks/scientific_analysis_agentic_starter.ipynb`
- A simple agentic pattern for scientific workflows:
  1. Load or generate scientific data
  2. Define analysis tools as Python functions
  3. Let an agent/planner choose tools based on the research question
  4. Return structured results for interpretation and reproducibility

## Quick start

1. Open the notebook in Jupyter Lab or VS Code.
2. Run all cells.
3. Modify:
   - the dataset section for your domain
   - the analysis tools (`summarize_groups`, `mean_difference`)
   - the planner (`mock_planner`) to call your preferred LLM API

## Notes on generative AI integration

The starter uses a mock planner so it runs offline. To use a real model:

- replace `mock_planner` with a model call (OpenAI, Anthropic, local model, etc.)
- keep tool execution deterministic and auditable
- log prompts, tool calls, and outputs for reproducibility
