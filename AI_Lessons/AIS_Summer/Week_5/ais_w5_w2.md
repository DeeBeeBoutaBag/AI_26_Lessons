<img src="https://github.com/Hgp-GeniusLabs/Curriculum/blob/10734f2c827128dde773ea4f266d154d46977866/Org-Wide/Assets/hgp_logo_original.png" width="150"/>

Lesson Plan: AI Systems Week 5, Day 2 --- READMEs, Technical Documentation, and Explaining the System Clearly
===========================================================================================================

**Duration:**
-------------

3 hours

**Lesson Overview:**
--------------------

On Day 2, Geniuses focus on one of the most important parts of making a capstone real: **documentation**. After defining a capstone vision and tech principles on Day 1, Geniuses now learn how to clearly explain what their AI software is, how it works, how someone should run it, and what it is still trying to become. This lesson centers on two key artifacts: the **README** and the **technical documentation file**.

Geniuses learn that a strong README is the front door to the project. It should help a teammate, facilitator, judge, investor, or future builder quickly understand the app, the user, the problem, the features, and the setup. They also learn that technical documentation is where the system architecture, workflows, AI components, and limitations become clear. During guided practice, the class builds a Python-based documentation organizer and drafts a GitHub-ready `README.md` and `TECHNICAL_DOC.md`. During independent practice, each Genius creates documentation for their own capstone concept. By the end of the lesson, Geniuses should understand that if a product cannot be explained clearly, it is not ready to build or pitch well.

**Objectives:**
---------------

-   Explain what a README is and why it matters in technical and product work.
-   Distinguish between a README and a technical documentation file.
-   Identify the core sections of a strong GitHub-ready `README.md`.
-   Identify the core sections of a strong `TECHNICAL_DOC.md`.
-   Build a Python-based documentation organizer in VS Code.
-   Create a first version of capstone documentation for an AI software product.
-   Reflect on how documentation supports clarity, trust, collaboration, and build readiness.

**Materials:**
--------------

-   Laptops for all Geniuses
-   VS Code installed
-   Python installed and working
-   Internet access
-   Projector or display
-   Whiteboard and markers
-   Slide deck for lecture and discussion
-   Reflection journal or digital notes
-   Terminal access in VS Code
-   Existing capstone concept work from Week 5 Day 1
-   Starter folder for Python files
-   Markdown preview in VS Code

**Standards:**
--------------

-   Computational Thinking: Organize system information into clear structures that support understanding and reuse.
-   Computer Science Practices: Document technical workflows, product purpose, and setup clearly.
-   Technical Communication: Write documentation for multiple audiences including teammates, facilitators, judges, and future builders.
-   Digital Literacy: Evaluate how documentation improves transparency, continuity, and professionalism.
-   Career Readiness: Practice professional technical writing and project organization.
-   Technical Foundations: Explain an AI system through product documentation and technical documentation.

**Lesson Activity:**
--------------------

### 1. **Introduction (Time: 25 minutes)**

-   **Objective:** Energize Geniuses and introduce the idea that great software work needs great explanation.
-   Start with a fun icebreaker called **"Could Someone Else Use This?"**
-   This should be the first thing and the most fun thing to wake Geniuses up and get them ready for the lesson.

#### **Icebreaker Option A: Physical Movement**

-   Label one side of the room **"Clear Enough"** and the other side **"Needs Better Docs."**
-   Read project scenarios aloud and have Geniuses move to the side that best matches.
-   Example prompts:
    -   A project has a cool demo but no setup instructions
    -   A project explains the problem, user, tech stack, and how to run it
    -   A project has strong code but no README
    -   A project has a README, but it does not explain what the AI system actually does
    -   A project explains what works, what is unfinished, and what comes next
    -   A project includes screenshots but no product summary
-   After each round, ask:
    -   What is missing here?
    -   What would confuse a teammate or judge?
    -   Why do docs matter even if the product looks strong?
    -   What makes a project feel professional?

#### **Icebreaker Option B: README Critique**

-   Show two short README openings:
    -   one vague and generic
    -   one clear and product-focused
-   Ask Geniuses:
    -   Which one makes you trust the project more?
    -   Which one makes the product easier to understand?
    -   What is missing from the weaker version?

