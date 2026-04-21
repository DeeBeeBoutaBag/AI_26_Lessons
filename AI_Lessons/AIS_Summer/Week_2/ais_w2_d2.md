<img src="https://github.com/Hgp-GeniusLabs/Curriculum/blob/10734f2c827128dde773ea4f266d154d46977866/Org-Wide/Assets/hgp_logo_original.png" width="150"/>

Lesson Plan: AI Systems Week 2, Day 2 --- Text Generation Systems, Prompt Design, and Output Quality
==================================================================================================

**Duration:**
-------------

3 hours

**Lesson Overview:**
--------------------

On Day 2, Geniuses go deeper into **text generation systems**. After being introduced to generative AI on Day 1, Geniuses now focus on how text generation systems work in practice and why prompt design, structure, and constraints shape output quality. The lesson emphasizes that text generation is not just about asking for words. It is about designing a system that can create useful, clear, relevant, and trustworthy outputs for a specific purpose.

Geniuses explore how text generation systems are used in modern apps for summarization, rewriting, drafting, brainstorming, support, explanation, and structured content creation. They compare weak prompts to strong prompts and learn that prompting is a form of system design. During guided practice, the class builds a Python-based text generation lab that compares prompt quality and returns more structured responses. During independent practice, each Genius builds a small text generation tool for a real use case and improves it through prompt iteration. By the end of the lesson, Geniuses should understand that better prompting leads to better AI system behavior.

**Objectives:**
---------------

-   Explain how text generation systems create outputs from prompts and instructions.
-   Identify common use cases for text generation such as summarization, drafting, rewriting, and structured writing.
-   Distinguish between weak prompts and strong prompts.
-   Explain why prompt design is part of technical system design.
-   Build a Python-based OpenAI text generation tool with structured output.
-   Compare different prompt styles and evaluate output quality.
-   Continue the Week 2 mini-project by improving a generative AI system through better prompt design.

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
-   Existing Week 2 Day 1 files
-   `.env` setup instructions for API keys

**Standards:**
--------------

-   Computational Thinking: Analyze how system instructions shape output quality and usefulness.
-   Computer Science Practices: Build and test prompt-driven text generation workflows.
-   Programming: Use Python and the OpenAI API to create structured text generation tools.
-   Digital Literacy: Evaluate the quality, risks, and usefulness of generated text.
-   Career Readiness: Practice technical experimentation, iteration, and output critique.
-   Technical Foundations: Explain text generation as a system behavior influenced by input quality and design choices.

**Lesson Activity:**
--------------------

### 1. **Introduction (Time: 25 minutes)**

-   **Objective:** Energize Geniuses and introduce the idea that not all prompts produce equally strong outputs.
-   Start with a fun icebreaker called **"Weak Prompt or Strong Prompt?"**
-   This should be the first thing and the most fun thing to wake Geniuses up and get them ready for the lesson.

#### **Icebreaker Option A: Physical Movement**

-   Label one side of the room **"Weak Prompt"** and the other side **"Strong Prompt."**
-   Read pairs of prompt examples aloud and have Geniuses move to the side that represents the stronger one.
-   Example pairs:
    -   "Help with homework"
    -   "Create a 5-point study guide for a biology quiz on cell division using simple language"
-   More examples:
    -   "Write something about leadership"
    -   "Write a short motivational paragraph about leadership for high school Geniuses preparing for interviews"
    -   "Summarize this"
    -   "Summarize this article in 3 bullet points and include one key takeaway"
-   After each round, ask:
    -   What made one prompt stronger?
    -   What details improved the output?
    -   What part gave the system more direction?
    -   Could too little instruction make the system less useful?

#### **Icebreaker Option B: Prompt Critique**

-   Show several prompts on the board.
-   Ask Geniuses to quickly identify:
    -   which prompt is the clearest
    -   which prompt is the vaguest
    -   which one would probably produce the most useful output
-   Discuss why prompt design matters.

#### **Transition**

-   Say:
    -   "A generative model can only work with the instructions it receives. Better prompting is not magic. It is better system design."
-   Ask:
    -   What information should a text generation system know before it writes?
    -   Why would output quality change so much based on prompt wording?

### 2. **Direct Instruction (Time: 55 minutes)**

-   **Objective:** Help Geniuses understand how text generation systems work and why prompt structure changes output quality.
-   Use slides to guide instruction and keep it interactive.

#### **Suggested Slide Flow**

-   **Slide 1: What Is a Text Generation System?**
    -   A text generation system takes in a prompt or instruction and creates new text as output
    -   It can write, rewrite, summarize, brainstorm, explain, and organize
-   **Slide 2: Common Text Generation Tasks**
    -   summarization
    -   rewriting
    -   brainstorming
    -   explanations
    -   outlines
    -   captions
    -   structured responses
    -   first drafts
