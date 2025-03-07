# AI Agent Observability and Evaluation

## What is Observability?

Observability is about understanding what's happening inside your AI agent by looking at external signals like logs, metrics, and traces. For AI agents, this means tracking actions, tool usage, model calls, and responses to debug and improve agent performance.

## Traces and Spans

- **Traces** represent a complete agent task from start to finish (like handling a user query).
- **Spans** are individual steps within the trace (like calling a language model or retrieving data).
- Using traces and spans helps identify bottlenecks, errors, and inefficiencies clearly.

![Example of a smolagent trace in Langfuse](https://langfuse.com/images/cookbook/huggingface-agent-course/trace-tree.png)

## Why Agent Observability Matters

Without observability, AI agents are "black boxes." Observability tools make agents transparent, enabling you to:

- Debug effectively
- Optimize performance
- Understand costs and accuracy trade-offs
- Continuously improve agent capabilities

## Observability Tools

Common observability tools for AI agents include platforms like Langfuse and Arize. These tools help collect detailed traces and offer dashboards to monitor critical metrics in real-time, making it easy to detect problems and optimize performance.

## Key Metrics to Monitor

- **Latency:** Response speed of the agent.
- **Costs:** Expense per agent interaction, including model and API usage.
- **Accuracy:** Quality and correctness of agent outputs.
- **User Feedback:** Direct user ratings and comments.
- **Implicit Feedback:** User behaviors like rephrased queries or session abandonment.
- **Automated Metrics:** LLM-as-a-Judge, recall, or custom evaluation scores.

Monitoring these metrics helps you quickly spot issues and decide where to focus improvement efforts.

## Evaluating AI Agents

Regular evaluation ensures your AI agent remains effective over time. There are two main methods:

### Online Evaluation

- Continuous monitoring of agent performance in production.
- Relies on user interactions, explicit ratings, implicit behaviors, and live monitoring.
- Helps identify user problems, user dissatisfaction, and model drift quickly.

### Offline Evaluation

- Uses controlled tests and datasets with known answers.
- Enables repeatable, systematic checking of agent accuracy and behavior.
- Allows safe experimentation and catching regressions before deploying to users.

Effective evaluation typically combines both methods—continuously monitoring live performance and running regular offline tests.

## Lets see how this works in practice

[Click here to open the notebook](notebooks/bonus-unit2/monitoring-agents.ipynb)


