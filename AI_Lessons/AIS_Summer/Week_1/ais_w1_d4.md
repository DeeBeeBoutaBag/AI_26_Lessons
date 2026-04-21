<img src="https://github.com/Hgp-GeniusLabs/Curriculum/blob/10734f2c827128dde773ea4f266d154d46977866/Org-Wide/Assets/hgp_logo_original.png" width="150"/>

Lesson Plan: AI Systems Week 1, Day 4 --- Rule-Based Systems vs AI Systems and First OpenAI API Lab
=================================================================================================

**Duration:**
-------------

3 hours

**Lesson Overview:**
--------------------

On Day 4, Geniuses reach an important turning point in AI Systems: they begin using the **OpenAI API** for the first time. The lesson is designed to make that moment meaningful, not magical. Instead of treating the API like a shortcut, Geniuses compare two different ways a system can work: a **rule-based system** and an **AI-powered system**. This helps them understand that modern AI tools are powerful, but they are still part of a larger system with inputs, outputs, structure, and tradeoffs.

The lesson focuses on text classification and structured output. Geniuses first build a simple rule-based classifier, then create an OpenAI-powered classifier and compare the strengths and weaknesses of both. They begin to see where fixed rules work well, where AI helps more, and why developers must still think about trust, accuracy, and system design. During independent practice, each Genius builds a first OpenAI-powered AI Systems mini-tool connected to their own use case. By the end of the lesson, Geniuses should understand that using an API does not replace systems thinking. It adds a powerful model into the system.

**Objectives:**
---------------

-   Explain the difference between a rule-based system and an AI-powered system.
-   Identify situations where fixed rules work well and where model-based reasoning works better.
-   Use the OpenAI API in Python for the first time.
-   Build a simple OpenAI-powered classifier with structured output.
-   Compare rule-based classification and AI-powered classification.
-   Reflect on the strengths, weaknesses, and risks of API-powered AI systems.
-   Continue the Week 1 mini-project by creating a first OpenAI-powered AI Systems prototype.

**Materials:**
--------------

-   Laptops for all Geniuses
-   VS Code installed
-   Python installed and working
-   OpenAI API key for each Genius or team
-   Internet access
-   Projector or display
-   Whiteboard and markers
-   Slide deck for lecture and discussion
-   Reflection journal or digital notes
-   Terminal access in VS Code
-   Starter folder for Python files
-   `.env` setup instructions or environment variable instructions

**Standards:**
--------------

-   Computational Thinking: Compare different system approaches for solving the same problem.
-   Computer Science Practices: Build and test both rule-based and model-based workflows.
-   Programming: Use Python and the OpenAI API to create a structured AI-powered system.
-   Digital Literacy: Evaluate the strengths and limits of modern AI APIs in real systems.
-   Career Readiness: Practice experimentation, comparison, debugging, and technical reasoning.
-   Technical Foundations: Understand that AI APIs are components inside larger systems, not complete solutions by themselves.

**Lesson Activity:**
--------------------

### 1. **Introduction (Time: 25 minutes)**

-   **Objective:** Energize Geniuses and introduce the idea that not every intelligent system needs a model, but some tasks become much easier when a model is involved.
-   Start with a fun icebreaker called **"Rules or AI?"**
-   This should be the first thing and the most fun thing to wake Geniuses up and get them ready for the lesson.

#### **Icebreaker Option A: Physical Movement**

-   Label one side of the room **"Rules"** and the other side **"AI."**
-   Read system tasks aloud and have Geniuses move to the side they think fits best.
-   Example prompts:
    -   Check whether a password is long enough
    -   Detect whether an email is probably spam
    -   Decide whether a sentence sounds angry or calm
    -   Sort uploaded files by exact file type
    -   Classify a user message as scheduling, homework, or personal support
    -   Count how many times the word "free" appears in a message
    -   Understand whether a paragraph sounds encouraging or negative
    -   Generate a more flexible summary from messy notes
