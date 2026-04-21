<img src="https://github.com/Hgp-GeniusLabs/Curriculum/blob/10734f2c827128dde773ea4f266d154d46977866/Org-Wide/Assets/hgp_logo_original.png" width="150"/>

Lesson Plan: AI Systems Week 4, Day 5 --- Multimodal Agent Studio, Voice + Vision + Image Creation Showcase
=========================================================================================================

**Duration:**
-------------

3 hours

**Lesson Overview:**
--------------------

Day 5 brings together everything Geniuses explored in Week 4: agentic AI, vision-aware reasoning, spoken output with TTS, and image-generating workflows. Today is a studio day focused on refinement, critique, and showcase. Geniuses use work time to strengthen a **multimodal agent system** that can see, reason, speak, and create with real product purpose. The lesson emphasizes that strong agents are not just impressive because they do many things. They must also be useful, structured, and responsibly designed.

Geniuses will refine their agent concept so it clearly explains what the user wants, what the agent sees, what it says, what it creates, and what trust issues must be managed. During guided practice, the class builds a Python-based multimodal agent summary tool that organizes user, goal, vision input, spoken output, image generation purpose, and responsible design choices. During independent practice, each Genius finalizes a multimodal agent concept or prototype and prepares a short showcase. By the end of the lesson, Geniuses should feel that they are not only experimenting with modern AI capabilities. They are learning how to design real multimodal AI software systems.

**Objectives:**
---------------

-   Synthesize key ideas from Week 4 on agentic AI, vision reasoning, TTS, and image generation.
-   Refine a multimodal agent concept so it is technically clearer and more product-ready.
-   Explain why a multimodal agent is the right software pattern for a chosen use case.
-   Identify trust, authority, review, and synthetic media concerns in multimodal agents.
-   Build a Python-based concept summarizer for a multimodal agent system.
-   Present a multimodal agent software concept clearly in terms of user, goal, inputs, outputs, and responsible design.
-   Prepare for deeper AI Systems work in the coming weeks.

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
-   Existing Week 4 files and concept work
-   Starter folder for Python files
-   `.env` setup instructions for API keys
-   Speakers or headphones if voice demos are used

**Standards:**
--------------

-   Computational Thinking: Connect perception, reasoning, voice, and creation into a coherent software workflow.
-   Computer Science Practices: Build and refine a multimodal agent system with clearer product structure and stronger technical explanation.
-   Programming: Use Python and the OpenAI API to support structured agent design and multimodal workflows.
-   Digital Literacy: Evaluate the usefulness, trustworthiness, and risks of agents that can see, speak, and generate.
-   Career Readiness: Practice technical communication, critique, and presentation.
-   Technical Foundations: Explain how modern multimodal agents combine several AI system behaviors into one product.

**Lesson Activity:**
--------------------

### 1. **Introduction (Time: 20 minutes)**

-   **Objective:** Energize Geniuses and frame the day around refining multimodal agents into stronger software ideas.
-   Start with a fun icebreaker called **"Powerful or Useful?"**
-   This should be the first thing and the most fun thing to wake Geniuses up and get them ready for the lesson.

#### **Icebreaker Option A: Physical Movement**

-   Label one side of the room **"Powerful"** and the other side **"Useful."**
-   Read multimodal agent ideas aloud and have Geniuses move to the side that best matches how the idea feels.
-   Example prompts:
    -   An agent that can describe any image and talk back
    -   An agent that explains worksheets aloud for Geniuses
    -   An agent that generates flashy visuals but solves no clear problem
    -   An agent that helps coaches review training images and gives spoken feedback
    -   An agent that creates event flyer concepts for youth organizers
    -   An agent that speaks confidently about everything even when uncertain
    -   An agent that helps low-vision users understand a scene
-   After each round, ask:
    -   What makes this mostly powerful or actually useful?
    -   Who is it helping?
    -   What real task does it solve?
    -   What trust issue matters most?

#### **Icebreaker Option B: Agent Critique Filter**

