<img src="https://github.com/Hgp-GeniusLabs/Curriculum/blob/10734f2c827128dde773ea4f266d154d46977866/Org-Wide/Assets/hgp_logo_original.png" width="150"/>

Lesson Plan: AI Systems Week 4, Day 2 --- Building Vision + Reasoning Agents
==========================================================================

**Duration:**
-------------

3 hours

**Lesson Overview:**
--------------------

On Day 2, Geniuses move from defining multimodal agents into building **vision + reasoning agent workflows**. After learning what makes an agent different from a chatbot, Geniuses now focus on agents that can inspect an image, decide what matters, and return a useful response tied to a real user goal. The lesson emphasizes that a vision-capable agent is not just "looking at an image." It is using visual input as part of a larger workflow that includes interpretation, decision-making, and support.

Geniuses explore how image-aware agents can power study tools, accessibility assistants, design feedback systems, sports training helpers, event support agents, and more. They also learn that image understanding is never perfect and that agents need careful prompting, structured outputs, and trust-aware design. During guided practice, the class builds a Python-based image-aware agent workflow using the OpenAI API to inspect an image-related scenario and return structured reasoning. During independent practice, each Genius creates a first image-aware agent prototype for a real use case. By the end of the lesson, Geniuses should understand that a vision agent is a workflow that sees, thinks, and responds with purpose.

**Objectives:**
---------------

-   Explain how vision + reasoning agents differ from simple image analysis tools.
-   Identify how user goals shape what a vision agent should pay attention to in an image.
-   Explain why structured outputs help make image-aware agents more usable in software.
-   Build a Python-based OpenAI image-aware agent workflow in VS Code.
-   Design a multimodal agent that uses image input to provide useful support.
-   Reflect on trust, uncertainty, and review needs in image-aware agents.
-   Continue the Week 4 mini-project by building an image-aware agent system concept.

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
-   `.env` setup instructions for API keys
-   Optional sample images for testing agent ideas

**Standards:**
--------------

-   Computational Thinking: Analyze how agents combine visual input, reasoning steps, and user goals into an output.
-   Computer Science Practices: Build and test a multimodal workflow using vision and structured response logic.
-   Programming: Use Python and the OpenAI API to design an image-aware agent workflow.
-   Digital Literacy: Evaluate the strengths and limits of agents that reason about images.
-   Career Readiness: Practice technical explanation, iteration, critique, and product thinking.
-   Technical Foundations: Explain how image-aware agents use perception plus reasoning to support real tasks.

**Lesson Activity:**
--------------------

### 1. **Introduction (Time: 25 minutes)**

-   **Objective:** Energize Geniuses and introduce the idea that an image-aware agent must do more than describe a picture. It must understand what matters for the user's goal.
-   Start with a fun icebreaker called **"What Should the Agent Notice?"**
-   This should be the first thing and the most fun thing to wake Geniuses up and get them ready for the lesson.

#### **Icebreaker Option A: Physical Movement**

-   Label different parts of the room:
    -   **Describe**
    -   **Analyze**
    -   **Advise**
    -   **Warn**
-   Read image-agent scenarios aloud and have Geniuses move to what the agent mainly needs to do.
-   Example prompts:
    -   A Genius uploads a worksheet and wants help understanding it
    -   A coach uploads a training photo and wants feedback on positioning
    -   A designer uploads a flyer draft and wants critique
    -   A user uploads a room photo and asks whether anything looks unsafe
    -   A student uploads a chart and asks for the main takeaway
    -   An event organizer uploads a poster draft and wants to know what is missing
-   After each round, ask:
    -   What is the user's goal?
    -   What would the agent need to notice in the image?
    -   Is describing enough, or does the agent need to reason further?
    -   What mistake would matter most here?

#### **Icebreaker Option B: Goal Changes Vision**

-   Write one image type on the board, like "basketball practice photo" or "event flyer."
-   Ask Geniuses how the agent's response changes depending on user goal:
    -   explain it
    -   critique it
    -   improve it
    -   find a problem in it
-   Discuss how the same image can require very different reasoning based on purpose.

#### **Transition**

-   Say:
    -   "An agent does not just see the image. It sees the image in relation to the user's goal."
-   Ask:
    -   Why is goal-awareness important in image agents?
    -   Why is a simple visual description not always enough?

### 2. **Direct Instruction (Time: 55 minutes)**

-   **Objective:** Help Geniuses understand how image-aware agent workflows are structured and why reasoning matters after visual input.
-   Use slides to guide instruction and keep it interactive.

#### **Suggested Slide Flow**

-   **Slide 1: What Is a Vision + Reasoning Agent?**
    -   A vision + reasoning agent takes in visual input, interprets what matters, and returns a response connected to a task or goal
    -   It is more than object detection or image labeling
-   **Slide 2: Input, Goal, Reasoning, Output**
    -   A strong image-aware agent workflow often includes:
        -   user goal
        -   image input
        -   visual interpretation
        -   reasoning step
        -   output for the user
