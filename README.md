# Multi-Agent Debugger

![debugging](https://img.shields.io/badge/debugging-blue?style=flat-square) ![visualization](https://img.shields.io/badge/visualization-blue?style=flat-square) ![multi-agent](https://img.shields.io/badge/multi--agent-blue?style=flat-square)

Visualizes the communication flow and state changes between multiple agents in real-time.

## Overview
Multi-Agent Debugger provides a comprehensive observability layer for complex autonomous systems. It tracks message passing and internal state transitions across distributed agents, rendering them into a live visual interface to help developers identify bottlenecks and logic errors in agentic workflows.

## Features
*   **Real-time Topology Mapping:** Automatically generates a live graph of agent interactions and message routes.
*   **State History Tracking:** Inspect the memory and state changes of individual agents at any point in the execution timeline.
*   **Message Payload Inspection:** Drill down into specific prompts, tool calls, and responses exchanged between agents.
*   **Performance Metrics:** Monitor latency and token usage across the entire multi-agent ecosystem.

## Installation
Clone the repository and install the necessary dependencies using pip:

```bash
git clone https://github.com/yourusername/multi-agent-debugger.git
cd multi-agent-debugger
pip install -r requirements.txt
```

## Usage
To start the debugger, run the main entry point. You can integrate it into your existing project by importing the `Debugger` class.

```bash
python main.py
```

**Basic Example:**
```python
from multi_agent_debugger import Debugger

# Initialize the visualizer
db = Debugger()
db.start_session()

# Log agent activity
db.log_interaction(sender="Manager", receiver="Coder", message="Generate a Python script")
```

## Contributing
We welcome contributions to improve the visualization and integration capabilities of this tool. Please submit a Pull Request with a clear description of your changes, ensuring that all new features include corresponding documentation and follow the existing code style.

## License
This project is licensed under the [MIT License](LICENSE).