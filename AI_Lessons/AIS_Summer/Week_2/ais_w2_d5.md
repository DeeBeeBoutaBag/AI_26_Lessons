<img src="https://github.com/Hgp-GeniusLabs/Curriculum/blob/10734f2c827128dde773ea4f266d154d46977866/Org-Wide/Assets/hgp_logo_original.png" width="150"/>

Lesson Plan: AI Systems Week 2, Day 5 --- Generative AI Studio, Responsible Creation, and Software Concept Showcase
=================================================================================================================

**Duration:**
-------------

3 hours

**Lesson Overview:**
--------------------

Day 5 brings together everything Geniuses explored in Week 2: what generative AI is, how text generation works, how image generation systems use structured prompts, and how multimodal systems combine different forms of input and output. The focus of today is refinement, critique, and showcase. Geniuses use studio-style work time to strengthen a **generative AI software concept** that could become part of a larger final project later in the course.

The lesson emphasizes that strong generative AI systems are not just creative. They are purposeful, structured, and responsible. Geniuses will refine their software concept so it clearly explains what is generated, why generation is the right system behavior, who the product is for, what trust issues exist, and how the system should be used responsibly. During guided practice, the class builds a more polished generative system summary tool in Python that combines product thinking, prompt design, and responsible AI reflection. During independent practice, each Genius finalizes a generative AI software concept and prepares a short showcase. By the end of the lesson, Geniuses should feel that they are not just experimenting with generation. They are learning how to design useful and trustworthy generative systems.

**Objectives:**
---------------

-   Synthesize key ideas from Week 2 on text, image, and multimodal generative AI systems.
-   Refine a generative AI software concept so it is technically clearer and more product-ready.
-   Explain why generation is the correct AI behavior for a chosen use case.
-   Identify trust, ethics, and review needs in a generative AI product.
-   Build a Python-based concept summarizer for a generative AI software system.
-   Present a generative AI system concept clearly in terms of inputs, outputs, value, and responsibility.
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
-   Existing Week 2 files and concept work
-   `.env` setup instructions for API keys

**Standards:**
--------------

-   Computational Thinking: Connect system behavior, inputs, outputs, and user goals into a coherent software concept.
-   Computer Science Practices: Build and refine a generative AI workflow with clearer structure and purpose.
-   Programming: Use Python and the OpenAI API to support structured system design and output organization.
-   Digital Literacy: Evaluate the usefulness, trustworthiness, and risks of generative AI products.
-   Career Readiness: Practice technical communication, critique, and presentation.
-   Technical Foundations: Explain the role of generation in modern AI software systems.

**Lesson Activity:**
--------------------

### 1. **Introduction (Time: 20 minutes)**

-   **Objective:** Energize Geniuses and frame the day around refining generative AI concepts into stronger software ideas.
-   Start with a fun icebreaker called **"Cool Generation or Useful Generation?"**
-   This should be the first thing and the most fun thing to wake Geniuses up and get them ready for the lesson.

#### **Icebreaker Option A: Physical Movement**

-   Label one side of the room **"Cool"** and the other side **"Useful."**
-   Read generative AI ideas aloud and have Geniuses move to the side that best matches how the idea feels.
-   Example prompts:
    -   A tool that generates random fantasy creature names
    -   A tool that generates study guides from class topics
    -   A tool that creates flashy abstract wallpapers
    -   A tool that generates flyer concepts for community events
    -   A tool that writes fake celebrity drama posts
    -   A tool that generates next-step plans for internship prep
    -   A tool that creates brand moodboards for youth businesses
-   After each round, ask:
    -   What makes this mostly cool or actually useful?
    -   Who would use it?
    -   What problem does it solve?
    -   Could it become a real software product?

#### **Icebreaker Option B: Product Filter**

-   Put generative app ideas on the board.
-   Ask Geniuses to sort them into:
    -   interesting but weak
    -   useful and realistic
    -   powerful but needs strong guardrails
