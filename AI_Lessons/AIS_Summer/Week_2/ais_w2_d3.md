<img src="https://github.com/Hgp-GeniusLabs/Curriculum/blob/10734f2c827128dde773ea4f266d154d46977866/Org-Wide/Assets/hgp_logo_original.png" width="150"/>

Lesson Plan: AI Systems Week 2, Day 3 --- Image Generation Systems, Prompt-to-Image Workflows, and Visual AI Creation
===================================================================================================================

**Duration:**
-------------

3 hours

**Lesson Overview:**
--------------------

On Day 3, Geniuses move from text generation into **image generation systems**. After exploring what generative AI is and how text generation systems work, Geniuses now focus on how AI systems create visual outputs from prompts and instructions. The lesson introduces the idea that image generation systems take in descriptive inputs, style guidance, subject details, and constraints, then generate new visual outputs based on learned visual patterns.

Geniuses explore how image generation differs from text generation, why prompt design still matters, and how visual AI is used in design, branding, storytelling, prototyping, advertising, content creation, and product development. They also examine the ethical and technical challenges of image generation, including bias, misleading visuals, copyright questions, stereotypes, synthetic media, and trust. During guided practice, the class builds an image prompt design lab in Python that structures prompts for different visual outcomes and uses the OpenAI API to generate or plan image outputs. During independent practice, each Genius creates a visual AI software concept and a structured prompt workflow for a real use case. By the end of the lesson, Geniuses should understand that image generation is not just "make a picture." It is a technical and creative system with real design choices and real consequences.

**Objectives:**
---------------

-   Define image generation systems and explain how they differ from text generation systems.
-   Identify the core parts of a prompt-to-image workflow.
-   Explain how subject, style, setting, mood, and constraints shape generated visuals.
-   Analyze real-world use cases for image generation in products, business, and creative workflows.
-   Build a Python-based image prompt design lab using structured input patterns.
-   Reflect on trust, bias, originality, and responsibility in image generation systems.
-   Continue the Week 2 mini-project by designing a generative visual AI system concept.

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

-   Computational Thinking: Break down image generation into structured system components and design variables.
-   Computer Science Practices: Build and test prompt-driven visual generation workflows.
-   Programming: Use Python and the OpenAI API to structure an image generation workflow.
-   Digital Literacy: Evaluate the usefulness, risks, and ethics of synthetic visual media.
-   Career Readiness: Practice technical experimentation, prompt design, and creative systems thinking.
-   Technical Foundations: Explain image generation as a modern generative AI system behavior.

**Lesson Activity:**
--------------------

### 1. **Introduction (Time: 25 minutes)**

-   **Objective:** Energize Geniuses and introduce the idea that AI can generate images by interpreting descriptive prompts and visual instructions.
-   Start with a fun icebreaker called **"What Would You Need to Tell the Image Generator?"**
-   This should be the first thing and the most fun thing to wake Geniuses up and get them ready for the lesson.

#### **Icebreaker Option A: Physical Movement**

-   Label different parts of the room:
    -   **Subject**
    -   **Style**
    -   **Setting**
    -   **Mood**
    -   **Details**
-   Read an image idea aloud and have Geniuses move to the part they think matters most to making the image strong.
-   Example prompts:
    -   "A futuristic basketball poster"
    -   "A community event flyer image"
    -   "A calm study desk scene"
    -   "A startup brand mascot"
    -   "A cinematic city at night"
-   After each round, ask:
    -   What does the system need to know first?
    -   What would make the image more specific?
    -   What part changes the output the most?
    -   What happens if the prompt is too vague?

#### **Icebreaker Option B: Prompt Upgrade**

-   Put simple image prompts on the board like:
    -   "A dog"
    -   "A flyer"
    -   "A classroom"
-   Ask Geniuses to improve them by adding:
    -   subject detail
    -   style
    -   setting
    -   mood
    -   composition
-   Discuss how a stronger image prompt becomes much more specific and usable.

#### **Transition**

-   Say:
    -   "Text generation creates words. Image generation creates visuals. But both depend on system instructions, structure, and design choices."
-   Ask:
    -   What makes a generated image useful instead of random?
    -   Why might image generation be powerful and risky at the same time?

### 2. **Direct Instruction (Time: 55 minutes)**

-   **Objective:** Help Geniuses understand how image generation systems work and why prompt structure matters in visual AI.
-   Use slides to guide instruction and keep it interactive.

#### **Suggested Slide Flow**

-   **Slide 1: What Is an Image Generation System?**
    -   An image generation system creates new visual content from prompts, instructions, and learned visual patterns
    -   It can generate:
        -   illustrations
        -   concept art
        -   posters
        -   product mockups
        -   branding images
        -   scene concepts
        -   story visuals
-   **Slide 2: Text Generation vs Image Generation**
    -   Text generation creates language outputs
    -   Image generation creates visual outputs
    -   Both depend on prompts and learned patterns
    -   Both can be guided by structure and constraints
-   **Slide 3: Common Image Prompt Ingredients**
    -   subject
    -   style
    -   setting
    -   mood
    -   color palette
    -   perspective
    -   composition
    -   output purpose