#### **Transition**

-   Say:
    -   "A README is not extra. It is part of the product. Documentation is how the system becomes understandable."
-   Ask:
    -   If someone opened your capstone today, what would they understand right away?
    -   What would still be confusing?

### 2. **Direct Instruction (Time: 50 minutes)**

-   **Objective:** Help Geniuses understand the purpose, audience, and structure of strong README and technical documentation files.
-   Use slides to guide instruction and keep it interactive.

#### **Suggested Slide Flow**

-   **Slide 1: Why Documentation Matters**
    -   Documentation helps people understand, run, continue, critique, and trust a project
    -   Capstones feel more serious when they are documented well
-   **Slide 2: What Is a README?**
    -   A README is the front door to the project
    -   It explains:
        -   what the product is
        -   who it is for
        -   what problem it solves
        -   what it includes
        -   how to run it
        -   what comes next
-   **Slide 3: What Is Technical Documentation?**
    -   Technical documentation explains:
        -   how the system works
        -   AI components used
        -   inputs and outputs
        -   workflow
        -   dependencies
        -   limitations
        -   architecture decisions
-   **Slide 4: README vs Technical Doc**
    -   **README**
        -   product-facing
        -   quick understanding
        -   project overview
    -   **Technical doc**
        -   system-facing
        -   deeper explanation
        -   workflow and implementation detail
-   **Slide 5: Strong README Sections**
    -   project title
    -   one-sentence summary
    -   problem
    -   user
    -   features
    -   AI system behavior
    -   tech stack
    -   setup instructions
    -   roadmap or next steps
-   **Slide 6: Strong Technical Doc Sections**
    -   system purpose
    -   inputs
    -   outputs
    -   workflow
    -   AI components
    -   file structure
    -   dependencies
    -   limitations
    -   future build priorities
-   **Slide 7: Who Are You Writing For?**
    -   teammate
    -   facilitator
    -   judge
    -   investor
    -   mentor
    -   future-you
-   **Slide 8: Common Documentation Mistakes**
    -   too vague
    -   too much jargon
    -   missing setup steps
    -   no product explanation
    -   no trust or limitation note
    -   no clear AI system explanation
-   **Slide 9: Why Documentation Matters for AI**
    -   AI projects need extra clarity because people need to know:
        -   what the system does
        -   what AI behavior it uses
        -   what users should and should not trust
        -   what limitations exist
-   **Slide 10: Week 5 Direction**
    -   Geniuses are building the full capstone package: docs, trust policies, prototype plans, and pitch materials

#### **Discussion Questions**

-   Why does a project need both a README and a technical doc?
-   What makes a README useful instead of just long?
-   Why should limitations be documented honestly?
-   What would a judge want to understand quickly?
-   Why are docs especially important for AI software?

#### **Reflection Prompt**

-   Have Geniuses write for 4 minutes:
    -   "If someone opened your capstone today, what are the first three things they would need to understand?"

### 3. **Guided Practice (Time: 50 minutes)**

-   **Objective:** Help Geniuses build a Python-based documentation organizer and start drafting a `README.md` and `TECHNICAL_DOC.md`.
-   Explain that today's code-along is about structuring what the project says about itself.
-   The class will create `doc_builder.py`.

#### **Guided Practice Build**

Create a folder called `capstone-doc-builder`.

#### **Project Goal**

Build a Python program that:

-   asks the user for key documentation sections
-   prints a structured summary
-   gives Geniuses a foundation for writing `README.md` and `TECHNICAL_DOC.md`

#### **Setup Steps**

1.  Open VS Code.
2.  Create a folder called `capstone-doc-builder`.
3.  Create a file called `doc_builder.py`.
4.  Create two markdown files:
    -   `README.md`
    -   `TECHNICAL_DOC.md`
5.  Run the Python file in the terminal and use the answers to draft both docs.

