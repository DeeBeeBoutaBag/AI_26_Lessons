<img src="https://github.com/Hgp-GeniusLabs/Curriculum/blob/10734f2c827128dde773ea4f266d154d46977866/Org-Wide/Assets/hgp_logo_original.png" width="150"/>

Lesson Plan: AI Systems Week 2, Day 4 --- Multimodal AI Systems, Video Generation Concepts, and Mixed-Input Workflows
===================================================================================================================

**Duration:**
-------------

3 hours

**Lesson Overview:**
--------------------

On Day 4, Geniuses expand beyond single-input generative systems into **multimodal AI systems**. After exploring text generation and image generation, Geniuses now focus on systems that combine different kinds of inputs and outputs such as text plus image, image plus text, and conceptually text-to-video or image-to-video workflows. The lesson introduces the idea that many of the most modern AI systems are not limited to one mode. They can interpret, connect, transform, and generate across multiple forms of information.

Geniuses explore how multimodal systems can power software products that analyze images, generate captions, design visual content, interpret diagrams, or create richer creative workflows. They also get an introduction to **video generation concepts**, not as a deep research topic, but as a modern extension of generative AI systems. During guided practice, the class builds a Python-based multimodal workflow planner that takes mixed inputs and designs a system response. During independent practice, each Genius creates a multimodal AI software concept that uses at least two forms of information together. By the end of the lesson, Geniuses should understand that multimodal AI systems are a major part of where modern AI products are going.

**Objectives:**
---------------

-   Define multimodal AI and explain how it differs from single-mode AI systems.
-   Identify common multimodal workflows such as image-to-text, text-to-image, text-plus-image reasoning, and mixed-input generation.
-   Explain the basic concept of video generation as an extension of generative systems.
-   Analyze how multimodal AI can support real software products and venture ideas.
-   Build a Python-based multimodal workflow planner in VS Code.
-   Reflect on the technical and ethical challenges of mixed-input AI systems.
-   Continue the Week 2 mini-project by designing a multimodal generative AI software concept.

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
-   Existing Week 2 files
-   `.env` setup instructions for API keys

**Standards:**
--------------

-   Computational Thinking: Analyze how systems process multiple forms of input and connect them into useful outputs.
-   Computer Science Practices: Build and test multimodal workflow concepts using structured logic and API-powered tools.
-   Programming: Use Python and the OpenAI API to design mixed-input system workflows.
-   Digital Literacy: Evaluate the opportunities and risks of multimodal and synthetic media systems.
-   Career Readiness: Practice technical design, experimentation, and product thinking.
-   Technical Foundations: Explain multimodal AI as a key modern AI systems behavior.

**Lesson Activity:**
--------------------

### 1. **Introduction (Time: 25 minutes)**

-   **Objective:** Energize Geniuses and introduce the idea that modern AI systems often work across more than one kind of input or output.
-   Start with a fun icebreaker called **"One Mode or Many?"**
-   This should be the first thing and the most fun thing to wake Geniuses up and get them ready for the lesson.

#### **Icebreaker Option A: Physical Movement**

-   Label one side of the room **"Single Mode"** and the other side **"Multimodal."**
-   Read product examples aloud and have Geniuses move to the side they think fits best.
-   Example prompts:
    -   A system that writes a paragraph from a topic
    -   A system that looks at an image and writes a caption
    -   A system that turns a design brief into a poster image
    -   A system that reads a chart image and explains it
    -   A system that takes text, an image reference, and a style goal to generate a new visual
    -   A system that creates a short video concept from a written script
-   After each round, ask:
    -   What makes this single-mode or multimodal?
    -   What kinds of inputs are involved?
    -   What kind of output is being created?
    -   Why might multimodal systems be more powerful or more complex?

#### **Icebreaker Option B: Workflow Breakdown**

-   Put workflows on the board such as:
    -   text → text
    -   text → image
    -   image → text
    -   text + image → text
    -   text + image → image
    -   text → video
