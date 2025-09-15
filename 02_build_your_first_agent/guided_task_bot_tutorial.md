
# Guided Tutorial: Build a Task Bot

In this tutorial, you’ll build a simple agent that manages tasks for a user. This hands-on project will reinforce your understanding of agentic systems.

## Step 1: Define the Agent’s Features
- Add tasks
- View tasks
- Mark tasks as complete

## Step 2: Write the Code
```python
class TaskBot:
	def __init__(self):
		self.tasks = []

	def add_task(self, task):
		self.tasks.append({'task': task, 'done': False})
		print(f"Added: {task}")

	def show_tasks(self):
		for i, t in enumerate(self.tasks, 1):
			status = '✓' if t['done'] else '✗'
			print(f"{i}. {t['task']} [{status}]")

	def complete_task(self, index):
		if 0 <= index < len(self.tasks):
			self.tasks[index]['done'] = True
			print(f"Completed: {self.tasks[index]['task']}")

# Example usage
bot = TaskBot()
bot.add_task("Finish agentic AI module")
bot.add_task("Review prompt engineering")
bot.show_tasks()
bot.complete_task(0)
bot.show_tasks()
```

## Step 3: Test and Expand
Try adding more features, such as deleting tasks or saving them to a file.

## Practical Tips
- Use clear function names and comments.
- Test each feature as you build.

---
**Next:** Making Agents Smarter.