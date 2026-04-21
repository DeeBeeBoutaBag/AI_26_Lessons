<img src="https://github.com/Hgp-GeniusLabs/Curriculum/blob/10734f2c827128dde773ea4f266d154d46977866/Org-Wide/Assets/hgp_logo_original.png" width="150"/>

Lesson Plan: AI Systems Week 4, Day 1 --- What Is an Agent That Can See and Talk?
===============================================================================

**Duration:**
-------------

3 hours

**Lesson Overview:**
--------------------

Week 4 introduces Geniuses to a new kind of AI system: **agentic AI that can see, reason, and respond in more embodied ways**. After studying AI foundations, generative systems, and vision systems, Geniuses now begin combining those ideas into a more advanced software pattern: the **multimodal agent**. Day 1 focuses on what makes an AI system feel agentic and how vision plus conversation create a stronger, more interactive user experience.

Geniuses explore the difference between a simple model response and an agent workflow. They examine how an agent can receive a goal, inspect an image, reason about what it sees, and produce a useful response for a user. They also begin thinking about how spoken output changes the design of an AI system and why multimodal agents can feel more natural, helpful, and powerful. During guided practice, the class builds a Python-based multimodal agent planner that takes a user goal and image-related context, then structures what the agent should do, say, and watch out for. During independent practice, each Genius creates the first version of a vision-and-voice agent system concept for a real use case. By the end of the lesson, Geniuses should understand that agentic AI is not just a chatbot. It is a system that can perceive, decide, and respond with purpose.

**Objectives:**
---------------

-   Define agentic AI and explain how it differs from a simple one-step model response.
-   Explain how an agent can use vision input as part of a larger system workflow.
-   Identify the difference between text-only AI and multimodal agents that can see and respond.
-   Analyze how spoken output changes the user experience of an AI system.
-   Build a Python-based multimodal agent planner in VS Code.
-   Reflect on trust, authority, and review challenges in agents that can see and talk.
-   Begin the Week 4 mini-project by designing a multimodal agent system concept.

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
-   Optional example images or multimodal product examples

**Standards:**
--------------

-   Computational Thinking: Analyze how multimodal agents combine perception, reasoning, and response into one system.
-   Computer Science Practices: Design a workflow for an AI agent that uses vision and conversation.
-   Programming: Use Python to structure an agent system with multimodal inputs and outputs.
-   Digital Literacy: Evaluate the usefulness and risks of agents that can see and speak.
-   Career Readiness: Practice technical explanation, critique, and modern systems design thinking.
-   Technical Foundations: Explain the basics of multimodal agent workflows in modern AI software.

**Lesson Activity:**
--------------------

### 1. **Introduction (Time: 25 minutes)**

-   **Objective:** Energize Geniuses and introduce the idea that modern AI agents can do more than answer text. They can inspect images, reason about what they see, and respond in more natural ways.
-   Start with a fun icebreaker called **"Chatbot or Agent?"**
-   This should be the first thing and the most fun thing to wake Geniuses up and get them ready for the lesson.

#### **Icebreaker Option A: Physical Movement**

-   Label one side of the room **"Chatbot"** and the other side **"Agent."**
-   Read scenarios aloud and have Geniuses move to the side that best matches.
-   Example prompts:
    -   A system answers one question with one paragraph
    -   A system looks at an image of a worksheet and explains it out loud
    -   A system replies to "hello" with a friendly message
    -   A system inspects a picture of a flyer, identifies missing information, and suggests fixes
    -   A system answers "what is AI?" with a definition
    -   A system reviews a training photo, gives feedback, and speaks the next drill instructions
    -   A system creates one response with no memory or task structure
    -   A system receives a goal, checks an image, then decides what to say next
-   After each round, ask:
    -   What makes this a chatbot or an agent?
    -   Is the system only answering, or is it doing a task?
    -   Is it using perception, planning, or multiple steps?
    -   What makes an agent feel more powerful or more risky?