-   Ask Geniuses to explain what kind of software product could use each one.
-   Discuss how many modern AI apps are starting to combine these modes.

#### **Transition**

-   Say:
    -   "The future of AI software is not only text or only images. More and more systems are learning to connect different kinds of information."
-   Ask:
    -   What becomes possible when a system can interpret both words and visuals?
    -   What gets harder when more modes are combined?

### 2. **Direct Instruction (Time: 55 minutes)**

-   **Objective:** Help Geniuses understand multimodal AI systems and video generation concepts in a modern, product-relevant way.
-   Use slides to guide instruction and keep it interactive.

#### **Suggested Slide Flow**

-   **Slide 1: What Is Multimodal AI?**
    -   Multimodal AI systems work with more than one type of information
    -   Examples of modes:
        -   text
        -   image
        -   audio
        -   video
        -   structured data
-   **Slide 2: Single-Mode vs Multimodal Systems**
    -   Single-mode:
        -   one input type
        -   one output type
    -   Multimodal:
        -   mixed input and/or mixed output
        -   richer reasoning and generation possibilities
-   **Slide 3: Common Multimodal Workflows**
    -   image → caption
    -   text → image
    -   text + image → explanation
    -   text + image → new design concept
    -   image + question → answer
    -   script → visual concept → video planning
-   **Slide 4: Why Multimodal AI Matters**
    -   more human-like workflows
    -   stronger creative tools
    -   richer product experiences
    -   better support for design, education, accessibility, and media
-   **Slide 5: Real-World Multimodal Product Ideas**
    -   study tools that explain diagrams
    -   AI design assistants
    -   content creation tools
    -   marketing creative systems
    -   document understanding tools
    -   presentation and storyboard builders
-   **Slide 6: Intro to Video Generation Concepts**
    -   Video generation systems may create:
        -   scenes
        -   motion-based visuals
        -   short clips
        -   storyboard-like outputs
    -   Video generation is harder because:
        -   time matters
        -   consistency across frames matters
        -   motion matters
        -   coherence matters
-   **Slide 7: Multimodal Prompt Design**
    -   What is the user giving the system?
    -   What does the system need to pay attention to?
    -   What should the output look like?
    -   What should stay consistent?
-   **Slide 8: Risks in Multimodal and Video Systems**
    -   synthetic misinformation
    -   deceptive visuals
    -   fake scenes
    -   visual bias
    -   weak context matching
    -   overtrusting generated media
-   **Slide 9: Responsible Multimodal Design**
    -   be clear when outputs are synthetic
    -   review visuals before real-world use
    -   avoid misleading representations
    -   keep user intent and public trust in mind
    -   design for transparency
-   **Slide 10: Week 2 Direction**
    -   Geniuses are moving toward a generative AI software showcase that can include text, image, and multimodal workflows

#### **Discussion Questions**

-   What makes multimodal AI more powerful than single-mode AI?
-   Why are multimodal systems harder to design?
-   What kinds of ventures could benefit from mixed-input workflows?
-   Why is video generation conceptually more difficult than still-image generation?
-   What trust challenges show up when AI can generate realistic media?

#### **Reflection Prompt**

-   Have Geniuses write for 4 minutes:
    -   "Describe one software app idea that would be stronger if it could work across both text and visuals."

### 3. **Guided Practice (Time: 50 minutes)**

-   **Objective:** Help Geniuses build a Python-based multimodal workflow planner that structures mixed-input AI product ideas.
-   Explain that today's code-along focuses on system design and workflow planning, not only direct output.
-   The class will create `multimodal_workflow_planner.py`.

#### **Guided Practice Build**

Create a folder called `multimodal-workflow-planner`.

#### **Project Goal**

Build a Python program that:

-   asks the user what kind of multimodal app they want to design
-   asks what the inputs are
-   asks what the output should be
-   asks what trust concerns exist
-   prints a structured multimodal workflow summary