-   Put multimodal agent ideas on the board.
-   Ask Geniuses to sort them into:
    -   useful and realistic
    -   interesting but weak
    -   powerful but needs strict guardrails
-   Discuss how multimodal agents become stronger when they are tied to real users and real workflows.

#### **Transition**

-   Say:
    -   "This week was not just about showing that an agent can see, speak, and create. It was about learning when those capabilities actually make a better product."
-   Ask:
    -   What makes a multimodal agent worth building?
    -   What makes a multimodal agent trustworthy enough to use?

### 2. **Direct Instruction (Time: 40 minutes)**

-   **Objective:** Help Geniuses review the core ideas from the week and prepare to refine and present their multimodal agent concepts.
-   Use slides to guide instruction and keep it interactive.

#### **Suggested Slide Flow**

-   **Slide 1: Week 4 Wrap-Up --- Agents That See, Speak, and Create**
    -   This week focused on multimodal agents that combine vision, reasoning, voice, and image generation
    -   Geniuses moved from simple agent ideas into more embodied AI software systems
-   **Slide 2: What Makes a Multimodal Agent Strong?**
    -   clear user
    -   clear goal
    -   clear reason for vision
    -   clear reason for voice
    -   clear reason for image generation
    -   trust and review design
-   **Slide 3: Weak Multimodal Agent Concepts**
    -   too many features with no purpose
    -   no real user
    -   no reason the agent needs all its abilities
    -   overconfident tone
    -   no trust thinking
    -   no structure in workflow
-   **Slide 4: Strong Multimodal Agent Concepts**
    -   specific problem
    -   real workflow
    -   useful outputs
    -   clear boundaries
    -   voice used where it helps
    -   visuals generated when they add value
    -   strong review thinking
-   **Slide 5: Week 4 System Behaviors Reviewed**
    -   vision + reasoning
    -   structured outputs
    -   text-to-speech
    -   image generation
    -   agent workflow design
-   **Slide 6: Why an Agent Is the Right Pattern**
    -   the task involves multiple steps
    -   the system needs perception plus response
    -   the user benefits from mixed input and output
    -   the workflow is more than one answer
-   **Slide 7: Trust and Guardrails in Multimodal Agents**
    -   do not sound more certain than the system is
    -   do not present generated images as factual truth
    -   support human review
    -   avoid risky over-automation
    -   keep the user aware of limits
-   **Slide 8: Product Questions Builders Should Answer**
    -   Who is the user?
    -   What goal does the user have?
    -   What does the agent see?
    -   What does it say?
    -   What does it create?
    -   What should the user still review?
    -   What should the agent never pretend to know?
-   **Slide 9: Showcase Thinking**
    -   Can you clearly explain:
        -   the agent name?
        -   the user?
        -   the goal?
        -   the visual input?
        -   the spoken output?
        -   the created visual output?
        -   the trust concern?
        -   the responsible design choice?
-   **Slide 10: Looking Ahead**
    -   The ideas from Week 4 can directly feed into final AI app and capstone directions
    -   Modern AI products often combine multiple system behaviors like the agents built this week

#### **Discussion Questions**

-   What makes a multimodal agent useful instead of only impressive?
-   Why should every capability in the agent serve a real user need?
-   What trust issue matters most when an agent can both speak and create visuals?
-   How do you know when an agent is overbuilt?
-   What makes a multimodal agent feel product-ready?

#### **Reflection Prompt**

-   Have Geniuses write for 4 minutes:
    -   "What is the strongest part of your multimodal agent concept right now, and what still needs improvement?"

### 3. **Guided Practice (Time: 45 minutes)**

-   **Objective:** Help Geniuses build a Python-based concept summarizer that organizes a multimodal agent system clearly.
-   Explain that today's code-along is about communicating a system idea with technical and responsible clarity.
-   The class will create `multimodal_agent_summary.py`.

#### **Guided Practice Build**

Create a folder called `multimodal-agent-summary`.

#### **Project Goal**

Build a Python program that:

-   asks the user key questions about a multimodal agent concept
-   organizes the answers into a structured summary
-   helps Geniuses explain the concept clearly