-   **Slide 4: Image Generation Use Cases**
    -   branding
    -   advertising
    -   storyboarding
    -   concept art
    -   social media content
    -   UI mockup inspiration
    -   campaign visuals
    -   educational illustration
-   **Slide 5: Why Prompt Specificity Matters**
    -   vague prompts create vague outputs
    -   stronger prompts help the system understand:
        -   what to include
        -   what to emphasize
        -   what style to follow
        -   what feeling to create
-   **Slide 6: Prompt-to-Image Workflow**
    -   user goal
    -   prompt design
    -   generation
    -   review
    -   refine
    -   final output selection
-   **Slide 7: Risks in Image Generation**
    -   misleading visuals
    -   stereotypes
    -   bias in generated appearance
    -   unrealistic or fake imagery
    -   weak brand consistency
    -   copyright and originality concerns
-   **Slide 8: Responsible Image Generation**
    -   be clear about use case
    -   avoid harmful stereotypes
    -   review outputs carefully
    -   do not present synthetic visuals deceptively
    -   think about fairness and representation
-   **Slide 9: Visual AI in Real Products**
    -   design support tools
    -   marketing creative tools
    -   product mockup generators
    -   storytelling tools
    -   AI-assisted content platforms
-   **Slide 10: Week 2 Direction**
    -   Geniuses are moving from text generation into image generation, then toward multimodal and broader generative systems

#### **Discussion Questions**

-   What makes an image generation prompt strong?
-   Why does image generation require review even if the image looks impressive?
-   What kinds of products could use image generation well?
-   What kinds of harms could happen with careless image generation?
-   Why should builders think about trust and representation in visual AI?

#### **Reflection Prompt**

-   Have Geniuses write for 4 minutes:
    -   "Describe one real product or venture that could benefit from image generation. What kind of visual output would it need?"

### 3. **Guided Practice (Time: 50 minutes)**

-   **Objective:** Help Geniuses build a Python-based image prompt design lab that creates structured prompt templates for image generation.
-   Explain that today's code-along is about designing stronger visual AI instructions, not just typing random prompt text.
-   The class will create `image_prompt_lab.py`.

#### **Guided Practice Build**

Create a folder called `image-prompt-lab`.

#### **Project Goal**

Build a Python program that:

-   asks the user for an image goal
-   asks for subject, style, setting, and mood
-   builds a structured prompt
-   optionally sends the prompt into an OpenAI image workflow or prints it for generation and refinement

#### **Setup Steps**

1.  Open VS Code.
2.  Create a folder called `image-prompt-lab`.
3.  Open the terminal in VS Code.
4.  Install dependencies:
```
pip install openai python-dotenv
```
1.  Create a `.env` file:
```
OPENAI_API_KEY=your_key_here
```
1.  Create a file called `image_prompt_lab.py`

#### **Sample Code**
```
# image_prompt_lab.py
# AI Systems Week 2 Day 3
# This program helps Geniuses build structured prompts
# for image generation systems.

print("Welcome to the Image Prompt Lab\n")

# Collect structured image prompt details
image_goal = input("What is the purpose of the image? ")
subject = input("What is the main subject? ")
style = input("What style should it have? ")
setting = input("What is the setting or environment? ")
mood = input("What mood should the image have? ")

# Build a structured prompt
final_prompt = f"""
Create an image for this purpose: {image_goal}.
Main subject: {subject}.
Style: {style}.
Setting: {setting}.
Mood: {mood}.
The image should be clear, visually strong, and suitable for its intended purpose.
"""

print("\n--- Structured Image Prompt ---")
print(final_prompt)

print("\n--- Reflection ---")
print("What part of the prompt makes the image specific?")
print("What would you refine if the output looked too generic?")
print("What trust or review step would matter before using the image publicly?")
```
#### **Optional API Extension**

If you want the class to also connect to image generation workflow thinking, add:

# optional_prompt_writer.py
# This version uses the OpenAI API to improve an image prompt.
```
import os
from dotenv import load_dotenv
from openai import OpenAI

load_dotenv()
client = OpenAI(api_key=os.getenv("OPENAI_API_KEY"))

raw_idea = input("Enter a rough image idea: ")

prompt = f"""
You are an image prompt designer.

Take this rough image idea:
"{raw_idea}"

Turn it into a stronger image generation prompt.
Include:
- subject
- style
- setting
- mood
- useful visual detail

Return only the final improved prompt.
"""

response = client.responses.create(
    model="gpt-4.1-mini",
    input=prompt
)

print("\n--- Improved Image Prompt ---")
print(response.output_text)
```
#### **Guided Practice Teaching Points**

-   Why prompt structure matters in visual systems
-   Why image goals should connect to product or user value
-   Why design variables like mood and setting change the result
-   Why image generation often needs iteration
-   Why generated visuals should be reviewed before public use

#### **Guided Practice Discussion**

-   What made the prompt stronger?
-   Which prompt fields felt most important?
-   What kind of image outputs would still need human editing or review?
-   How could this workflow help in a real software app?

