
# Project 1: Smart To-Do Agent

Build an agent that manages tasks intelligently. This project will help you apply agentic concepts in a practical way.

## Step 1: Define Features
- Add, view, complete, and delete tasks
- Save tasks to a file
- Prioritize tasks

## Step 2: Write the Code
```python
class SmartTodoAgent:
	def __init__(self):
		self.tasks = []

	def add_task(self, task, priority=1):
		self.tasks.append({'task': task, 'done': False, 'priority': priority})
		print(f"Added: {task} (Priority: {priority})")

	def show_tasks(self):
		sorted_tasks = sorted(self.tasks, key=lambda x: x['priority'])
		for i, t in enumerate(sorted_tasks, 1):
			status = '✓' if t['done'] else '✗'
			print(f"{i}. {t['task']} [{status}] (Priority: {t['priority']})")

	def complete_task(self, index):
		if 0 <= index < len(self.tasks):
			self.tasks[index]['done'] = True
			print(f"Completed: {self.tasks[index]['task']}")

	def delete_task(self, index):
		if 0 <= index < len(self.tasks):
			removed = self.tasks.pop(index)
			print(f"Deleted: {removed['task']}")

# Example usage
agent = SmartTodoAgent()
agent.add_task("Finish agentic AI module", priority=2)
agent.add_task("Review prompt engineering", priority=1)
agent.show_tasks()
agent.complete_task(0)
agent.delete_task(1)
agent.show_tasks()
```

## Step 3: Expand Functionality
- Save/load tasks to/from a file
- Add deadlines and reminders

## Practical Tips
- Test each feature as you build
- Use comments to explain your code

---
**Next:** Web Researcher Agent.