#### **Setup Steps**

1.  Open VS Code.
2.  Create a folder called `multimodal-workflow-planner`.
3.  Create a file called `multimodal_workflow_planner.py`.
4.  Run the file in the terminal.

#### **Sample Code**
```
# multimodal_workflow_planner.py
# AI Systems Week 2 Day 4
# This program helps Geniuses design a multimodal AI workflow.

print("Welcome to the Multimodal Workflow Planner\n")

app_name = input("What is the name of your multimodal AI app? ")
input_modes = input("What input modes does it use? (example: text and image) ")
output_mode = input("What output does it create? ")
use_case = input("What real problem or task does it help with? ")
trust_concern = input("What is one trust or ethics concern? ")

print("\n--- Multimodal Workflow Summary ---")
print(f"App Name: {app_name}")
print(f"Input Modes: {input_modes}")
print(f"Output Mode: {output_mode}")
print(f"Use Case: {use_case}")
print(f"Trust Concern: {trust_concern}")

print("\n--- Reflection ---")
print("What makes this app multimodal?")
print("Why are these mixed inputs useful together?")
print("What must be reviewed before using the output seriously?")
```
#### **Optional API Extension**

If you want to use the OpenAI API to help structure a workflow idea:
```
# multimodal_prompt_designer.py
# This program uses the OpenAI API to improve a multimodal workflow idea.

import os
from dotenv import load_dotenv
from openai import OpenAI

load_dotenv()
client = OpenAI(api_key=os.getenv("OPENAI_API_KEY"))

idea = input("Describe your multimodal app idea: ")

prompt = f"""
You are a multimodal AI systems designer.

Take this rough app idea:
"{idea}"

Turn it into a structured multimodal workflow with:
1. App name
2. Input modes
3. Output mode
4. Use case
5. One trust concern
6. One responsible design choice

Return the result in a clean labeled format.
"""

response = client.responses.create(
    model="gpt-4.1-mini",
    input=prompt
)

print("\n--- Multimodal App Workflow ---")
print(response.output_text)
```
#### **Guided Practice Teaching Points**

-   Why multimodal systems need clearer workflow design
-   Why mixed inputs should each serve a real purpose
-   Why multimodal apps should still be simple enough to explain clearly
-   Why trust becomes more important when visuals and media are involved
-   Why workflow clarity matters as much as output creativity

#### **Guided Practice Discussion**

-   What makes the workflow actually multimodal?
-   Which kinds of mixed inputs make the most sense together?
-   What part of a multimodal app would be hardest to build well?
-   What trust concern would matter most in public-facing use?

### 4. **Independent Practice (Time: 30 minutes)**

-   **Objective:** Geniuses independently create a multimodal AI software concept using at least two forms of information together.
-   This continues the Week 2 mini-project.

#### **Mini-Project Title**

**Generative AI System Concept --- Day 4 Multimodal Workflow**

#### **Independent Task**

Each Genius creates a Python file for a multimodal AI system concept.

Examples:

-   diagram explainer app
-   storyboard generator
-   visual study guide builder
-   text-plus-image branding assistant
-   flyer planning and generation system
-   image caption and design refinement app
-   short video concept planner

Their system must include:

-   system name
-   at least two input modes
-   one output mode
-   one product use case
-   one trust or ethics concern
-   one responsible design choice

#### **Required Deliverables**

-   A working Python file called `my_multimodal_system.py`
-   A working `.env` file if using the API extension
-   A system concept with:
    -   system name
    -   input modes
    -   output mode
    -   use case
    -   one trust concern
    -   one responsible design choice
-   A short written reflection:
    -   What makes this system multimodal?
    -   Why are mixed inputs useful here?
    -   What would a user still need to verify?