-   Discuss how product value and responsibility matter as much as creative output.

#### **Transition**

-   Say:
    -   "This week was not about generation for generation's sake. It was about understanding when creative AI becomes a real system that helps someone."
-   Ask:
    -   What makes a generative system worth building?
    -   What makes a generative system trustworthy enough to use?

### 2. **Direct Instruction (Time: 40 minutes)**

-   **Objective:** Help Geniuses review the core ideas from the week and prepare to refine and present their software concepts.
-   Use slides to guide instruction and keep it interactive.

#### **Suggested Slide Flow**

-   **Slide 1: Week 2 Wrap-Up --- AI Systems That Create**
    -   This week focused on systems that generate text, images, and multimodal outputs
    -   Geniuses moved from identifying systems to building creative system workflows
-   **Slide 2: What Makes a Generative AI Software Concept Strong?**
    -   clear user
    -   clear problem
    -   clear generated output
    -   clear reason generation is useful
    -   clear trust and review thinking
-   **Slide 3: Weak Generative Concepts**
    -   vague purpose
    -   no real user
    -   generation added just because it seems impressive
    -   no responsible design thinking
    -   no structure in the output
-   **Slide 4: Strong Generative Concepts**
    -   useful output
    -   product clarity
    -   clear workflow
    -   bounded prompts
    -   review or trust features
    -   realistic audience and value
-   **Slide 5: Week 2 System Types Reviewed**
    -   text generation
    -   image generation
    -   multimodal generation
    -   prompt-driven workflows
    -   structured outputs
-   **Slide 6: What Makes Generation the Right Choice?**
    -   when the product needs new content
    -   when the system is helping draft, design, transform, or create
    -   when rigid categories would not be enough
-   **Slide 7: Trust and Guardrails in Generation**
    -   review before publishing
    -   avoid deception
    -   avoid harmful or misleading content
    -   use clear boundaries
    -   explain limitations
-   **Slide 8: Product Questions Builders Should Answer**
    -   What does the system generate?
    -   Why would a user want that?
    -   What input does the system need?
    -   What output format is most useful?
    -   What should users still double-check?
-   **Slide 9: Showcase Thinking**
    -   Can you clearly explain:
        -   the product name?
        -   the user?
        -   the input?
        -   the generated output?
        -   the trust concern?
        -   the responsible design choice?
-   **Slide 10: Looking Ahead**
    -   Week 3 will move into more technical AI systems areas beyond pure generation
    -   The ideas from this week can still feed into larger final project directions

#### **Discussion Questions**

-   What makes a generative AI product useful instead of just flashy?
-   Why does a clear user matter?
-   What trust issue matters most in generative systems?
-   How do you know when generation is the right AI behavior?
-   What makes a generative app concept feel real?

#### **Reflection Prompt**

-   Have Geniuses write for 4 minutes:
    -   "What is the strongest part of your generative AI system concept right now, and what still needs improvement?"

### 3. **Guided Practice (Time: 45 minutes)**

-   **Objective:** Help Geniuses build a Python-based concept summarizer that organizes a generative AI software idea clearly.
-   Explain that today's code-along is about communicating a system idea with technical and responsible clarity.
-   The class will create `generative_system_summary.py`.

#### **Guided Practice Build**

Create a folder called `generative-system-summary`.

#### **Project Goal**

Build a Python program that:

-   asks the user key questions about a generative software concept
-   organizes the answers into a structured summary
-   optionally uses the OpenAI API to polish the summary

#### **Setup Steps**

