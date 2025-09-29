# ITOps-Data-LifeCycle-Management-Agent
An intelligent agent for unified cloud infrastructure management, powered by **LangGraph's ReAct framework**. This agent integrates with **Kubernetes**, **Kubecost**, **Trace Volume Management**, **Visualisation** and **Jaeger** to provide a conversational interface for cluster operations, cost analysis, and trace data management and visualisation.

## Core Capabilities

- **Kubernetes Management:** Execute `kubectl` equivalent commands using natural language.
- **Cloud Cost Monitoring:** Track real-time cloud and in-cluster costs via Kubecost.
- **Jaeger:** Fetch existing services and traces for a given time period.
- **Trace Analysis:** Evaluate and Execute sampling alogorithms for trace data.
- **Automated Workflows:** Proactively identify and suggest optimizations, such as cost-driven trace data reduction.

The agent is deployed at : `{}`

Interaction with the agent can be done via prompts

## Sample Prompts
- Get the observability for the last 24 hours
- Show me all the pods that are currently running in the otel-demo namespace.
- What are all the services currently availible?
- Fetch traces from the 'cart' for the last hour
- Benchmark the available sampling strategies on the trace file `<path>`, setting the rate to 0.45 and the window to 3600 seconds
- I need to inspect the standard output for the 'currency-84c6b8f5d5-5lxmq' pod, which is in the otel-demo namespace.
- Run a cost analysis to get the total and observability costs for the 'otel-demo' namespace specifically.