-   **Slide 3: Same Image, Different Agent Tasks**
    -   The same image can support:
        -   explanation
        -   critique
        -   summary
        -   warning
        -   recommendation
        -   next steps
    -   The goal changes the workflow
-   **Slide 4: Real-World Use Cases**
    -   worksheet explainer
    -   design feedback agent
    -   accessibility helper
    -   sports training support
    -   event setup checker
    -   document and diagram support
    -   visual planning assistant
-   **Slide 5: Why Structured Output Matters**
    -   Structured output makes agents easier to connect to real apps
    -   Examples:
        -   summary
        -   key findings
        -   next step
        -   warning
        -   confidence or caution note
-   **Slide 6: What Makes a Vision Agent Strong**
    -   clear user goal
    -   focused visual reasoning
    -   useful output format
    -   task-aware response
    -   trust and review language
-   **Slide 7: What Can Go Wrong**
    -   the agent notices the wrong details
    -   the agent overstates certainty
    -   the image is low quality or incomplete
    -   the agent assumes too much
    -   the user trusts the output too quickly
-   **Slide 8: Responsible Image-Agent Design**
    -   keep the task narrow
    -   do not pretend certainty
    -   support review and follow-up
    -   use caution in high-stakes cases
    -   recognize missing context
-   **Slide 9: Image Agents as Product Workflows**
    -   input is only one part
    -   the software also needs:
        -   prompt design
        -   output structure
        -   user guidance
        -   trust notes
        -   interaction flow
-   **Slide 10: Week 4 Direction**
    -   Geniuses will continue adding voice and image generation to these agents so they become more complete multimodal systems

#### **Discussion Questions**

-   Why is a user goal important in a vision agent?
-   What makes an image-aware agent more useful than plain captioning?
-   Why is structured output helpful in real products?
-   What trust issue matters most in image-aware reasoning?
-   What kinds of tasks should image-aware agents handle carefully?

#### **Reflection Prompt**

-   Have Geniuses write for 4 minutes:
    -   "Describe a task where an AI agent would need to inspect an image and then reason about what the user should do next."

### 3. **Guided Practice (Time: 50 minutes)**

-   **Objective:** Help Geniuses build a Python-based image-aware agent workflow using the OpenAI API with structured outputs.
-   Explain that today's code-along focuses on how an agent can inspect a visual scenario and return organized support.
-   The class will create `vision_reasoning_agent.py`.

#### **Guided Practice Build**

Create a folder called `vision-reasoning-agent`.

#### **Project Goal**

Build a Python program that:

-   asks the user for a goal
-   asks the user to describe or reference an image scenario
-   sends the goal and image-related context to the OpenAI API
-   returns a structured agent response with findings, suggested next step, and caution note

#### **Setup Steps**

1.  Open VS Code.
2.  Create a folder called `vision-reasoning-agent`.
3.  Open the terminal in VS Code.
4.  Install dependencies:
```
pip install openai python-dotenv
```
1.  Create a `.env` file:
```
OPENAI_API_KEY=your_key_here
```
1.  Create a file called `vision_reasoning_agent.py`

#### **Sample Code**
```
# vision_reasoning_agent.py
# AI Systems Week 4 Day 2
# This program creates a simple vision + reasoning agent workflow.

import os
from dotenv import load_dotenv
from openai import OpenAI

load_dotenv()
client = OpenAI(api_key=os.getenv("OPENAI_API_KEY"))

print("Welcome to the Vision + Reasoning Agent\n")

user_goal = input("What does the user want help with? ")
image_context = input("Describe the image or visual scene the agent is working from: ")

prompt = f"""
You are a vision-aware support agent.

The user's goal is:
"{user_goal}"

The image or visual scene is described as:
"{image_context}"

Your job is to:
1. Identify the most important visual details for the user's goal
2. Explain what seems most relevant
3. Suggest one useful next step
4. Add one short caution note if the image description may be incomplete or uncertain

Return your answer in this format:

Key Visual Findings:
- ...

Why It Matters:
- ...

Suggested Next Step:
- ...

Caution Note:
- ...
"""

response = client.responses.create(
    model="gpt-4.1-mini",
    input=prompt
)

print("\n--- Vision Agent Output ---")
print(response.output_text)

print("\n--- Reflection ---")
print("Did the output match the user's goal?")
print("What part of the response should still be reviewed by a human?")
```
#### **Guided Practice Teaching Points**

-   Why goal and image context both matter
-   Why structured outputs make agent responses more useful
-   Why image-aware support is stronger than generic response generation
-   Why caution notes matter in multimodal agents
-   Why this is a workflow, not just one model answer

#### **Guided Practice Discussion**

-   What made the output feel agent-like?
-   Did the agent focus on the most important visual details?
-   Why is "suggested next step" valuable?
-   What kind of trust note would matter most in a real app?

### 4. **Independent Practice (Time: 30 minutes)**

-   **Objective:** Geniuses independently create a first image-aware agent prototype tied to a real use case.
-   This continues the Week 4 mini-project.

#### **Mini-Project Title**

**Multimodal Agent System Concept --- Day 2 Vision + Reasoning Agent**

#### **Independent Task**