### 4. **Independent Practice (Time: 30 minutes)**

-   **Objective:** Geniuses independently create a visual AI system concept and structured prompt workflow for a real use case.
-   This continues the Week 2 mini-project.

#### **Mini-Project Title**

**Generative AI System Concept --- Day 3 Visual AI Workflow**

#### **Independent Task**

Each Genius creates a Python file for a visual generation system concept.

Examples:

-   poster image generator
-   flyer visual assistant
-   brand concept art generator
-   story scene image generator
-   social media visual generator
-   product mockup idea generator
-   mascot design assistant

Their system must include:

-   system name
-   one input idea
-   one image generation use case
-   a structured prompt workflow
-   one trust or ethics concern
-   one responsible design choice

#### **Required Deliverables**

-   A working Python file called `my_image_generator_system.py`
-   A working `.env` file if using API support
-   A system concept with:
    -   system name
    -   input type
    -   output type
    -   image use case
    -   one prompt structure improvement
    -   one risk or ethics concern
    -   one responsible design choice
-   A short written reflection:
    -   Why is image generation the right system type here?
    -   What makes the visual prompt strong?
    -   What must be reviewed before using the image seriously?

#### **Independent Practice Starter Code**
```
# my_image_generator_system.py
# Week 2 Day 3 independent practice
# This program creates a visual AI system concept.

print("My Visual AI System\n")

system_name = "FlyerForge AI"
input_type = "Event theme, audience, and visual style request"
output_type = "A structured prompt for generating a flyer image"
use_case = "Create bold visuals for youth event promotion"
prompt_improvement = "Include subject, style, setting, mood, and audience"
ethics_concern = "The system could generate misleading or stereotypical visuals"
responsible_design = "All outputs should be reviewed for fairness, accuracy, and public appropriateness"

print(f"System Name: {system_name}")
print(f"Input Type: {input_type}")
print(f"Output Type: {output_type}")
print(f"Use Case: {use_case}")
print(f"Prompt Improvement: {prompt_improvement}")
print(f"Ethics Concern: {ethics_concern}")
print(f"Responsible Design Choice: {responsible_design}")
```
#### **Facilitator Support Moves**

-   Help Geniuses choose a real visual product use case
-   Ask:
    -   What is the image for?
    -   Who is the audience?
    -   What style makes sense here?
    -   What kind of visual harm or misunderstanding could happen?
-   Encourage systems that are useful and well-bounded

### 5. **Closure (Time: 20 minutes)**

-   **Objective:** Reinforce that image generation is a structured system behavior and not just random visual creativity.
-   Bring the class together for a final share-out.
-   Ask 3--5 Geniuses to share:
    -   their system name
    -   what kind of image it helps generate
    -   one strong prompt design choice
    -   one ethics or trust concern
-   Lead a closing discussion:
    -   What makes image generation different from text generation?
    -   Why does visual prompt structure matter?
    -   What kinds of review are important in image generation systems?
-   Preview the next lesson:
    -   Geniuses will move into multimodal and mixed-input systems, including how text and image workflows connect and how broader generative software apps are designed.

**Assessment:**
---------------

Student learning will be assessed through:

-   Participation in the icebreaker and discussion
-   Reflection responses during direct instruction
-   Completion of the guided Python image prompt lab
-   Completion of an independent visual AI system concept
-   Final share-out and explanation of prompt structure and responsible design

### **Exit Ticket**

1.  What is an image generation system?
2.  What are three things a strong image prompt should include?
3.  What is one risk in image generation systems?

**Extra Activities:**
---------------------

-   Geniuses who finish early can:
    -   create multiple prompt versions for the same image goal
    -   compare minimalist vs detailed prompts
    -   add audience-based prompt changes
    -   create a brand-style visual prompt series
    -   use the API to improve prompts further
    -   build a prompt menu system
-   Add a "who is this image for?" field
-   Add a "what should be avoided?" field
-   Add a "revision prompt" section
-   Add a "public use review checklist" section

**Reflection / Takeaways:**
---------------------------

This lesson works best when Geniuses realize that image generation is both creative and technical. Day 3 helps them understand that visual AI systems depend on structured prompting, user goals, style control, and careful review. By the end of the lesson, Geniuses should feel more confident thinking about image generation as a real software system behavior and more aware that strong visual outputs require responsibility as well as creativity.

**Facilitator Notes**
---------------------

-   Keep using **Geniuses** consistently in examples and discussion.
-   Reinforce that image generation should be tied to real goals and real audiences.
-   Encourage specificity in prompts and caution in public-facing use.
-   Keep the lesson grounded in product and software thinking, not only creative experimentation.
-   Remind Geniuses that tomorrow they will explore multimodal systems and broader generative workflows.

**Week 2 Day 3 Mini-Project Connection**
----------------------------------------

By the end of Day 3, each Genius should have:

-   A named visual AI system concept
-   A real image generation use case
-   A structured image prompt workflow
-   A Python-based visual prompt lab or concept script
-   At least one identified trust or ethics concern
-   At least one responsible design choice
-   A stronger understanding of image generation as a modern AI system behavior