#### **Icebreaker Option B: Multimodal Product Sort**

-   Put product ideas on the board such as:
    -   text-only tutor
    -   image-aware study helper
    -   speaking coach with vision input
    -   chatbot that only returns text
    -   agent that reviews a design and gives spoken suggestions
-   Ask Geniuses to sort them into:
    -   simple response system
    -   multimodal agent
-   Discuss how mixed inputs and mixed outputs change the software experience.

#### **Transition**

-   Say:
    -   "This week, Geniuses start building AI systems that do more than talk. They can see, reason, speak, and eventually create."
-   Ask:
    -   What makes an AI system feel more like an assistant or teammate?
    -   Why does vision make an agent more useful in the real world?

### 2. **Direct Instruction (Time: 55 minutes)**

-   **Objective:** Help Geniuses understand the foundations of multimodal agents that can see and talk.
-   Use slides to guide instruction and keep it interactive.

#### **Suggested Slide Flow**

-   **Slide 1: What Is an Agentic AI System?**
    -   An agentic AI system does more than return one answer
    -   It can:
        -   receive a goal
        -   inspect input
        -   reason through what matters
        -   choose a response or next step
        -   sometimes use tools or workflows
-   **Slide 2: Chatbot vs Agent**
    -   **Chatbot:**
        -   one request
        -   one response
    -   **Agent:**
        -   goal
        -   steps
        -   perception
        -   decisions
        -   outputs connected to a task
-   **Slide 3: What Makes an Agent Multimodal?**
    -   A multimodal agent can work with more than one type of input or output
    -   Example:
        -   image in
        -   text reasoning
        -   spoken response out
-   **Slide 4: Vision + Reasoning + Voice**
    -   These systems can:
        -   inspect a scene
        -   answer a question about what they see
        -   give guidance
        -   speak the response
    -   This creates a more embodied product experience
-   **Slide 5: Real-World Use Cases**
    -   worksheet explainer agent
    -   accessibility assistant
    -   training coach
    -   visual design reviewer
    -   event setup helper
    -   product quality checker
    -   scene-aware support tool
-   **Slide 6: Why Voice Changes the Product**
    -   voice feels more immediate
    -   voice can improve accessibility
    -   voice can feel more natural
    -   voice can also make weak answers sound too convincing
-   **Slide 7: Core Parts of a Vision-and-Voice Agent**
    -   user goal
    -   image or scene input
    -   agent reasoning step
    -   response decision
    -   spoken or text output
    -   trust or review layer
-   **Slide 8: Risks in Agents That Can See and Talk**
    -   overconfidence
    -   weak scene understanding
    -   misleading spoken tone
    -   users trusting the system too quickly
    -   privacy concerns with image input
    -   poor decisions from incomplete context
-   **Slide 9: Responsible Design for Multimodal Agents**
    -   do not pretend certainty
    -   make the task clear
    -   be careful with high-stakes uses
    -   communicate when outputs should be reviewed
    -   design for support, not blind authority
-   **Slide 10: Week 4 Direction**
    -   Geniuses will build toward agents that can see, speak, and later generate visuals as part of solving real tasks

#### **Discussion Questions**

-   What makes an agent different from a simple model response?
-   Why is vision useful in an AI agent?
-   Why does voice make the product feel different?
-   What trust risks increase when an AI speaks with confidence?
-   What kinds of problems fit a vision-and-voice agent best?

#### **Reflection Prompt**

-   Have Geniuses write for 4 minutes:
    -   "Describe one real task where an AI agent would need both vision and spoken output to be truly useful."

### 3. **Guided Practice (Time: 45 minutes)**

-   **Objective:** Help Geniuses build a Python-based multimodal agent planner that structures a vision-and-voice system workflow.
-   Explain that today's code-along is about designing how the agent works before building more advanced capability later in the week.
-   The class will create `vision_voice_agent_planner.py`.

#### **Guided Practice Build**

