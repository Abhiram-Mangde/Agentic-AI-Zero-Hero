
# Self-Reflection for Agents

Self-reflection enables agents to evaluate their actions, learn from mistakes, and improve future performance.

## Why Self-Reflection Matters
- **Continuous Improvement:** Agents get better over time by analyzing outcomes.
- **Error Correction:** Identify and fix mistakes.
- **Adaptation:** Change strategies based on feedback.

## Practical Example: Reflective Agent
```python
class ReflectiveAgent:
	def __init__(self):
		self.actions = []
		self.feedback = []

	def act(self, action):
		self.actions.append(action)
		print(f"Action taken: {action}")

	def reflect(self, result):
		self.feedback.append(result)
		print(f"Reflection: {result}")

# Example usage
agent = ReflectiveAgent()
agent.act("Answered user question")
agent.reflect("User was satisfied")
agent.act("Suggested a resource")
agent.reflect("User wanted more details")
```

## Real-Life Scenario
Customer support agents reflect on user feedback to improve service quality.

---
**Next:** Tool Use: Expanding Agent Capabilities.