#### **Independent Practice Starter Code**
```
# my_multimodal_system.py
# Week 2 Day 4 independent practice
# This program creates a multimodal AI system concept.

print("My Multimodal AI System\n")

system_name = "SceneSpark AI"
input_modes = "Text prompt and reference image"
output_mode = "A refined visual concept description for a generated scene"
use_case = "Help creators turn rough scene ideas into stronger visual design directions"
trust_concern = "The generated concept could misrepresent the intended meaning or create misleading visuals"
responsible_design = "The system should clearly show that outputs are AI-generated drafts and require creator review"

print(f"System Name: {system_name}")
print(f"Input Modes: {input_modes}")
print(f"Output Mode: {output_mode}")
print(f"Use Case: {use_case}")
print(f"Trust Concern: {trust_concern}")
print(f"Responsible Design Choice: {responsible_design}")
```
#### **Facilitator Support Moves**

-   Help Geniuses choose mixed inputs that actually strengthen the system
-   Ask:
    -   Why are both input modes needed?
    -   What is the system trying to combine?
    -   What output would be most useful?
    -   What must the user still review carefully?
-   Encourage software concepts that are clear, modern, and product-relevant

### 5. **Closure (Time: 20 minutes)**

-   **Objective:** Reinforce that multimodal AI systems are a major direction in modern AI product design.
-   Bring the class together for a final share-out.
-   Ask 3--5 Geniuses to share:
    -   their system name
    -   the mixed inputs it uses
    -   the output it creates
    -   one trust or ethics concern
-   Lead a closing discussion:
    -   What makes a system multimodal?
    -   Why do mixed-input systems feel more powerful?
    -   What trust challenges increase when systems combine text and visuals?
-   Preview the next lesson:
    -   Geniuses will use flex day to refine and showcase a generative AI software concept that may use text, image, or multimodal workflows.

**Assessment:**
---------------

Student learning will be assessed through:

-   Participation in the icebreaker and discussion
-   Reflection responses during direct instruction
-   Completion of the guided Python multimodal workflow planner
-   Completion of an independent multimodal AI system concept
-   Final share-out and explanation of workflow design and trust choices

### **Exit Ticket**

1.  What is a multimodal AI system?
2.  Why are multimodal systems useful?
3.  What is one trust risk in multimodal or synthetic media systems?

**Extra Activities:**
---------------------

-   Geniuses who finish early can:
    -   add a third input mode concept
    -   create two versions of the same app with different outputs
    -   compare text-plus-image vs text-only workflows
    -   add a "video generation next step" section
    -   use the API to improve the system concept
    -   design a user flow for the app
-   Add a "why both inputs matter" section
-   Add a "how the user reviews output" section
-   Add a "what should never be automated fully" section
-   Add a "possible venture use case" section

**Reflection / Takeaways:**
---------------------------

This lesson works best when Geniuses realize that the most modern AI systems are often not limited to one kind of input or output. Day 4 helps them think beyond text-only or image-only systems and toward richer workflows that reflect how real software products are evolving. By the end of the lesson, Geniuses should feel more confident imagining and designing AI apps that combine multiple forms of intelligence while still being careful about trust, review, and responsible use.

**Facilitator Notes**
---------------------

-   Keep using **Geniuses** consistently in examples and discussion.
-   Reinforce that multimodal systems should still be understandable and purposeful.
-   Encourage mixed-input ideas that solve real tasks, not just flashy demos.
-   Keep trust, transparency, and responsible synthetic media use visible throughout the lesson.
-   Remind Geniuses that tomorrow they will refine and showcase their generative AI system concepts from the week.

**Week 2 Day 4 Mini-Project Connection**
----------------------------------------

By the end of Day 4, each Genius should have:

-   A named multimodal AI system concept
-   At least two input modes
-   A clear output mode
-   A real product use case
-   A Python-based workflow planner or concept script
-   At least one identified trust or ethics concern
-   At least one responsible design choice
-   A stronger understanding of modern mixed-input AI systems
