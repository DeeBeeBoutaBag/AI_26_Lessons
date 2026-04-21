<img src="https://github.com/Hgp-GeniusLabs/Curriculum/blob/10734f2c827128dde773ea4f266d154d46977866/Org-Wide/Assets/hgp_logo_original.png" width="150"/>

Lesson Plan: AI Systems Week 4, Day 4 --- Agents That Generate Images
===================================================================

**Duration:**
-------------

3 hours

**Lesson Overview:**
--------------------

On Day 4, Geniuses take their multimodal agents another step forward by giving them the ability to **generate visual output**. After learning what makes an agent different from a chatbot, building image-aware reasoning agents, and adding spoken output, Geniuses now focus on agents that can **create images as part of solving a task**. This is where Week 4 starts to feel especially modern: the agent can see, reason, speak, and now create.

The lesson emphasizes that image generation should not be treated like a random extra feature. It should be part of a clear workflow. Geniuses explore when an agent should generate an image, what kind of user value that image creates, and how prompt design affects the usefulness of visual output. They also examine the risks of generated visuals, including misleading outputs, stereotypes, weak prompt quality, and overtrust in synthetic visuals. During guided practice, the class builds a Python-based agent workflow that takes a user goal, reasons about what visual output would help, and generates a structured image prompt for creation. During independent practice, each Genius creates an image-generating agent concept or prototype for a real use case. By the end of the lesson, Geniuses should understand that image generation is not just creative output. It is a tool an agent can use to help a user accomplish something.

**Objectives:**
---------------

-   Explain when image generation is a useful agent action and when it is unnecessary.
-   Identify how an agent can use image generation to support a real user goal.
-   Explain how image prompt design affects output quality and usefulness.
-   Build a Python-based agent workflow that plans and generates visual output.
-   Use structured prompt design for an image-generating agent.
-   Reflect on trust, fairness, and review needs in synthetic visual outputs.
-   Continue the Week 4 mini-project by adding image generation capability to an agent system.

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
-   Optional example prompts and generated image concepts

**Standards:**
--------------

-   Computational Thinking: Analyze how an agent decides when and why to generate visual output.
-   Computer Science Practices: Build and test an agent workflow that includes image generation as a system action.
-   Programming: Use Python and the OpenAI API to create an image-generating agent workflow.
-   Digital Literacy: Evaluate the usefulness and risks of generated images in AI products.
-   Career Readiness: Practice technical explanation, critique, and product workflow design.
-   Technical Foundations: Explain image generation as one capability inside a broader multimodal agent system.

**Lesson Activity:**
--------------------

### 1. **Introduction (Time: 25 minutes)**

-   **Objective:** Energize Geniuses and introduce the idea that agents can create visual output to help users solve real problems.
-   Start with a fun icebreaker called **"Should the Agent Generate an Image?"**
-   This should be the first thing and the most fun thing to wake Geniuses up and get them ready for the lesson.

#### **Icebreaker Option A: Physical Movement**

-   Label one side of the room **"Yes, Generate It"** and the other side **"No, Don't Generate It."**
-   Read scenarios aloud and have Geniuses move to the side that best matches.
-   Example prompts:
    -   A user wants a visual flyer concept for a youth event
    -   A user wants to know whether a math answer is correct
    -   A coach wants a drill card visual for practice
    -   A user wants a quick spoken reminder for homework
    -   A student wants a concept image to match a story idea
    -   A user wants help understanding whether a room setup is safe
    -   A business owner wants a brand moodboard starter image
-   After each round, ask:
    -   Why should the agent generate an image here or not?
    -   What user value does the image create?
    -   Could text alone solve this?
    -   What could go wrong if the image is misleading?

#### **Icebreaker Option B: Workflow Match**

-   Put tasks on the board and ask Geniuses:
    -   Does this need text output?
    -   voice output?
    -   image output?
    -   more than one?
-   Discuss how strong agents choose the right tool for the job instead of using every capability all the time.

#### **Transition**

-   Say:
    -   "A strong agent does not generate images just because it can. It generates images when visuals actually help the user move forward."
-   Ask:
    -   When does visual creation become useful?
    -   What makes generated visuals powerful and risky at the same time?

### 2. **Direct Instruction (Time: 55 minutes)**

-   **Objective:** Help Geniuses understand how image generation fits inside agent workflows and why prompt quality and trust matter.
-   Use slides to guide instruction and keep it interactive.

#### **Suggested Slide Flow**

-   **Slide 1: Agents That Can Create**
    -   A modern agent can:
        -   receive a goal
        -   inspect input
        -   reason about what matters
        -   choose a response
        -   generate an image if it would help solve the task
-   **Slide 2: When Should an Agent Generate an Image?**
    -   branding support
    -   event promotion visuals
    -   study diagrams
    -   concept art
    -   scene mockups
    -   drill cards
    -   storyboard ideas
    -   product concept sketches
-   **Slide 3: When Should an Agent Not Generate an Image?**
    -   when text is enough
    -   when the user needs factual verification, not visuals
    -   when the output could be misleading
    -   when the use case is high-stakes and synthetic visuals could confuse people