-   After each round, ask:
    -   Why would rules work here?
    -   Why would AI work better here?
    -   Could both approaches work?
    -   Which one feels more flexible? Which one feels more predictable?

#### **Icebreaker Option B: Quick System Sort**

-   Put tasks on the board and ask small groups to sort them into:
    -   best handled by rules
    -   best handled by AI
    -   could use both
-   Use the results to introduce the day's comparison between deterministic logic and model-powered behavior.

#### **Transition**

-   Say:
    -   "Today Geniuses begin using the OpenAI API, but not as magic. We are using it as one system component and comparing it against simpler system logic."
-   Ask:
    -   When should a builder choose rules?
    -   When should a builder choose AI?
    -   What could happen if we use AI for something that does not actually need it?

### 2. **Direct Instruction (Time: 50 minutes)**

-   **Objective:** Help Geniuses understand the role of model APIs inside AI systems and why comparison matters.
-   Use slides to guide instruction and keep it interactive.

#### **Suggested Slide Flow**

-   **Slide 1: Today's Focus --- First OpenAI API Lab**
    -   Today Geniuses compare rule-based systems and AI-powered systems
    -   The goal is not just to call an API, but to understand when and why to use one
-   **Slide 2: What Is a Rule-Based System?**
    -   A system that follows explicit human-written logic
    -   Example:
        -   if a message contains "free" and "click now," label it spam
    -   Strong when:
        -   rules are simple
        -   categories are clear
        -   behavior must be predictable
-   **Slide 3: What Is an AI-Powered System?**
    -   A system that uses a trained model to interpret patterns and produce outputs
    -   Strong when:
        -   language is messy
        -   inputs vary
        -   reasoning is more flexible
        -   rigid rules would miss too much
-   **Slide 4: Rules vs AI**
    -   Rules:
        -   consistent
        -   fast
        -   transparent
        -   limited flexibility
    -   AI:
        -   flexible
        -   handles messy data
        -   can generalize
        -   less predictable
        -   may need extra trust checks
-   **Slide 5: What Is the OpenAI API?**
    -   A way for software to send input to a model and receive output
    -   It allows developers to build AI-powered behavior into their own systems
    -   It is not the whole app. It is one part of the app
-   **Slide 6: API Inputs and Outputs**
    -   Input:
        -   prompt
        -   instructions
        -   user content
    -   Output:
        -   text
        -   structured categories
        -   JSON
        -   reasoning-style summaries
    -   Developers still define:
        -   workflow
        -   rules
        -   UI
        -   trust features
        -   evaluation
-   **Slide 7: Why Structured Output Matters**
    -   AI output becomes much easier to use if it is organized
    -   Example:
        -   category
        -   confidence
        -   explanation
    -   This makes the system easier to connect to real apps
-   **Slide 8: First API Use Case --- Classification**
    -   This fits well because Geniuses already understand categories, inputs, and risks
    -   It also makes comparison with rules easy
-   **Slide 9: Responsible Use of API-Based Systems**
    -   do not assume the model is always right
    -   add review or caution for uncertain cases
    -   compare model output with real need
    -   think about cost, reliability, and trust
-   **Slide 10: This Week's Direction**
    -   Geniuses are now moving from understanding AI systems conceptually into building modern AI-powered system components

#### **Discussion Questions**

-   What are the biggest strengths of rule-based systems?
-   What are the biggest strengths of AI-powered systems?
-   Why might a builder choose both instead of only one?
-   Why is structured output useful in technical systems?
-   What responsibilities come with adding a model to a product?

#### **Reflection Prompt**

-   Have Geniuses write for 4 minutes:
    -   "Describe one task where simple rules are enough and one task where an AI model would help more. Why?"

### 3\. **Guided Practice (Time: 60 minutes)**

-   **Objective:** Help Geniuses build both a rule-based classifier and an OpenAI-powered classifier in Python.
-   Explain that today's code-along is about comparison and systems thinking.
-   The class will create `rule_vs_ai_classifier.py`.