Each Genius creates a Python file that uses the OpenAI API for a vision-aware agent task.

Examples:

-   worksheet explainer agent
-   flyer feedback agent
-   sports form review agent
-   room setup checker
-   diagram helper
-   design critique agent
-   accessibility scene explainer

Their system must include:

-   agent name
-   user
-   user goal
-   image or scene input type
-   structured output
-   one trust or ethics concern
-   one responsible design choice

#### **Required Deliverables**

-   A working Python file called `my_vision_agent.py`
-   A working `.env` file configured locally
-   A vision-aware agent concept with:
    -   agent name
    -   user
    -   user goal
    -   image input type
    -   structured output sections
    -   one trust concern
    -   one responsible design choice
-   A short written reflection:
    -   Why does this agent need vision plus reasoning?
    -   What makes the output useful to the user?
    -   What should still be verified by a human?

#### **Independent Practice Starter Code**
```
# my_vision_agent.py
# Week 4 Day 2 independent practice
# This program creates a vision-aware agent workflow.

import os
from dotenv import load_dotenv
from openai import OpenAI

load_dotenv()
client = OpenAI(api_key=os.getenv("OPENAI_API_KEY"))

agent_name = "FlyerFix AI"
user = "Student event organizers"
user_goal = input("What kind of feedback does the user want on the flyer? ")
image_context = input("Describe the flyer or visual design: ")

prompt = f"""
You are a design feedback agent.

The user is:
"{user}"

The goal is:
"{user_goal}"

The flyer or visual design is described as:
"{image_context}"

Return in this format:

Main Issue:
- ...

What Works:
- ...

Suggested Fix:
- ...

Review Note:
- ...
"""

response = client.responses.create(
    model="gpt-4.1-mini",
    input=prompt
)

print(f"\nAgent Name: {agent_name}")
print("\n--- Vision Agent Output ---")
print(response.output_text)

print("\nTrust Note: The agent should help guide revision, but final design decisions should still be reviewed by a human.")
```
#### **Facilitator Support Moves**

-   Help Geniuses choose a focused image-aware task
-   Ask:
    -   What does the user want from the image?
    -   What reasoning happens after the visual inspection?
    -   What output format would be most useful?
    -   What should users not trust blindly?
-   Encourage systems that are useful, narrow, and product-relevant

### 5. **Closure (Time: 20 minutes)**

-   **Objective:** Reinforce that image-aware agents are strongest when they combine perception, reasoning, and useful task-focused outputs.
-   Bring the class together for a final share-out.
-   Ask 3--5 Geniuses to share:
    -   their agent name
    -   what kind of image it works with
    -   what it helps the user do
    -   one trust or ethics concern
-   Lead a closing discussion:
    -   What makes a vision + reasoning agent different from a simple image tool?
    -   Why does goal-awareness matter?
    -   What trust design should image-aware agents always include?
-   Preview the next lesson:
    -   Geniuses will add voice and spoken output so their agents can respond in more interactive, embodied ways.

**Assessment:**
---------------

Student learning will be assessed through:

-   Participation in the icebreaker and discussion
-   Reflection responses during direct instruction
-   Completion of the guided Python vision + reasoning agent build
-   Completion of an independent image-aware agent prototype
-   Final share-out and explanation of system value and trust choices

### **Exit Ticket**

1.  What makes a vision + reasoning agent different from simple image labeling?
2.  Why is structured output useful in image-aware agents?
3.  What is one trust risk in an image-aware agent system?

**Extra Activities:**
---------------------

-   Geniuses who finish early can:
    -   add a second output mode such as "warning" or "confidence note"
    -   compare two different user goals for the same image type
    -   add a "needs human review" field
    -   create a stricter output format
    -   build a second vision-agent use case
    -   add a "what the agent should never assume" section
-   Add a "missing context" note
-   Add a "best next action" section
-   Add a "what image quality issue might matter?" section
-   Add a "future TTS response" section

**Reflection / Takeaways:**
---------------------------

This lesson works best when Geniuses realize that an image-aware agent is more than a system that sees. It is a system that sees in order to help with a real task. Day 2 helps Geniuses connect visual interpretation to reasoning, next-step support, and structured outputs that feel product-ready. By the end of the lesson, Geniuses should feel more confident designing agents that inspect images, make useful observations, and return responses that are both helpful and responsibly framed.

**Facilitator Notes**
---------------------

-   Keep using **Geniuses** consistently in examples and discussion.
-   Reinforce that image-aware agents should be goal-driven, not just descriptive.
-   Encourage structured outputs so the systems feel like real software components.
-   Keep trust and uncertainty visible throughout the lesson.
-   Remind Geniuses that tomorrow they will add spoken output and voice experience to these multimodal agents.

**Week 4 Day 2 Mini-Project Connection**
----------------------------------------

By the end of Day 2, each Genius should have:

-   A named vision + reasoning agent concept or prototype
-   A defined user and user goal
-   A clear image or scene input type
-   A structured output format
-   At least one trust or ethics concern
-   At least one responsible design choice
-   A stronger understanding of how image-aware agents move from perception to useful action