Create a folder called `vision-voice-agent-planner`.

#### **Project Goal**

Build a Python program that:

-   asks the user for an agent name
-   asks what the agent sees
-   asks what goal the user has
-   asks what kind of spoken response the agent should give
-   asks what trust concern exists
-   prints a structured multimodal agent summary

#### **Setup Steps**

1.  Open VS Code.
2.  Create a folder called `vision-voice-agent-planner`.
3.  Create a file called `vision_voice_agent_planner.py`.
4.  Run the file in the terminal.

#### **Sample Code**
```
# vision_voice_agent_planner.py
# AI Systems Week 4 Day 1
# This program helps Geniuses design a multimodal agent
# that can see and talk.

print("Welcome to the Vision + Voice Agent Planner\n")

agent_name = input("What is the name of your agent? ")
user_goal = input("What does the user want help with? ")
visual_input = input("What kind of image or scene does the agent inspect? ")
spoken_output = input("What kind of spoken response should the agent give? ")
trust_concern = input("What is one trust or ethics concern? ")

print("\n--- Multimodal Agent Summary ---")
print(f"Agent Name: {agent_name}")
print(f"User Goal: {user_goal}")
print(f"Visual Input: {visual_input}")
print(f"Spoken Output: {spoken_output}")
print(f"Trust Concern: {trust_concern}")

print("\n--- Reflection ---")
print("Why does this agent need vision?")
print("Why does spoken output help the user here?")
print("What should a human still review or verify?")
```
#### **Optional Extension**

Add a simple staged workflow output:
```
# optional_agent_steps.py
# This demonstrates how an agent workflow might be structured.

agent_steps = [
    "Step 1: Receive the user's goal",
    "Step 2: Inspect the image or scene",
    "Step 3: Identify the most relevant visual information",
    "Step 4: Decide what guidance to give",
    "Step 5: Return a spoken or text response",
    "Step 6: Add a trust note or review reminder if needed"
]

print("\n--- Example Agent Workflow ---")
for step in agent_steps:
    print(step)
```
#### **Guided Practice Teaching Points**

-   Why an agent needs a clear goal
-   Why visual input should connect directly to the task
-   Why spoken output should serve a real user need
-   Why trust must be part of the workflow, not added later
-   Why agent planning helps make multimodal systems easier to explain and build

#### **Guided Practice Discussion**

-   What kinds of user goals fit this kind of agent?
-   What makes vision necessary in the workflow?
-   What kinds of spoken output are helpful versus distracting?
-   What trust issue would matter most in public or real-world use?

### 4. **Independent Practice (Time: 35 minutes)**

-   **Objective:** Geniuses independently create the first version of a vision-and-voice agent system concept for a real use case.
-   This begins the Week 4 mini-project.

#### **Mini-Project Title**

**Multimodal Agent System Concept --- Day 1 Foundation**

#### **Independent Task**

Each Genius creates a Python file for a multimodal agent concept.

Examples:

-   worksheet explainer agent
-   form review coach
-   accessibility scene helper
-   sports training feedback agent
-   event setup guide
-   design critique agent
-   classroom visual support assistant

Their concept must include:

-   agent name
-   user
-   user goal
-   visual input
-   spoken output
-   one trust or ethics concern
-   one responsible design choice

#### **Required Deliverables**

-   A working Python file called `my_multimodal_agent.py`
-   A system concept with:
    -   agent name
    -   user
    -   user goal
    -   visual input
    -   spoken output
    -   one trust concern
    -   one responsible design choice
-   A short written reflection:
    -   Why is this an agent and not just a chatbot?
    -   Why does the system need vision?
    -   Why should users still verify some of the output?

