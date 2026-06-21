# Better Food Agent

### Agentic-AI-Team-8
USD MS-AAI 510 Agentic AI Systems Final Project


Architecture:

Two Datasets: FDA food additives (health risk scores) + restaurant nutrition data (MenuStat 2022).

Six SQL Tools: Get additive info, analyze meals, compare meals, find nutritious options, find healthier alternatives, batch analyze ingredients.

One MCP Tool: You.com web search for ingredient lists using Python. Not registered to Unity Catalog due to it needing live MCP connection.

Agent: better_food_agent using databricks-gpt-oss-120b (with 20b for comparison).

Pipeline:

Setup: Install dependencies, download datasets, create Unity Catalog tables.

Tools: Create and test 6 SQL functions that query nutrition/additive data.

Agent: Define agent code in better_food_agent.py, configure LLM, add MCP connection for web search.

Testing: Run sample queries, create traces for observation.

Evaluation: Build eval dataset, create custom judge (better_food_judge), run evaluation, collect human feedback.

Optimization: Use SIMBA to align judge with human feedback, compare original vs. aligned judge performance.
