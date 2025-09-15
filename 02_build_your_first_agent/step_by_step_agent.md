
# Step-by-Step: Creating a Simple Agent

Building your first agent is a hands-on way to understand how agentic systems work. Follow these steps to create a basic task bot in Python.

## Step 1: Define the Agent’s Purpose
Decide what your agent should do. Example: Manage a to-do list.

## Step 2: Set Up the Environment
Install Python and your favorite code editor (VS Code recommended).

## Step 3: Write the Agent Code
```python
class TaskAgent:
	def __init__(self):
		self.tasks = []

	def add_task(self, task):
		self.tasks.append(task)
		print(f"Added task: {task}")

	def show_tasks(self):
		print("Your tasks:")
		for i, task in enumerate(self.tasks, 1):
			print(f"{i}. {task}")

# Example usage
agent = TaskAgent()
agent.add_task("Finish AI homework")
agent.add_task("Read agentic systems article")
agent.show_tasks()
```

## Step 4: Test and Improve
Run your agent, add more features (like removing tasks or saving to a file), and experiment!

## Practical Advice
- Start simple, then iterate and add complexity.
- Use print statements to debug and understand agent behavior.

---
**Next:** Introduction to Prompt Engineering.