#### **Independent Practice Starter Code**
```
# my_multimodal_agent.py
# Week 4 Day 1 independent practice
# This program creates a vision-and-voice agent system concept.

print("My Multimodal Agent System\n")

agent_name = "StudyLens AI"
user = "High school Geniuses"
user_goal = "Understand a worksheet or diagram more clearly"
visual_input = "Photo of a worksheet, diagram, or classroom handout"
spoken_output = "Simple spoken explanation of what the image shows and what to focus on next"
trust_concern = "The agent could misunderstand the visual content and explain it incorrectly"
responsible_design = "The agent should present itself as support and encourage the user to double-check important academic details"

print(f"Agent Name: {agent_name}")
print(f"User: {user}")
print(f"User Goal: {user_goal}")
print(f"Visual Input: {visual_input}")
print(f"Spoken Output: {spoken_output}")
print(f"Trust Concern: {trust_concern}")
print(f"Responsible Design Choice: {responsible_design}")
```
#### **Facilitator Support Moves**

-   Help Geniuses choose a task where both vision and voice matter
-   Ask:
    -   What is the user trying to accomplish?
    -   Why must the agent inspect an image or scene?
    -   Why is spoken output useful instead of only text?
    -   What could make the user overtrust this agent?
-   Encourage concepts that are practical, multimodal, and clearly useful

### 5. **Closure (Time: 20 minutes)**

-   **Objective:** Reinforce that multimodal agents combine perception and response into a more advanced AI software pattern.
-   Bring the class together for a final share-out.
-   Ask 3--5 Geniuses to share:
    -   their agent name
    -   what it sees
    -   what it says
    -   one trust or ethics concern
-   Lead a closing discussion:
    -   What makes an AI system agentic?
    -   Why do vision and voice together create a stronger product experience?
    -   What kinds of review and trust design matter most in speaking agents?
-   Preview the next lesson:
    -   Geniuses will begin building deeper vision-and-reasoning agents that inspect images and return more structured guidance.

**Assessment:**
---------------

Student learning will be assessed through:

-   Participation in the icebreaker and discussion
-   Reflection responses during direct instruction
-   Completion of the guided Python multimodal agent planner
-   Completion of an independent multimodal agent concept
-   Final share-out and explanation of system purpose and trust choices

### **Exit Ticket**

1.  What makes an AI system agentic?
2.  Why is vision useful in an AI agent?
3.  What is one trust risk in an agent that can see and talk?

**Extra Activities:**
---------------------

-   Geniuses who finish early can:
    -   add a second user goal for the same agent
    -   add a "when not to trust the agent fully" section
    -   compare a text-only version and a multimodal version
    -   add a "why voice matters" section
    -   add a future feature for image generation later in the week
    -   create a simple step-by-step agent workflow printout
-   Add a "human review needed?" field
-   Add a "what the agent should never do" section
-   Add a "public use warning" section
-   Add a "future voice style" section

**Reflection / Takeaways:**
---------------------------

This lesson works best when Geniuses realize that a multimodal agent is more than a chatbot with extra features. It is a system that combines perception, reasoning, and response into a purposeful workflow. Day 1 sets the tone for Week 4 by helping Geniuses understand that agents that can see and talk feel more natural and more useful, but they also require stronger trust design and clearer responsibility. By the end of the lesson, Geniuses should feel more confident imagining and explaining modern AI agents as real software systems.

**Facilitator Notes**
---------------------

-   Keep using **Geniuses** consistently in examples and discussion.
-   Reinforce that voice can make weak outputs sound more believable, so trust design matters more, not less.
-   Encourage real use cases over vague assistant ideas.
-   Keep the difference between chatbot and agent visible throughout the lesson.
-   Remind Geniuses that tomorrow they will move deeper into image-aware agent workflows and structured visual reasoning.

**Week 4 Day 1 Mini-Project Connection**
----------------------------------------

By the end of Day 1, each Genius should have:

-   A named multimodal agent concept
-   A defined user and user goal
-   A clear visual input type
-   A clear spoken output purpose
-   At least one trust or ethics concern
-   At least one responsible design choice
-   A stronger understanding of what makes an agent that can see and talk feel modern, useful, and responsibly designed