-   **Slide 4: Image Generation as an Agent Action**
    -   user goal
    -   agent decides whether visual output helps
    -   agent builds a structured prompt
    -   system generates image
    -   user reviews and decides what to keep
-   **Slide 5: Strong Image Prompt Ingredients**
    -   subject
    -   purpose
    -   style
    -   setting
    -   mood
    -   audience
    -   important details
    -   what should be avoided
-   **Slide 6: Product Use Cases**
    -   flyer generation assistant
    -   training diagram builder
    -   creative brand helper
    -   story scene generator
    -   classroom visual explainer
    -   business campaign concept agent
-   **Slide 7: What Makes Generated Images Risky**
    -   deceptive visuals
    -   weak representation
    -   stereotypes
    -   generic outputs
    -   mismatch with user need
    -   users assuming the image is factual
-   **Slide 8: Responsible Image-Generating Agents**
    -   explain that output is synthetic
    -   keep prompts intentional
    -   review before public use
    -   avoid harmful or misleading content
    -   use generation to support creativity, not deception
-   **Slide 9: Agent Workflow Thinking**
    -   The image is not the whole system
    -   The agent still needs:
        -   user goal
        -   reasoning
        -   visual prompt planning
        -   trust language
        -   follow-up or revision support
-   **Slide 10: Week 4 Direction**
    -   Tomorrow Geniuses will combine seeing, speaking, and creating into a more complete multimodal agent showcase

#### **Discussion Questions**

-   When is image generation actually useful in an agent?
-   Why should an agent not generate an image for every task?
-   What makes an image prompt strong?
-   What trust issues matter most when an agent creates visuals?
-   How can an image-generating agent be creative without becoming careless?

#### **Reflection Prompt**

-   Have Geniuses write for 4 minutes:
    -   "Describe one real task where an AI agent should generate a visual output. What should the image help the user do?"

### 3. **Guided Practice (Time: 50 minutes)**

-   **Objective:** Help Geniuses build a Python-based image-generating agent workflow that turns a user goal into a structured visual prompt and image output.
-   Explain that today's code-along is about agent decision-making plus visual generation.
-   The class will create `image_generating_agent.py`.

#### **Guided Practice Build**

Create a folder called `image-generating-agent`.

#### **Project Goal**

Build a Python program that:

-   asks the user for a goal
-   asks what visual output would help
-   creates a structured image prompt
-   generates an image using the OpenAI API
-   saves the image output
-   prints a trust note for review

#### **Setup Steps**

1.  Open VS Code.
2.  Create a folder called `image-generating-agent`.
3.  Open the terminal in VS Code.
4.  Install dependencies:
```
pip install openai python-dotenv
```
1.  Create a `.env` file:
```
OPENAI_API_KEY=your_key_here
```
1.  Create a file called `image_generating_agent.py`

#### **Sample Code**
```
# image_generating_agent.py
# AI Systems Week 4 Day 4
# This program creates an agent workflow that plans
# and generates an image for a user task.

import os
import base64
from dotenv import load_dotenv
from openai import OpenAI

load_dotenv()
client = OpenAI(api_key=os.getenv("OPENAI_API_KEY"))

print("Welcome to the Image-Generating Agent\n")

user_goal = input("What does the user want help creating? ")
audience = input("Who is the image for? ")
style = input("What style should the image have? ")
mood = input("What mood should the image have? ")

prompt_builder = f"""
You are an image-planning agent.

The user's goal is:
"{user_goal}"

The audience is:
"{audience}"

The desired style is:
"{style}"

The mood is:
"{mood}"

Write one strong image generation prompt that includes:
- subject
- purpose
- style
- mood
- audience awareness
- useful visual detail

Return only the final image prompt.
"""

prompt_response = client.responses.create(
    model="gpt-4.1-mini",
    input=prompt_builder
)

final_image_prompt = prompt_response.output_text.strip()

print("\n--- Final Image Prompt ---")
print(final_image_prompt)

image_response = client.images.generate(
    model="gpt-image-1",
    prompt=final_image_prompt,
    size="1024x1024"
)

image_base64 = image_response.data[0].b64_json
image_bytes = base64.b64decode(image_base64)

with open("agent_generated_image.png", "wb") as f:
    f.write(image_bytes)

print("\nSaved generated image to agent_generated_image.png")
print("\nTrust Note: This image is AI-generated and should be reviewed before public or professional use.")
```
#### **Guided Practice Teaching Points**

-   Why the agent first plans the image prompt instead of jumping straight to generation
-   Why user goal and audience matter in visual output
-   Why saving the image file makes the workflow feel like real software
-   Why trust notes should appear with synthetic visuals
-   Why image generation belongs inside a broader workflow, not as a random trick

#### **Guided Practice Discussion**

-   What made the prompt stronger?
-   Why did audience and mood matter?
-   What would a user still need to review after the image is generated?
-   When would this workflow be useful in a real product?

### 4. **Independent Practice (Time: 30 minutes)**

-   **Objective:** Geniuses independently create an image-generating agent concept or prototype for a real use case.
-   This continues the Week 4 mini-project.

#### **Mini-Project Title**