1.  Open VS Code.
2.  Create a folder called `generative-system-summary`.
3.  Create a file called `generative_system_summary.py`.
4.  If using the API polish feature, install dependencies:
```
pip install openai python-dotenv
```
1.  Create a `.env` file if needed:
```
OPENAI_API_KEY=your_key_here
```
#### **Sample Code**
```
# generative_system_summary.py
# AI Systems Week 2 Day 5
# This program helps Geniuses summarize a generative AI software concept.

print("Welcome to the Generative System Summary Tool\n")

system_name = input("What is the name of your generative AI system? ")
user = input("Who is the system for? ")
input_type = input("What input does the system take? ")
output_type = input("What does the system generate? ")
use_case = input("What real task or problem does it help with? ")
trust_concern = input("What is one trust or ethics concern? ")
responsible_design = input("What is one responsible design choice? ")

print("\n--- Generative AI Software Summary ---")
print(f"System Name: {system_name}")
print(f"User: {user}")
print(f"Input Type: {input_type}")
print(f"Generated Output: {output_type}")
print(f"Use Case: {use_case}")
print(f"Trust Concern: {trust_concern}")
print(f"Responsible Design Choice: {responsible_design}")

print("\n--- Reflection ---")
print("Why is generation the right AI behavior for this product?")
print("What should the user still review before trusting the output?")
```
#### **Optional API Polish Version**
```
# optional_summary_polisher.py
# This program uses the OpenAI API to polish a system summary.

import os
from dotenv import load_dotenv
from openai import OpenAI

load_dotenv()
client = OpenAI(api_key=os.getenv("OPENAI_API_KEY"))

raw_summary = input("Paste your rough generative AI system summary: ")

prompt = f"""
You are a technical AI systems writing assistant.

Take this rough generative AI software summary:
"{raw_summary}"

Rewrite it so it is:
- clearer
- more structured
- more professional
- still easy for a high school Genius to understand

Return labeled sections for:
1. System Name
2. User
3. Input
4. Output
5. Use Case
6. Trust Concern
7. Responsible Design Choice
"""

response = client.responses.create(
    model="gpt-4.1-mini",
    input=prompt
)

print("\n--- Polished Summary ---")
print(response.output_text)
```
#### **Guided Practice Teaching Points**

-   Why system concepts need clear technical structure
-   Why product communication matters in technical AI work
-   Why trust concerns should be named directly
-   Why summary tools help Geniuses think more clearly about what they are building
-   Why a strong concept is a bridge between experimentation and real software design

#### **Guided Practice Discussion**

-   What section of the summary feels most important?
-   What makes a use case feel real?
-   Why should responsible design be included in the summary, not added later?
-   How would this summary help someone else understand the product quickly?

### 4. **Independent Practice (Time: 45 minutes)**

-   **Objective:** Geniuses independently refine a generative AI software concept and prepare for a short showcase.
-   This completes the Week 2 mini-project.

#### **Mini-Project Title**

**Week 2 Generative AI Software Concept --- Showcase Build**

#### **Independent Task**

Each Genius finalizes a generative AI software concept that uses one or more of the following:

-   text generation
-   image generation
-   multimodal generation

Their concept must clearly explain:

-   system name
-   user
-   input
-   output
-   use case
-   why generation is the correct AI behavior
-   one trust or ethics concern
-   one responsible design choice

They may use Python to print the summary or use the API to polish it.

#### **Required Deliverables**

-   A working Python file called `week2_generative_system_showcase.py`
-   A working `.env` file if using the API
-   A complete generative system concept with:
    -   system name
    -   user
    -   input
    -   output
    -   use case
    -   one trust concern
    -   one responsible design choice
    -   one explanation of why generation fits
-   A short written reflection:
    -   What kind of generative AI system is this?
    -   Why would a user want it?
    -   What part of the output should never be trusted blindly?