#### **Sample Code**
```
# doc_builder.py
# AI Systems Week 5 Day 2
# This program helps Geniuses organize capstone documentation.

print("Welcome to the Capstone Documentation Builder\n")

project_name = input("Project name: ")
summary = input("One-sentence project summary: ")
user = input("Who is the product for? ")
problem = input("What problem does it solve? ")
ai_behavior = input("What AI system behavior does it use? ")
features = input("List 2 to 3 main features: ")
tech_stack = input("What tech stack does it use? ")
setup = input("What is one basic setup step? ")
limitation = input("What is one current limitation? ")

print("\n--- Documentation Summary ---")
print(f"Project Name: {project_name}")
print(f"Summary: {summary}")
print(f"User: {user}")
print(f"Problem: {problem}")
print(f"AI Behavior: {ai_behavior}")
print(f"Features: {features}")
print(f"Tech Stack: {tech_stack}")
print(f"Setup Step: {setup}")
print(f"Limitation: {limitation}")

print("\n--- Reflection ---")
print("What should a README explain first?")
print("What should a technical doc explain more deeply?")
print("What should the user never have to guess?")
```
#### **Sample `README.md`**
```
# CourtSense AI

CourtSense AI is an AI-powered sports analytics software concept that helps coaches and athletes review practice footage and turn visual movement into clearer training insight.

## Problem
Practice footage can be difficult to review quickly and consistently without extra support.

## User
Basketball coaches and athletes.

## Why It Matters
The product helps users turn sports video into useful insight about spacing, movement, and training patterns.

## AI System Behavior
- Computer vision
- Object detection
- Tracking
- Multimodal agent feedback

## Features
- Review practice footage
- Detect movement patterns
- Generate coaching support insights
- Provide structured next-step guidance

## Tech Stack
- Python
- OpenAI API
- Computer vision workflow concepts
- Optional voice and multimodal outputs

## Setup
1. Open the project in VS Code
2. Install dependencies
3. Add environment variables if using APIs
4. Run the prototype script

## Roadmap
- Improve prototype workflow
- Add stronger visual feedback
- Add spoken coaching summaries
- Prepare full capstone demo
```
#### **Sample `TECHNICAL_DOC.md`**
```
# Technical Documentation: CourtSense AI

## System Purpose
CourtSense AI is a vision-based AI software concept that helps coaches and athletes review basketball footage and identify movement, spacing, and training insights.

## Inputs
- Practice footage or training video
- Optional user goal or coaching focus

## Outputs
- Movement summaries
- Tracking-based insights
- Structured coaching suggestions
- Optional spoken response or future multimodal output

## AI Components
- Computer vision concepts
- Object detection
- Tracking
- Agent reasoning workflow
- Optional text-to-speech and image generation workflows

## Workflow
1. User provides video or frame context
2. System identifies relevant visual patterns
3. Agent organizes findings
4. System returns structured insight
5. Human coach reviews output

## Tech Stack
- Python
- OpenAI API
- VS Code environment
- Future prototype expansion possible with web UI

## Current Limitations
- Prototype is still concept-level and not full real-time vision
- Output depends on workflow design and future implementation detail
- Human review is still required for meaningful coaching use

## Next Technical Priorities
- Define MVP workflow
- Improve frame-based logic
- Build clearer prototype outputs
- Add better trust and review handling
```
#### **Guided Practice Teaching Points**

-   Why the README should be easier to scan than the technical doc
-   Why technical docs should explain the workflow clearly
-   Why limitations should be honest
-   Why setup steps matter even in a prototype
-   Why documentation is part of product credibility

#### **Guided Practice Discussion**

-   Which section feels most important in the README?
-   Which section feels most important in the technical doc?
-   What would make these docs stronger?
-   What should a builder never leave out?

### 4. **Independent Practice (Time: 35 minutes)**

-   **Objective:** Geniuses independently create capstone documentation files for their project.
-   This continues the Week 5 capstone launch package.

#### **Mini-Project Title**

**Capstone Launch Package --- Day 2 README and Technical Documentation**

#### **Independent Task**

Each Genius creates:

-   `README.md`
-   `TECHNICAL_DOC.md`

Their files must explain:

-   project title
-   one-sentence summary
-   user
-   problem
-   AI behavior
-   features
-   tech stack
-   setup
-   workflow
-   limitations
-   roadmap or next steps

#### **Required Deliverables**

-   A working Python file called `my_doc_builder.py`
-   A completed `README.md`
-   A completed `TECHNICAL_DOC.md`
-   Documentation that includes:
    -   product overview
    -   AI system explanation
    -   features
    -   setup
    -   limitations
    -   future direction
