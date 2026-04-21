<img src="https://github.com/Hgp-GeniusLabs/Curriculum/blob/10734f2c827128dde773ea4f266d154d46977866/Org-Wide/Assets/hgp_logo_original.png" width="150"/>

Lesson Plan: AI Systems Week 2, Day 1 --- What Is Generative AI? Creating Text, Images, and New Possibilities
===========================================================================================================

**Duration:**
-------------

3 hours

**Lesson Overview:**
--------------------

Week 2 introduces Geniuses to **Generative AI Systems**. After spending Week 1 learning how AI systems classify, rank, recommend, and learn from data, Geniuses now begin exploring a different kind of system behavior: **generation**. Instead of deciding what category something belongs to, generative systems create something new such as text, images, ideas, summaries, plans, and other outputs based on patterns learned from large amounts of data.

This lesson introduces the technical and creative foundations of generative AI. Geniuses explore how generative systems differ from classification systems, what kinds of inputs and outputs they use, and why these systems are powerful in modern software, media, and business. They also begin thinking critically about the risks of generative systems including hallucinations, misinformation, bias, originality, and trust. During guided practice, the class builds a simple Python OpenAI-powered text generator in VS Code and compares it to a classifier-style system. During independent practice, each Genius creates the first version of a generative AI system concept tied to a real use case. By the end of the lesson, Geniuses should understand that generative AI is not just about making cool outputs. It is about designing systems that create in structured, useful, and responsible ways.

**Objectives:**
---------------

-   Define generative AI and explain how it differs from classification systems.
-   Identify common types of generative outputs such as text, images, audio, and video.
-   Explain how generative systems take in prompts or inputs and produce new outputs.
-   Analyze real-world examples of generative AI products and workflows.
-   Build a simple Python-based OpenAI text generation tool in VS Code.
-   Reflect on the strengths, risks, and responsible design challenges of generative AI systems.
-   Begin the Week 2 mini-project by designing a generative AI software concept.

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
-   Optional examples of generative AI tools or products

**Standards:**
--------------

-   Computational Thinking: Distinguish between different AI system behaviors such as classification and generation.
-   Computer Science Practices: Build and test a simple generative AI workflow using structured prompts.
-   Programming: Use Python and the OpenAI API to create a basic generative AI tool.
-   Digital Literacy: Evaluate the usefulness, limitations, and risks of generated content.
-   Career Readiness: Practice technical reasoning, experimentation, and responsible systems design.
-   Technical Foundations: Explain how generative systems create outputs from prompts and learned patterns.

**Lesson Activity:**
--------------------

### 1. **Introduction (Time: 25 minutes)**

-   **Objective:** Energize Geniuses and introduce the idea that some AI systems are built to create rather than only classify or sort.
-   Start with a fun icebreaker called **"Classify It or Generate It?"**
-   This should be the first thing and the most fun thing to wake Geniuses up and get them ready for the lesson.

#### **Icebreaker Option A: Physical Movement**

-   Label one side of the room **"Classification"** and the other side **"Generation."**
-   Read examples aloud and have Geniuses move to the side they think fits best.
-   Example prompts:
    -   Label an email as spam or not spam
    -   Write a short thank-you email
    -   Identify whether an image contains a dog
    -   Create a poster image from a prompt
    -   Classify a review as positive or negative
    -   Generate a study guide from class notes
    -   Detect whether a photo contains a stop sign
    -   Create three slogan ideas for a business
-   After each round, ask:
    -   Why is this classification or generation?
    -   What is the system taking in?
    -   What is it giving back?
    -   Which feels more open-ended?
    -   Which feels riskier if the output is wrong?

#### **Icebreaker Option B: Product Sort**

-   Put real-world product examples on the board.
-   Ask Geniuses to sort them into:
    -   mainly classification
    -   mainly generation
    -   mixed system
-   Examples:
    -   spam filter
    -   AI image generator
    -   AI note summarizer
    -   object detector
    -   AI chatbot
    -   content moderation system
-   Discuss how some modern tools combine multiple AI system types.

#### **Transition**

-   Say:
    -   "Last week, Geniuses learned about systems that identify, sort, and rank. This week begins with systems that create."
-   Ask:
    -   What makes generated content different from predicted categories?
    -   Why are generative systems exciting and risky at the same time?

### 2. **Direct Instruction (Time: 55 minutes)**

-   **Objective:** Help Geniuses understand what generative AI is, how it works at a high level, and why it matters in modern AI systems.
-   Use slides to guide instruction and keep it interactive.

#### **Suggested Slide Flow**

-   **Slide 1: What Is Generative AI?**
    -   Generative AI systems create new outputs based on patterns learned from data
    -   Outputs may include:
        -   text
        -   images
        -   music
        -   code
        -   video
        -   ideas
        -   structured content
