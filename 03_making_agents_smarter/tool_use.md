
# Tool Use: Expanding Agent Capabilities

Agents become truly powerful when they can use external tools to solve problems beyond their built-in capabilities. Tool use allows agents to access information, perform calculations, interact with APIs, and automate tasks in the real world.

## Why is Tool Use Important?
- **Extends agent abilities:** Agents can answer questions, fetch data, and perform actions they otherwise couldn’t.
- **Enables real-world impact:** From booking appointments to analyzing data, tool use bridges the gap between AI and practical utility.

## Real-World Examples
- **Web search:** Agents use search engines to find up-to-date information.
- **Calculator:** Agents solve math problems using external calculators.
- **APIs:** Agents interact with weather, finance, or productivity APIs to provide useful services.

## How Agents Use Tools: Step-by-Step
1. **Detect need for a tool:** The agent identifies when a task requires external help.
2. **Select the right tool:** The agent chooses the appropriate tool (e.g., web search, calculator).
3. **Invoke the tool:** The agent sends a query or command to the tool.
4. **Process the result:** The agent uses the tool’s output to complete the task.

### Example: Agent Using a Calculator Tool (Python Pseudocode)
```python
def agent_ask_math_question(question):
	if 'calculate' in question:
		# Use calculator tool
		result = calculator_tool(question)
		return f"The answer is {result}"
	else:
		return "I can only help with calculations."

def calculator_tool(query):
	# Simulate external tool use
	# In practice, this could call an API or use a library
	return eval(query.replace('calculate', '').strip())

# Example usage
print(agent_ask_math_question('calculate 2 + 2'))
```

## Practical Exercise
**Build an agent that uses a weather API to answer: 'What’s the weather in London today?'**

1. Research a free weather API (e.g., OpenWeatherMap).
2. Write code for the agent to call the API and return the result.
3. Test your agent with different cities.

---
Tool use is a key skill for building advanced, practical agents. Experiment with different tools and APIs to expand your agent’s capabilities!