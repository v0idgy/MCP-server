# MCP Servers

MCP servers can provides the functionalities like:
- Resources: File-like data that can be read by client (like API responses or file contents)
- Tools: Functions that can be called by the LLM (with user approval)
- Prompts: Pre-written templates that help users accomplish specific tasks

### Requirements 
- Python 3.10 or higher
- uv as package manager
- Python MCP SDK 1.2.0 or higher

### Setting up the Environment

1. Install uv if not available {curl -LsSf https://astral.sh/uv/install.sh | sh}

2. Initialise the project with {uv init .}

3. Add the dependencies {uv add "mcp[cli]" httpx}

4. Create weather.py file which has content for our MCP server 

5. Run the script with the help of uv run or via MCP inspector
- {uv run weather.py}
- {npx @modelcontextprotocol/inspector -- "uv" "run" "weather.py"}