#### **Setup Steps**

1.  Open VS Code.
2.  Create a folder called `multimodal-agent-summary`.
3.  Create a file called `multimodal_agent_summary.py`.
4.  Run the file in the terminal.

#### **Sample Code**
```
# multimodal_agent_summary.py
# AI Systems Week 4 Day 5
# This program helps Geniuses summarize a multimodal agent concept.

print("Welcome to the Multimodal Agent Summary Tool\n")

agent_name = input("What is the name of your multimodal agent? ")
user = input("Who is the agent for? ")
user_goal = input("What does the user want help with? ")
visual_input = input("What visual input does the agent use? ")
spoken_output = input("What spoken output does the agent give? ")
image_generation = input("What kind of visual output can the agent generate? ")
trust_concern = input("What is one trust or ethics concern? ")
responsible_design = input("What is one responsible design choice? ")

print("\n--- Multimodal Agent Summary ---")
print(f"Agent Name: {agent_name}")
print(f"User: {user}")
print(f"User Goal: {user_goal}")
print(f"Visual Input: {visual_input}")
print(f"Spoken Output: {spoken_output}")
print(f"Generated Visual Output: {image_generation}")
print(f"Trust Concern: {trust_concern}")
print(f"Responsible Design Choice: {responsible_design}")

print("\n--- Reflection ---")
print("Why does this agent need more than one capability?")
print("What should the user still review before trusting the output?")
print("What makes this agent useful instead of only impressive?")
```
#### **Guided Practice Teaching Points**

-   Why multimodal agent concepts need clear workflow structure
-   Why the user goal matters more than the number of features
-   Why trust concerns should be named directly
-   Why summary tools help builders think more clearly
-   Why a strong concept is a bridge between technical learning and real software design

#### **Guided Practice Discussion**

-   What section of the summary feels most important?
-   What makes a multimodal agent use case feel real?
-   Why should responsible design be included in the summary, not added later?
-   How would this summary help a teammate, judge, or investor understand the product?

### 4. **Independent Practice (Time: 45 minutes)**

-   **Objective:** Geniuses independently refine a multimodal agent concept or prototype and prepare for a short showcase.
-   This completes the Week 4 mini-project.

#### **Mini-Project Title**

**Week 4 Multimodal Agent System --- Showcase Build**

#### **Independent Task**

Each Genius finalizes a multimodal agent concept or prototype that includes:

-   vision
-   spoken output or TTS
-   image generation
-   agent workflow logic

Their concept must clearly explain:

-   agent name
-   user
-   user goal
-   visual input
-   spoken output
-   created visual output
-   why an agent is the correct system pattern
-   one trust or ethics concern
-   one responsible design choice

They may use Python to print the summary or connect parts of their earlier code if they want a stronger prototype.

#### **Required Deliverables**

-   A working Python file called `week4_multimodal_agent_showcase.py`
-   A working `.env` file if API features are used
-   A complete multimodal agent concept with:
    -   agent name
    -   user
    -   user goal
    -   visual input
    -   spoken output
    -   generated visual output
    -   why agent workflow fits
    -   one trust concern
    -   one responsible design choice
-   A short written reflection:
    -   What kind of multimodal agent is this?
    -   Why would a user want it?
    -   What part of the output should never be trusted blindly?