-   **Slide 2: Generation vs Classification**
    -   **Classification:** decide what something is
    -   **Generation:** create what could come next
    -   Classification often chooses from existing categories
    -   Generation creates new content from patterns
-   **Slide 3: Common Generative Inputs**
    -   prompt text
    -   example content
    -   style instructions
    -   image or audio references
    -   structured constraints
    -   user goals
-   **Slide 4: Common Generative Outputs**
    -   paragraphs
    -   summaries
    -   stories
    -   messages
    -   images
    -   rewritten text
    -   plans
    -   captions
    -   creative variations
-   **Slide 5: Real-World Generative Systems**
    -   writing assistants
    -   image generators
    -   AI slide builders
    -   summarization systems
    -   brainstorming tools
    -   code assistants
    -   multimodal creative apps
-   **Slide 6: What Makes Generative AI Powerful**
    -   flexibility
    -   speed
    -   creativity support
    -   personalization
    -   content transformation
    -   idea expansion
-   **Slide 7: What Makes Generative AI Risky**
    -   hallucinations
    -   false information
    -   biased output
    -   harmful content
    -   overconfidence
    -   synthetic media misuse
    -   unclear originality
-   **Slide 8: Responsible Generative AI Design**
    -   make the task clear
    -   constrain the output
    -   communicate limits
    -   avoid pretending certainty
    -   add review for important use cases
    -   think about who could be affected
-   **Slide 9: Prompting as System Design**
    -   prompts are not magic words
    -   prompts are system instructions
    -   stronger prompts help define:
        -   role
        -   task
        -   format
        -   tone
        -   boundaries
-   **Slide 10: Week 2 Direction**
    -   Geniuses will explore text generation, image generation, multimodal systems, and responsible generative AI software concepts

#### **Discussion Questions**

-   What makes generation different from simple classification?
-   Why do generative systems need strong prompts or instructions?
-   What is exciting about generative systems?
-   What is risky about them?
-   What kinds of apps should use more caution when generating content?

#### **Reflection Prompt**

-   Have Geniuses write for 4 minutes:
    -   "Think of one real-world problem that could be helped by a generative AI system. What would the system create, and why would that be useful?"

### 3. **Guided Practice (Time: 50 minutes)**

-   **Objective:** Help Geniuses build their first simple text generation tool using Python and the OpenAI API.
-   Explain that today's code-along introduces the API as a generative system component.
-   The class will create `text_generator_lab.py`.

#### **Guided Practice Build**

Create a folder called `text-generator-lab`.

#### **Project Goal**

Build a Python program that:

-   asks the user for a topic or task
-   sends the request to the OpenAI API
-   generates a short structured output
-   helps Geniuses see how a generative system works

#### **Setup Steps**

1.  Open VS Code.
2.  Create a folder called `text-generator-lab`.
3.  Open the terminal in VS Code.
4.  Install dependencies:
```
pip install openai python-dotenv
```
1.  Create a `.env` file:
```
OPENAI_API_KEY=your_key_here
```
1.  Create a file called `text_generator_lab.py`

#### **Sample Code**
```
# text_generator_lab.py
# AI Systems Week 2 Day 1
# This program uses the OpenAI API to generate a short structured response.

import os
from dotenv import load_dotenv
from openai import OpenAI

# Load environment variables
load_dotenv()

# Create the OpenAI client
client = OpenAI(api_key=os.getenv("OPENAI_API_KEY"))

print("Welcome to the Text Generator Lab\n")

# Ask the Genius for a prompt topic
topic = input("What topic should the system generate on? ")

prompt = f"""
You are a helpful generative AI system.

Generate a short response about this topic:
"{topic}"

Return your answer in this format:
Title: <short title>
Response: <3 to 4 sentence response>
"""

response = client.responses.create(
    model="gpt-4.1-mini",
    input=prompt
)

print("\n--- Generated Output ---")
print(response.output_text)

print("\n--- Reflection ---")
print("What kind of input did this system take?")
print("What kind of output did it create?")
print("How is this different from a classifier?")
```
#### **Guided Practice Teaching Points**

-   Why the model is being asked to generate instead of classify
-   Why the prompt sets the task, format, and boundaries
-   Why structured output makes generation easier to use in real software
-   Why this is still a system, not just a chatbot moment
-   Why generated outputs should still be reviewed in real-world use

#### **Guided Practice Discussion**

-   What makes this output generative?
-   How did the prompt shape the result?
-   What would happen if the prompt were much more vague?
-   Why is structure helpful in generated outputs?

### 4. **Independent Practice (Time: 30 minutes)**

-   **Objective:** Geniuses independently create a first generative AI system concept and a small API-powered prototype.
-   This begins the Week 2 mini-project.

#### **Mini-Project Title**

**Generative AI System Concept --- Day 1 Foundation**

