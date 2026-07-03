# Agentic AI Assistant using FLAN-T5 and Tool Calling

## Overview

This project demonstrates a simple **Agentic AI Assistant** built using Google's **FLAN-T5 Large** language model from Hugging Face. The assistant can intelligently decide whether to:

* Perform mathematical calculations
* Retrieve the current system time
* Answer general user queries using a language model

The project showcases the core concept of **AI Agents**, where an LLM acts as a decision-maker and selects appropriate tools to complete a task.

---

## Features

### Tool Selection Agent

The language model analyzes the user's request and chooses one of the following actions:

* **Calculator Tool**

  * Solves basic arithmetic expressions.
  * Supports addition, subtraction, multiplication, and division.

* **Time Tool**

  * Returns the current system time.

* **Chat Tool**

  * Handles general conversations and questions using FLAN-T5.

### Agent Workflow

1. User enters a query.
2. FLAN-T5 acts as a decision-making agent.
3. Agent selects:

   * `TOOL_CALCULATOR`
   * `TOOL_TIME`
   * `ANSWER`
4. Selected tool executes.
5. Final response is returned to the user.

---

## Technologies Used

* Python
* Hugging Face Transformers
* Google FLAN-T5 Large
* Regular Expressions (Regex)
* Datetime Module

---

## Project Structure

```text
agentic-ai-assistant/
│
├── main.py
├── README.md
└── requirements.txt
```

---

## Installation

### Clone the Repository

```bash
git clone <repository-url>
cd agentic-ai-assistant
```

### Install Dependencies

```bash
pip install transformers torch sentencepiece
```

---

## Running the Project

```bash
python main.py
```

Example:

```text
Agentic AI (type 'exit' to quit)

You: 25 + 15
Agent: 40

You: what is the current time
Agent: 14:32:10

You: Explain machine learning
Agent: Machine learning is a branch of artificial intelligence that allows computers to learn from data.
```

---

## Sample Agent Architecture

```text
User Input
     │
     ▼
Decision Agent (FLAN-T5)
     │
 ┌───┼─────────┐
 ▼   ▼         ▼
Calc Time    Chat
Tool Tool    Tool
 │     │       │
 └─────┴───────┘
       │
       ▼
 Final Response
```

---

## Learning Outcomes

Through this project, I gained hands-on experience in:

* Agentic AI fundamentals
* Large Language Models (LLMs)
* Prompt Engineering
* Tool Calling Mechanisms
* Hugging Face Transformers
* AI Decision-Making Workflows
* Building Intelligent Assistants

---

## Future Enhancements

* Add web search capabilities
* Integrate weather APIs
* Support document question answering
* Add memory for multi-turn conversations
* Implement LangChain or LangGraph agents
* Create a Streamlit-based user interface

---

## Internship Information

**Organization:** CSRBOX

This project was developed as part of an internship learning initiative focused on exploring Agentic AI systems, LLM-based decision making, and intelligent tool integration.

---

## Author

**Parchuri Purna Chandra Rao**

* Python Developer
* AI/ML Enthusiast
* Agentic AI Learner

---
