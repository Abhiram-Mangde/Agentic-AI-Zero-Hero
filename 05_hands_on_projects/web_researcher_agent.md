
# Project 2: Web Researcher Agent

Create an agent that researches topics online and summarizes findings. This project demonstrates tool use and information synthesis.

## Step 1: Define Features
- Search the web for information
- Summarize results
- Save summaries

## Step 2: Write the Code (Pseudocode)
```python
import requests

class WebResearcherAgent:
	def __init__(self):
		self.summaries = []

	def search_web(self, query):
		# Simulate web search (replace with real API)
		print(f"Searching for: {query}")
		return f"Results for {query}..."

	def summarize(self, text):
		# Simulate summarization (replace with LLM or API)
		summary = text[:50] + "..."
		self.summaries.append(summary)
		print(f"Summary: {summary}")

# Example usage
agent = WebResearcherAgent()
results = agent.search_web("Agentic AI frameworks")
agent.summarize(results)
```

## Step 3: Expand Functionality
- Integrate with real web search and summarization APIs
- Save summaries to a file

## Practical Tips
- Respect API rate limits and terms of service
- Test with different queries

---
**Next:** GitHub Assistant Agent.