**Multimodal Agent System Concept --- Day 4 Image-Generating Agent**

#### **Independent Task**

Each Genius creates a Python file that adds image generation to their agent concept.

Examples:

-   flyer creation agent
-   training drill card agent
-   brand concept agent
-   story scene builder
-   event promotion visual assistant
-   classroom visual explainer agent

Their system must include:

-   agent name
-   user
-   user goal
-   image generation purpose
-   structured image prompt logic
-   one trust or ethics concern
-   one responsible design choice

#### **Required Deliverables**

-   A working Python file called `my_image_agent.py`
-   A working `.env` file configured locally
-   An image-generating agent concept or prototype with:
    -   agent name
    -   user
    -   user goal
    -   image generation purpose
    -   structured image prompt design
    -   one trust concern
    -   one responsible design choice
-   A short written reflection:
    -   Why does this agent need image generation?
    -   What makes the visual output useful?
    -   What should a human still review before using the image seriously?

#### **Independent Practice Starter Code**
```
# my_image_agent.py
# Week 4 Day 4 independent practice
# This program creates an image-generating agent concept.

print("My Image-Generating Agent\n")

agent_name = "PosterPilot AI"
user = "Student leaders and youth organizers"
user_goal = "Create a strong visual concept for an upcoming event flyer"
image_generation_purpose = "Generate a bold promotional image that matches the event theme and audience"
prompt_design = "The agent should include subject, audience, style, mood, and purpose in the image prompt"
trust_concern = "The generated image could look polished but still misrepresent the event or target audience"
responsible_design = "All generated visuals should be reviewed and revised by a human before being shared publicly"

print(f"Agent Name: {agent_name}")
print(f"User: {user}")
print(f"User Goal: {user_goal}")
print(f"Image Generation Purpose: {image_generation_purpose}")
print(f"Prompt Design Logic: {prompt_design}")
print(f"Trust Concern: {trust_concern}")
print(f"Responsible Design Choice: {responsible_design}")
```
#### **Facilitator Support Moves**

-   Help Geniuses pick a use case where images genuinely help
-   Ask:
    -   Why is a visual output useful here?
    -   What should the image communicate?
    -   What details must the agent include in the prompt?
    -   What should users never assume just because the image looks polished?
-   Encourage useful, bounded, real product workflows

### 5. **Closure (Time: 20 minutes)**

-   **Objective:** Reinforce that image generation can make agents more helpful and creative, but only when used with clear purpose and careful review.
-   Bring the class together for a final share-out.
-   Ask 3--5 Geniuses to share:
    -   their agent name
    -   what kind of visual it creates
    -   why image generation helps the user
    -   one trust or ethics concern
-   Lead a closing discussion:
    -   What makes image generation useful in an agent workflow?
    -   Why should image generation be intentional, not automatic?
    -   What review and trust design should always be included with synthetic visuals?
-   Preview the next lesson:
    -   Geniuses will combine seeing, speaking, and creating into a full multimodal agent concept or prototype showcase.

**Assessment:**
---------------

Student learning will be assessed through:

-   Participation in the icebreaker and discussion
-   Reflection responses during direct instruction
-   Completion of the guided Python image-generating agent build
-   Completion of an independent image-generating agent concept or prototype
-   Final share-out and explanation of creative and responsible design choices

### **Exit Ticket**

1.  When should an agent generate an image?
2.  What makes an image prompt strong?
3.  What is one trust risk in an image-generating agent?

**Extra Activities:**
---------------------

-   Geniuses who finish early can:
    -   generate multiple image prompt versions and compare them
    -   add a "what to avoid" field in the prompt builder
    -   create a second use case for the same agent
    -   add a "revision prompt" round
    -   add a "why this image helps" explanation
    -   combine image generation with spoken output ideas
-   Add an audience-specific visual mode
-   Add a "public use review checklist"
-   Add a "do not use for..." section
-   Add a "future multimodal expansion" section

**Reflection / Takeaways:**
---------------------------

This lesson works best when Geniuses realize that image generation is strongest when it serves a real task inside a bigger agent workflow. Day 4 helps them understand that visual creation is not only about making something impressive. It is about using synthetic visuals intentionally to support design, learning, communication, and planning. By the end of the lesson, Geniuses should feel more confident building agents that create visuals while also recognizing that generated images need careful review, clear purpose, and responsible use.

**Facilitator Notes**
---------------------

-   Keep using **Geniuses** consistently in examples and discussion.
-   Reinforce that image generation should be tied to user value, not only novelty.
-   Encourage prompt planning before image generation.
-   Keep trust, representation, and public-use caution visible.
-   Remind Geniuses that tomorrow they will combine seeing, speaking, and creating into a stronger multimodal agent showcase.

**Week 4 Day 4 Mini-Project Connection**
----------------------------------------

By the end of Day 4, each Genius should have:

-   A named image-generating agent concept or prototype
-   A defined user and user goal
-   A clear reason visual creation helps the workflow
-   A structured image prompt design process
-   Experience using image generation in an agent workflow
-   At least one trust or ethics concern
-   At least one responsible design choice
-   A stronger understanding of how agents can create visuals as part of solving real tasks