#### **Independent Practice Starter Code**
```
# week2_generative_system_showcase.py
# Week 2 independent practice
# This program prints a refined generative AI software concept.

print("Week 2 Generative AI Software Concept\n")

system_name = "PosterPulse AI"
user = "Youth organizers and student leaders"
input_type = "Event theme, audience, visual tone, and key message"
output_type = "Poster concept text and structured image prompt"
use_case = "Help users generate stronger promotional visuals for events"
why_generation = "The system needs to create new visual and textual content, not just classify existing information"
trust_concern = "The output could be visually misleading or not match the intended audience well"
responsible_design = "The system should require user review before any public use and should avoid harmful or stereotypical imagery"

print(f"System Name: {system_name}")
print(f"User: {user}")
print(f"Input Type: {input_type}")
print(f"Generated Output: {output_type}")
print(f"Use Case: {use_case}")
print(f"Why Generation Fits: {why_generation}")
print(f"Trust Concern: {trust_concern}")
print(f"Responsible Design Choice: {responsible_design}")
```
#### **Facilitator Support Moves**

-   Help Geniuses focus on clarity and usefulness
-   Ask:
    -   What does the system really generate?
    -   Why is that useful to the user?
    -   What makes it more than a random content toy?
    -   What is the most important trust issue?
-   Encourage software concepts that feel modern, bounded, and real

### 5. **Closure (Time: 30 minutes)**

-   **Objective:** Celebrate the week's learning and reinforce that generative AI systems can be creative, useful, and responsibly designed.
-   Bring the class together for a Week 2 showcase.
-   Ask 5--7 Geniuses to share:
    -   their system name
    -   what it generates
    -   who it is for
    -   one trust concern
    -   one responsible design choice
-   Lead a closing discussion:
    -   What did you learn this week about generative AI systems?
    -   What is the difference between text, image, and multimodal generation?
    -   What makes a generative AI software concept feel real and useful?
    -   Why is trust still central in systems that create?
-   Preview the next lesson:
    -   Week 3 will move into the next major AI Systems theme and build on the idea that modern AI products often combine multiple technical behaviors, not just one.

**Assessment:**
---------------

Student learning will be assessed through:

-   Participation in the icebreaker and discussion
-   Reflection responses during direct instruction
-   Completion of the guided concept summary tool
-   Completion of a full Week 2 generative AI software concept
-   Final showcase and explanation of technical and responsible design choices

### **Exit Ticket**

1.  What is one kind of generative AI system you explored this week?
2.  Why is generation the right AI behavior for your concept?
3.  What is one trust issue that must be considered in generative AI systems?

**Extra Activities:**
---------------------

-   Geniuses who finish early can:
    -   add a second version of their concept with a different user
    -   add a public-use review checklist
    -   create multiple output modes for the same system
    -   connect text and image workflows together
    -   polish their summary using the API
    -   turn the concept into a simple venture-style pitch
-   Add a "what this system should never generate" section
-   Add a "review before publish" section
-   Add a "future features" section
-   Add a "why now" section

**Reflection / Takeaways:**
---------------------------

This lesson works best when Geniuses realize that generative AI is not only about creativity. It is about system behavior, user value, technical structure, and responsibility. Day 5 helps bring Week 2 together by moving from separate labs into a clearer software concept that someone else could understand, critique, and build further. By the end of the week, Geniuses should feel more confident explaining what generative AI systems do, how they are designed, and why they need strong boundaries and thoughtful use.

**Facilitator Notes**
---------------------

-   Keep using **Geniuses** consistently in examples and discussion.
-   Reinforce that strong generative systems solve real problems for real users.
-   Encourage concepts that are useful, not only visually or creatively impressive.
-   Help Geniuses speak clearly about trust, review, and responsibility.
-   Use the showcase to see who is beginning to think like a real AI systems builder.

**Week 2 Wrap-Up**
------------------

By the end of Week 2, each Genius should have:

-   A named generative AI system concept
-   Experience with text generation workflows
-   Experience with image generation prompt structure
-   A multimodal system idea or workflow
-   At least one OpenAI-powered generative prototype
-   At least one identified trust or ethics concern
-   At least one responsible design choice
-   A clearer sense of how generative AI can become real software