#### **Guided Practice Build**

Create a folder called `rule-vs-ai-classifier`.

#### **Project Goal**

Build a Python program that:

-   takes a user message
-   classifies it first with simple rules
-   classifies it again with the OpenAI API
-   compares the results

#### **Setup Steps**

1.  Open VS Code.
2.  Create a folder called `rule-vs-ai-classifier`.
3.  Open the terminal in VS Code.
4.  Install dependencies:
```
pip install openai python-dotenv
```
1.  Create a `.env` file:
```
OPENAI_API_KEY=your_key_here
```
1.  Create a file called `rule_vs_ai_classifier.py`

#### **Sample Code**
```
# rule_vs_ai_classifier.py
# AI Systems Week 1 Day 4
# This program compares a rule-based classifier
# with an OpenAI-powered classifier.

import os
from dotenv import load_dotenv
from openai import OpenAI

# Load environment variables from the .env file
load_dotenv()

# Create OpenAI client
client = OpenAI(api_key=os.getenv("OPENAI_API_KEY"))

print("Welcome to Rule vs AI Classifier\n")

# Ask the Genius for a user message
message = input("Enter a message to classify: ")

# ----------------------------
# Rule-based classification
# ----------------------------
rule_category = "general"
spam_keywords = ["free", "click now", "prize", "urgent", "winner"]

for keyword in spam_keywords:
    if keyword in message.lower():
        rule_category = "spam"
        break

# ----------------------------
# OpenAI-powered classification
# ----------------------------
prompt = f"""
You are a classification system.

Classify the following message into one of these categories:
- spam
- school
- personal
- general

Message:
"{message}"

Return your answer in this exact format:
Category: <one category>
Reason: <short explanation>
"""

response = client.responses.create(
    model="gpt-4.1-mini",
    input=prompt
)

# ----------------------------
# Print results
# ----------------------------
print("\n--- Rule-Based Result ---")
print(f"Category: {rule_category}")

print("\n--- OpenAI Result ---")
print(response.output_text)

print("\n--- Reflection ---")
print("Which system felt more flexible?")
print("Which system felt more predictable?")
print("When would you want to combine both?")
```
#### **Guided Practice Teaching Points**

-   Why rules are transparent but limited
-   Why the AI classifier can handle more flexible language
-   Why the OpenAI output should still be constrained with categories
-   Why models should often be guided into structured responses
-   Why comparing system approaches is a real engineering practice

#### **Guided Practice Discussion**

-   Which system felt more useful?
-   Which one was easier to trust?
-   What kinds of messages would break the rule-based version?
-   How could a real product combine rules and AI together?

### 4. **Independent Practice (Time: 30 minutes)**

-   **Objective:** Geniuses independently build a first OpenAI-powered AI Systems mini-tool connected to their own use case.
-   This continues the Week 1 mini-project.

#### **Mini-Project Title**

**AI System Concept Brief --- Day 4 First API Prototype**

#### **Independent Task**

Each Genius creates a Python file that uses the OpenAI API to do one structured system task related to their idea.

Examples:

-   classify a message
-   sort a user request into categories
-   label a task by urgency
-   identify a likely support category
-   summarize a short system description into structured fields

Their mini-tool must include:

-   a system name
-   one user input
-   one clearly defined task
-   structured output
-   one trust or review note

#### **Required Deliverables**

-   A working Python file called `my_api_system.py`
-   A working `.env` file configured locally
-   A mini-tool with:
    -   system name
    -   user input
    -   one AI-powered task
    -   structured output
    -   one trust or review consideration
-   A short written reflection:
    -   Why does this tool benefit from AI instead of only rules?
    -   What could go wrong if the output is wrong?
    -   How could you improve trust in this system?