-   A short written reflection:
    -   What part of your documentation feels strongest?
    -   What still needs clarification?
    -   How will these docs help during the capstone build?

#### **Independent Practice Starter Code**
```
# my_doc_builder.py
# Week 5 Day 2 independent practice
# This program prints a simple capstone documentation summary.

print("My Capstone Documentation Summary\n")

project_name = "StudyLens AI"
summary = "A multimodal agent that helps Geniuses understand worksheets and diagrams through image-aware reasoning and spoken support."
user = "High school Geniuses"
problem = "Students often need clearer help understanding visual academic materials."
ai_behavior = "Vision + reasoning + TTS agent workflow"
features = "Worksheet explanation, key finding summary, spoken guidance"
tech_stack = "Python, OpenAI API, TTS workflow"
setup = "Install dependencies, add API key, run the Python agent script"
limitation = "The system may misunderstand unclear or low-quality visuals"

print(f"Project Name: {project_name}")
print(f"Summary: {summary}")
print(f"User: {user}")
print(f"Problem: {problem}")
print(f"AI Behavior: {ai_behavior}")
print(f"Features: {features}")
print(f"Tech Stack: {tech_stack}")
print(f"Setup: {setup}")
print(f"Limitation: {limitation}")
```
#### **Facilitator Support Moves**

-   Help Geniuses make their docs specific and readable
-   Ask:
    -   Would a new person understand the product from the first paragraph?
    -   Are the AI system behaviors named clearly?
    -   Are setup instructions simple enough?
    -   Are limitations honest and useful?
-   Encourage strong headings and product clarity

### 5. **Closure (Time: 20 minutes)**

-   **Objective:** Reinforce that documentation is part of technical maturity and product readiness.
-   Bring the class together for a final share-out.
-   Ask 3--5 Geniuses to share:
    -   their project name
    -   one README section they are proud of
    -   one technical detail they documented
    -   one limitation they included honestly
-   Lead a closing discussion:
    -   What makes documentation strong?
    -   Why should limitations be documented instead of hidden?
    -   How do docs help a capstone feel more real and serious?
-   Preview the next lesson:
    -   Geniuses will focus on data use, trust boundaries, AI policies, and responsible design rules for their capstone systems.

**Assessment:**
---------------

Student learning will be assessed through:

-   Participation in the icebreaker and discussion
-   Reflection responses during direct instruction
-   Completion of the guided documentation builder
-   Completion of independent `README.md` and `TECHNICAL_DOC.md`
-   Final share-out and explanation of documentation choices

### **Exit Ticket**

1.  What is a README?
2.  What is one difference between a README and a technical doc?
3.  Why should limitations be documented honestly?

**Extra Activities:**
---------------------

-   Geniuses who finish early can:
    -   add a "future features" section
    -   add a "who should use this" section
    -   add a file structure section
    -   add a "what this product should not be used for" note
    -   add a short product pitch into the README
    -   improve formatting and headings
-   Add a "known issues" section
-   Add a "why AI is used here" section
-   Add a "trust note" section
-   Add a "demo plan" placeholder

**Reflection / Takeaways:**
---------------------------

This lesson works best when Geniuses realize that strong software is not only coded well. It is explained well. Day 2 helps them turn their capstone concept into something another person can understand, run, and build on. By the end of the lesson, Geniuses should feel that their project is more real because it now has documentation that reflects product thinking, technical clarity, and honest limitations.

**Facilitator Notes**
---------------------

-   Keep using **Geniuses** consistently in examples and discussion.
-   Reinforce that concise, clear writing is stronger than vague or overly complicated writing.
-   Encourage honesty about limitations and unfinished work.
-   Help Geniuses name the AI system behavior clearly in their docs.
-   Remind Geniuses that tomorrow they will create data, trust, and AI policy documents for their capstone.

**Week 5 Day 2 Mini-Project Connection**
----------------------------------------

By the end of Day 2, each Genius should have:

-   A GitHub-ready `README.md`
-   A `TECHNICAL_DOC.md`
-   A clearer explanation of their capstone product
-   A clearer explanation of their AI system workflow
-   Honest setup notes and limitations
-   A stronger foundation for trust policy, prototype planning, and pitching