-   **Slide 3: Prompting Is System Design**
    -   Prompts shape:
        -   task
        -   tone
        -   structure
        -   length
        -   audience
        -   boundaries
-   **Slide 4: Weak Prompt vs Strong Prompt**
    -   Weak prompts are vague, broad, or missing important details
    -   Strong prompts define:
        -   role
        -   task
        -   audience
        -   format
        -   constraints
        -   tone
-   **Slide 5: Strong Prompt Ingredients**
    -   What the system is
    -   What the system should do
    -   Who the output is for
    -   What format to use
    -   What boundaries to respect
    -   What the output should include
-   **Slide 6: Structured Output Matters**
    -   headings
    -   bullet points
    -   steps
    -   labeled sections
    -   JSON or fixed formats
    -   Why structure makes text generation easier to use inside real software
-   **Slide 7: Real-World Text Generation Products**
    -   study guide tools
    -   AI writing assistants
    -   business message generators
    -   customer support draft tools
    -   note summarizers
    -   brainstorming apps
-   **Slide 8: Risks in Text Generation**
    -   false information
    -   vague or generic writing
    -   overconfidence
    -   tone mismatch
    -   harmful or biased outputs
    -   weak formatting
-   **Slide 9: Responsible Text Generation**
    -   be clear about the task
    -   constrain the output
    -   avoid pretending certainty
    -   use review when the stakes are high
    -   give structure when users need clear results
-   **Slide 10: Week 2 Direction**
    -   Geniuses will move from text generation into image generation and multimodal systems later this week

#### **Discussion Questions**

-   Why does prompt quality matter so much in text generation?
-   What makes a generated output useful instead of generic?
-   Why might a structured response be better than one paragraph?
-   What kinds of text generation tasks should be reviewed by humans?
-   Why is prompt engineering really a systems skill?

#### **Reflection Prompt**

-   Have Geniuses write for 4 minutes:
    -   "Think of a text generation tool you would actually use. What should the system know before it writes?"

### 3. **Guided Practice (Time: 50 minutes)**

-   **Objective:** Help Geniuses build a Python-based text generation lab that compares weak prompts and strong prompts.
-   Explain that today's code-along is about improving output through better instructions.
-   The class will create `prompt_quality_lab.py`.

#### **Guided Practice Build**

Create a folder called `prompt-quality-lab`.

#### **Project Goal**

Build a Python program that:

-   asks the user for a topic
-   sends a weak prompt to the model
-   sends a strong prompt to the model
-   prints both outputs for comparison

#### **Setup Steps**

1.  Open VS Code.
2.  Create a folder called `prompt-quality-lab`.
3.  Open the terminal in VS Code.
4.  Install dependencies:
```
pip install openai python-dotenv
```
1.  Create a `.env` file:
```
OPENAI_API_KEY=your_key_here
```
1.  Create a file called `prompt_quality_lab.py`

#### **Sample Code**
```
# prompt_quality_lab.py
# AI Systems Week 2 Day 2
# This program compares weak prompting and strong prompting
# in a text generation system.

import os
from dotenv import load_dotenv
from openai import OpenAI

# Load environment variables
load_dotenv()

# Create OpenAI client
client = OpenAI(api_key=os.getenv("OPENAI_API_KEY"))

print("Welcome to the Prompt Quality Lab\n")

topic = input("Enter a topic for text generation: ")

# Weak prompt
weak_prompt = f"""
Write something about {topic}.
"""

# Strong prompt
strong_prompt = f"""
You are a helpful writing assistant.

Create a short response about this topic:
"{topic}"

Requirements:
- Write for high school Geniuses
- Use clear and engaging language
- Include a short title
- Include 3 bullet points
- End with 1 encouraging takeaway sentence
"""

# Run weak prompt
weak_response = client.responses.create(
    model="gpt-4.1-mini",
    input=weak_prompt
)

# Run strong prompt
strong_response = client.responses.create(
    model="gpt-4.1-mini",
    input=strong_prompt
)

# Print results
print("\n--- Weak Prompt Output ---")
print(weak_response.output_text)

print("\n--- Strong Prompt Output ---")
print(strong_response.output_text)

print("\n--- Reflection ---")
print("Which output was clearer?")
print("Which one was easier to use in a real product?")
print("What did the stronger prompt add?")
```
#### **Guided Practice Teaching Points**

-   Why vague prompts lead to vague output
-   Why strong prompts make outputs more usable
-   Why formatting instructions improve system usefulness
-   Why a writing tool still needs constraints
-   Why comparing outputs is a real engineering habit

#### **Guided Practice Discussion**

-   Which output was more helpful?
-   What did the stronger prompt do better?
-   What would make the output even more useful?
-   Why might a real app use prompt templates instead of fully open-ended prompting?

### 4. **Independent Practice (Time: 30 minutes)**