#### **Independent Practice Starter Code**
```
# week4_multimodal_agent_showcase.py
# Week 4 independent practice
# This program prints a refined multimodal agent concept.

print("Week 4 Multimodal Agent System\n")

agent_name = "EventGuide AI"
user = "Youth organizers and student leaders"
user_goal = "Review event visuals, get spoken guidance, and generate new promotional concepts"
visual_input = "Flyer drafts, room setup photos, or event planning visuals"
spoken_output = "Short spoken guidance on what looks strong, what is missing, and what to improve next"
generated_visual_output = "New flyer concept image prompts or event visual concept drafts"
why_agent_fits = "The system needs to inspect visuals, reason about the user's goal, speak useful feedback, and create new visual support as part of one workflow"
trust_concern = "The agent could sound more certain than it should and create visuals that look polished but still misrepresent the event"
responsible_design = "The agent should clearly label generated content as synthetic and require human review before anything is shared publicly"

print(f"Agent Name: {agent_name}")
print(f"User: {user}")
print(f"User Goal: {user_goal}")
print(f"Visual Input: {visual_input}")
print(f"Spoken Output: {spoken_output}")
print(f"Generated Visual Output: {generated_visual_output}")
print(f"Why Agent Workflow Fits: {why_agent_fits}")
print(f"Trust Concern: {trust_concern}")
print(f"Responsible Design Choice: {responsible_design}")
```
#### **Facilitator Support Moves**

-   Help Geniuses focus on clarity, usefulness, and realism
-   Ask:
    -   What exactly does the agent help the user do?
    -   Why are vision, voice, and image generation all needed?
    -   What is the most important trust issue?
    -   What should the user always review before acting on the agent's output?
-   Encourage concepts that are specific, modern, and grounded in real value

### 5. **Closure (Time: 30 minutes)**

-   **Objective:** Celebrate the week's learning and reinforce that modern multimodal agents can be useful, powerful, and responsibly designed.
-   Bring the class together for a Week 4 showcase.
-   Ask 5--7 Geniuses to share:
    -   their agent name
    -   who it is for
    -   what it sees
    -   what it says
    -   what it creates
    -   one trust concern
    -   one responsible design choice
-   Lead a closing discussion:
    -   What did you learn this week about multimodal agents?
    -   What is the difference between a chatbot and an agent?
    -   What makes a multimodal agent feel real and useful?
    -   Why is trust central in systems that can see, speak, and create?
-   Preview the next lesson:
    -   Week 5 will move into the next major AI Systems theme and continue building toward real AI software apps and ventures.

**Assessment:**
---------------

Student learning will be assessed through:

-   Participation in the icebreaker and discussion
-   Reflection responses during direct instruction
-   Completion of the guided concept summary tool
-   Completion of a full Week 4 multimodal agent concept or prototype
-   Final showcase and explanation of technical and responsible design choices

### **Exit Ticket**

1.  What is one capability your multimodal agent includes?
2.  Why is an agent workflow the right pattern for your concept?
3.  What is one trust issue that must be considered in multimodal agents?

**Extra Activities:**
---------------------

-   Geniuses who finish early can:
    -   add a second version of their agent for a different user
    -   add a "what the agent should never do" section
    -   add a short product pitch based on the concept
    -   compare a text-only version and a multimodal version
    -   combine voice and image generation more tightly
    -   add a future feature roadmap
-   Add a "human review checklist"
-   Add a "public use warning" section
-   Add a "best use case / worst use case" section
-   Add a "why now" section

**Reflection / Takeaways:**
---------------------------

This lesson works best when Geniuses realize that multimodal agents are one of the clearest examples of modern AI systems becoming full software experiences. Day 5 helps bring Week 4 together by moving from separate agent capabilities into a stronger product concept that someone else could understand, critique, and build further. By the end of the week, Geniuses should feel more confident explaining what multimodal agents do, how they are structured, and why they must be designed with strong trust, review, and user-value thinking.

**Facilitator Notes**
---------------------

-   Keep using **Geniuses** consistently in examples and discussion.
-   Reinforce that strong agents solve real problems for real users.
-   Encourage concepts that are useful, not only technically impressive.
-   Help Geniuses speak clearly about trust, synthetic output, and human review.
-   Use the showcase to see who is beginning to think like a real AI systems builder.

**Week 4 Wrap-Up**
------------------

By the end of Week 4, each Genius should have:

-   A named multimodal agent concept or prototype
-   A defined user and user goal
-   A clear visual input type
-   A spoken output path or TTS concept
-   An image generation capability or workflow
-   A clear explanation of why an agent pattern fits
-   At least one identified trust or ethics concern
-   At least one responsible design choice
-   A stronger sense of how modern AI agents can become real software
