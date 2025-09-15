
# Project 4: Code Writer Agent

Build an agent that can write and refactor code. This project demonstrates prompt engineering and code automation.

## Step 1: Define Features
- Generate code from prompts
- Refactor existing code
- Review code for errors

## Step 2: Write the Code (Pseudocode)
```python
class CodeWriterAgent:
	def __init__(self):
		pass

	def generate_code(self, prompt):
		# Simulate code generation (replace with LLM or API)
		print(f"Generating code for: {prompt}")
		return f"# Code for {prompt}..."

	def refactor_code(self, code):
		# Simulate refactoring
		print("Refactoring code...")
		return code.replace('...', '# Refactored code')

# Example usage
agent = CodeWriterAgent()
code = agent.generate_code("sort a list in Python")
print(code)
refactored = agent.refactor_code(code)
print(refactored)
```

## Step 3: Expand Functionality
- Integrate with real LLMs or code APIs
- Add code review and error detection

## Practical Tips
- Test generated code before using
- Use clear prompts for best results

---
**Next:** YouTube Summary Agent.