-   **Objective:** Geniuses independently build a small text generation tool for a real use case and improve it through prompt design.
-   This continues the Week 2 mini-project.

#### **Mini-Project Title**

**Generative AI System Concept --- Day 2 Text Generation Tool**

#### **Independent Task**

Each Genius creates a Python file that uses the OpenAI API for one text generation use case.

Examples:

-   study guide generator
-   email draft helper
-   summary generator
-   brainstorming tool
-   caption generator
-   interview answer helper
-   action plan generator

Their tool must include:

-   system name
-   one input
-   one text generation task
-   structured output
-   one prompt improvement
-   one trust or review note

#### **Required Deliverables**

-   A working Python file called `my_text_generator.py`
-   A working `.env` file configured locally
-   A generative text system with:
    -   system name
    -   input type
    -   output type
    -   one real use case
    -   one strong prompt design choice
    -   one trust or review consideration
-   A short written reflection:
    -   What does your system generate?
    -   What prompt choice improved the output most?
    -   What still needs human review?

#### **Independent Practice Starter Code**
```
# my_text_generator.py
# Week 2 Day 2 independent practice
# This program creates a structured text generation tool.

import os
from dotenv import load_dotenv
from openai import OpenAI

load_dotenv()
client = OpenAI(api_key=os.getenv("OPENAI_API_KEY"))

system_name = "IdeaSpark AI"
user_input = input("Enter a topic or idea: ")

prompt = f"""
You are a brainstorming assistant.

Generate:
1. A short title
2. 3 creative ideas
3. 1 next step

Topic:
"{user_input}"

Write clearly for high school Geniuses.
"""

response = client.responses.create(
    model="gpt-4.1-mini",
    input=prompt
)

print(f"\nSystem Name: {system_name}")
print("\n--- Generated Output ---")
print(response.output_text)

print("\nTrust Note: These ideas can help start the thinking process, but a user should still choose what is strongest and most realistic.")
```
#### **Facilitator Support Moves**

-   Help Geniuses choose a focused text generation task
-   Ask:
    -   What exactly should the system write?
    -   What format would help the user most?
    -   What prompt detail improves the result?
    -   What should a user still review before trusting the output?
-   Encourage systems that solve one real task clearly

### 5. **Closure (Time: 20 minutes)**

-   **Objective:** Reinforce that text generation systems are strongest when their tasks, prompts, and outputs are carefully designed.
-   Bring the class together for a final share-out.
-   Ask 3--5 Geniuses to share:
    -   their system name
    -   what it generates
    -   one strong prompt design choice
    -   one trust or review note
-   Lead a closing discussion:
    -   Why does prompt quality matter?
    -   What makes a text generation system more useful?
    -   Why is human review still important in many writing tasks?
-   Preview the next lesson:
    -   Geniuses will move into image generation systems, prompt-to-image workflows, and the technical and ethical challenges of visual generation.

**Assessment:**
---------------

Student learning will be assessed through:

-   Participation in the icebreaker and discussion
-   Reflection responses during direct instruction
-   Completion of the guided prompt comparison lab
-   Completion of an independent text generation tool
-   Final share-out and explanation of prompt design and review choices

### **Exit Ticket**

1.  What is a text generation system?
2.  What makes a prompt strong?
3.  Why might a generated text output still need review?

**Extra Activities:**
---------------------

-   Geniuses who finish early can:
    -   test multiple prompt versions
    -   generate different tones for the same topic
    -   add a stricter format like JSON
    -   compare short vs detailed instructions
    -   build a rewrite tool instead of a drafting tool
    -   add a second generation mode to the same system
-   Add a "weak output vs improved output" comparison section
-   Add user audience options
-   Add a system note explaining when the tool should not be trusted fully
-   Add a follow-up prompt improvement round

**Reflection / Takeaways:**
---------------------------

This lesson works best when Geniuses realize that text generation systems are not only creative. They are highly shaped by design choices. Day 2 helps make prompt design feel technical and practical instead of mysterious. By the end of the lesson, Geniuses should feel more confident building text generation tools that are useful, structured, and intentionally guided rather than vague and unpredictable.

**Facilitator Notes**
---------------------

-   Keep using **Geniuses** consistently in examples and discussion.
-   Reinforce that prompt design is a systems skill, not just a writing trick.
-   Encourage focused tasks and structured outputs.
-   Help Geniuses compare outputs instead of assuming one run is enough.
-   Remind Geniuses that tomorrow they will explore image generation systems and prompt-to-image workflows.

**Week 2 Day 2 Mini-Project Connection**
----------------------------------------

By the end of Day 2, each Genius should have:

-   A named text generation system concept
-   A real-world text generation use case
-   A Python-based OpenAI text generation tool
-   Experience comparing weak and strong prompts
-   At least one strong prompt design improvement
-   At least one trust or review note
-   A stronger understanding of how text generation systems behave and how output quality can be shaped