#### **Independent Practice Starter Code**
```
# my_api_system.py
# Day 4 independent practice
# This program uses the OpenAI API for a simple classification task.

import os
from dotenv import load_dotenv
from openai import OpenAI

load_dotenv()
client = OpenAI(api_key=os.getenv("OPENAI_API_KEY"))

system_name = "SupportRoute AI"
user_input = input("Describe what kind of help you need: ")

prompt = f"""
You are a routing system.

Classify the user's request into one of these categories:
- homework
- scheduling
- personal support
- general question

User request:
"{user_input}"

Return your answer in this exact format:
Category: <one category>
Reason: <short explanation>
"""

response = client.responses.create(
    model="gpt-4.1-mini",
    input=prompt
)

print(f"\nSystem Name: {system_name}")
print("\n--- AI Output ---")
print(response.output_text)

print("\nTrust Note: This output should help guide the next step, but a human should review important or sensitive cases.")
```
#### **Facilitator Support Moves**

-   Help Geniuses choose a narrow, structured use case
-   Ask:
    -   What is the system trying to decide or organize?
    -   Why are fixed rules not enough here?
    -   What output format would make this usable in a real app?
    -   What trust note or review step should be included?
-   Encourage small, well-scoped API tasks rather than huge ideas

### 5. **Closure (Time: 15 minutes)**

-   **Objective:** Reinforce that model APIs are powerful system components, but they still need structure, constraints, and responsibility.
-   Bring the class together for a final share-out.
-   Ask 3--5 Geniuses to share:
    -   their system name
    -   the task their API prototype performs
    -   one reason AI helped more than rules
    -   one trust issue they noticed
-   Lead a closing discussion:
    -   When are rules enough?
    -   When does AI add value?
    -   Why does using an API still require technical thinking?
-   Preview the next lesson:
    -   Geniuses will expand into recommendation, ranking, and pattern-based systems and continue learning how AI systems go beyond simple category decisions.

**Assessment:**
---------------

Student learning will be assessed through:

-   Participation in the icebreaker and discussion
-   Reflection responses during direct instruction
-   Completion of the guided rule-vs-AI classifier build
-   Completion of an independent API-powered mini-tool
-   Final share-out and explanation of system choices

### **Exit Ticket**

1.  What is the difference between a rule-based system and an AI-powered system?
2.  Why is structured output useful when using an API?
3.  What is one system task where AI helps more than fixed rules?

**Extra Activities:**
---------------------

-   Geniuses who finish early can:
    -   add a confidence field to their prompt output
    -   compare three different user messages
    -   add a second rule-based category set
    -   return JSON instead of plain text format
    -   add a "needs human review" category
    -   test where the rule-based system fails badly
-   Add a fallback rule if the AI output is unclear
-   Add a second version with different categories
-   Add a "why not rules?" reflection section
-   Add a combined system where rules run first and AI handles the uncertain cases

**Reflection / Takeaways:**
---------------------------

This lesson works best when Geniuses realize that modern AI systems do not replace systems design. They deepen it. Day 4 introduces the OpenAI API in a way that stays grounded in technical thinking, comparison, and responsibility. By the end of the lesson, Geniuses should understand that calling a model is not the same as building a thoughtful AI system. Good builders still define the task, constrain the output, compare approaches, and design for trust.

**Facilitator Notes**
---------------------

-   Keep using **Geniuses** consistently in examples and discussion.
-   Reinforce that the OpenAI API is one component inside a system.
-   Encourage narrow, structured, technical use cases instead of vague chatbot prompts.
-   Keep the comparison between rules and AI central to the lesson.
-   Remind Geniuses that tomorrow they will continue exploring pattern-based systems and connect what they have learned into a stronger Week 1 system concept.

**Week 1 Day 4 Mini-Project Connection**
----------------------------------------

By the end of Day 4, each Genius should have:

-   A first OpenAI-powered AI Systems mini-tool
-   A clearer sense of when AI adds value over simple rules
-   Experience using the OpenAI API in Python
-   A structured system task such as classification or routing
-   At least one trust or review note
-   A stronger foundation for technical AI systems building
