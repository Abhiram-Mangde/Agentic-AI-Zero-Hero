
# Memory in Agents

Memory is a key feature that allows agents to learn from experience, store important information, and adapt to new situations.

## Why Memory Matters
- **Learning:** Agents use memory to improve decisions over time.
- **Context:** Memory helps agents remember user preferences, past actions, and outcomes.
- **Adaptation:** Agents can change behavior based on what they’ve learned.

## Types of Memory
- **Short-term:** Temporary storage for immediate tasks.
- **Long-term:** Persistent storage for knowledge and experiences.

## Practical Example: Task Agent with Memory
```python
class MemoryAgent:
	def __init__(self):
		self.memory = []

	def remember(self, info):
		self.memory.append(info)
		print(f"Remembered: {info}")

	def recall(self):
		print("Memory:")
		for item in self.memory:
			print(f"- {item}")

# Example usage
agent = MemoryAgent()
agent.remember("User likes Python")
agent.remember("Completed task: Build agent")
agent.recall()
```

## Real-Life Scenario
Smart assistants remember your favorite music, recent searches, and appointments to provide personalized service.

---
**Next:** Planning & Reasoning Strategies.