#### **Independent Task**

Each Genius creates a Python file that uses the OpenAI API to perform one small generative task tied to a real use case.

Examples:

-   generate a study guide
-   generate slogan ideas
-   generate a short story prompt
-   generate a thank-you message
-   generate a task plan
-   generate social media caption ideas
-   generate a summary from a topic prompt

Their mini-tool must include:

-   system name
-   one input
-   one generative output
-   one use case
-   one risk or trust concern
-   one responsible design choice

#### **Required Deliverables**

-   A working Python file called `my_generative_system.py`
-   A working `.env` file configured locally
-   A system concept with:
    -   system name
    -   input type
    -   output type
    -   use case
    -   one risk
    -   one responsible design choice
-   A short written reflection:
    -   Why is this a generative AI system?
    -   What makes this output useful?
    -   What would a user still need to double-check?

#### **Independent Practice Starter Code**
```
# my_generative_system.py
# Week 2 Day 1 independent practice
# This program creates a small generative AI system.

import os
from dotenv import load_dotenv
from openai import OpenAI

load_dotenv()
client = OpenAI(api_key=os.getenv("OPENAI_API_KEY"))

system_name = "StudySpark AI"
user_input = input("Enter a school topic: ")

prompt = f"""
You are a study support generator.

Create:
1. A short study topic title
2. Three key points to review\
3. One helpful next step

Topic:
"{user_input}"
"""

response = client.responses.create(
    model="gpt-4.1-mini",
    input=prompt
)

print(f"\nSystem Name: {system_name}")
print("\n--- Generated Study Output ---")
print(response.output_text)

print("\nTrust Note: This generated study support should be reviewed for accuracy before being used for important assignments or tests.")
```
#### **Facilitator Support Moves**

-   Help Geniuses choose a clear generative use case
-   Ask:
    -   What is the system creating?
    -   Why is generation useful here?
    -   What kind of prompt will make the output stronger?
    -   What could go wrong if the system generates bad content?
-   Encourage narrow and useful tasks instead of vague "do anything" tools

### 5. **Closure (Time: 20 minutes)**

-   **Objective:** Reinforce that generative AI systems create useful outputs, but they still require structure, caution, and responsible design.
-   Bring the class together for a final share-out.
-   Ask 3--5 Geniuses to share:
    -   their system name
    -   what it generates
    -   one use case
    -   one risk or trust concern
-   Lead a closing discussion:
    -   What makes generative AI different from classification systems?
    -   Why are prompts part of system design?
    -   Why should generated content still be reviewed?
-   Preview the next lesson:
    -   Geniuses will go deeper into text generation systems, prompt quality, and how better prompting changes the quality, structure, and usefulness of output.

**Assessment:**
---------------

Student learning will be assessed through:

-   Participation in the icebreaker and discussion
-   Reflection responses during direct instruction
-   Completion of the guided Python text generation lab
-   Completion of an independent generative AI mini-tool
-   Final share-out and explanation of generative use cases and risks

### **Exit Ticket**

1.  What is generative AI?
2.  How is generation different from classification?
3.  What is one risk in generative AI systems?

**Extra Activities:**
---------------------

-   Geniuses who finish early can:
    -   try multiple prompts and compare outputs
    -   add stronger formatting instructions
    -   generate multiple versions of the same response
    -   create a system that rewrites tone in different styles
    -   add a "needs review" warning for important use cases
    -   test how vague prompts change output quality
-   Add a category explaining whether the use case is low-risk or high-risk
-   Add a second generative mode to the same file
-   Add a prompt template users can reuse
-   Add a short comparison section between generation and classification

**Reflection / Takeaways:**
---------------------------

This lesson works best when Geniuses realize that generative AI systems are different from many of the systems they studied in Week 1. Instead of identifying what something is, they create what could come next. Day 1 of Week 2 introduces that shift while keeping the lesson technical, grounded, and responsible. By the end of the lesson, Geniuses should feel excited about what generative AI can do, while also understanding that useful generation depends on structure, prompting, and careful review.

**Facilitator Notes**
---------------------

-   Keep using **Geniuses** consistently in examples and discussion.
-   Reinforce that generative AI is powerful, but not automatically trustworthy.
-   Keep prompts structured so students see good systems habits early.
-   Encourage useful, bounded tasks over vague "chatbot" thinking.
-   Remind Geniuses that tomorrow they will go deeper into text generation, prompt engineering, and output quality.

**Week 2 Day 1 Mini-Project Connection**
----------------------------------------

By the end of Day 1, each Genius should have:

-   A named generative AI system concept
-   A clearly defined input and output
-   A real use case for what the system generates
-   A first OpenAI-powered generative mini-tool
-   At least one identified risk
-   At least one responsible design choice
-   A stronger understanding of how generative systems differ from classifiers and other AI system types
