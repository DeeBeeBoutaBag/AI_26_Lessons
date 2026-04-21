<img src="https://github.com/Hgp-GeniusLabs/Curriculum/blob/10734f2c827128dde773ea4f266d154d46977866/Org-Wide/Assets/hgp_logo_original.png" width="150"/>

Lesson Plan: Applied AI Week 1, Day 4 --- Prompt Engineering, Product Behavior, and Mini-Project Build Day
========================================================================================================

**Duration:**
-------------

3 hours

**Lesson Overview:**
--------------------

In Day 4, Geniuses bring together everything they have built so far by focusing on prompt engineering, product behavior, and output quality. After identifying a responsible AI opportunity, clarifying the target user, and designing a workflow, Geniuses now improve the actual intelligence and usefulness of their product. The lesson explores how prompts shape AI behavior, how product teams define tone and output structure, and how builders can make AI responses more helpful, safe, and trustworthy. During guided practice, the class builds a Python-based OpenAI-powered Prompt Tester in VS Code that compares weak prompts and strong prompts for the same product idea. In independent practice, each Genius completes a stronger version of their mini-project by refining their product prompt, improving product behavior, and preparing a functional Day 4 build. By the end of the lesson, Geniuses will have a clearer, more usable, and more responsible Applied AI prototype.

**Objectives:**
---------------

-   Explain how prompt design shapes the quality, structure, and trustworthiness of AI outputs.
-   Identify the difference between weak prompts and strong prompts in real product contexts.
-   Design prompts that reflect user needs, product goals, and responsible AI considerations.
-   Improve an AI product by defining its tone, response structure, and boundaries.
-   Build a Python tool in VS Code that uses the OpenAI API to compare prompt quality.
-   Complete a stronger Day 4 mini-project prototype with improved prompts, workflow logic, and product behavior.

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
-   Existing Day 1, Day 2, and Day 3 files
-   `.env` file with OpenAI API key configured

**Standards:**
--------------

-   Computational Thinking: Refine inputs and outputs to improve system performance.
-   Computer Science Practices: Test, compare, and improve computational solutions.
-   Digital Literacy: Evaluate how interface and response design influence user trust.
-   Career Readiness: Use iteration, communication, and strategic thinking to improve products.
-   Entrepreneurship and Innovation: Improve a product by making its value clearer, its output stronger, and its experience more trustworthy.

**Lesson Activity:**
--------------------

### 1. **Introduction (Time: 25 minutes)**

-   **Objective:** Energize Geniuses and help them see that better AI products come from better instructions, better design choices, and better iteration.
-   Start with an icebreaker called **"Prompt Battle."**
-   This should be the first and most energetic part of the lesson.

#### **Icebreaker Option A: Physical Competition**

-   Divide the room into small groups.
-   Display a simple product goal such as:
    -   Help a Genius organize homework
    -   Help a user prepare for an interview
    -   Help a family member understand a confusing message
-   Give each group 2 minutes to write a prompt that would get a great result from an AI tool.
-   After time is up, read the prompts aloud.
-   The class votes by moving to one side of the room for:
    -   **Strong Prompt**
    -   **Needs Work**
-   Discuss:
    -   What made one prompt clearer?
    -   Which prompt gave the AI better instructions?
    -   Which one would work better inside a real product?

#### **Icebreaker Option B: Website Activity**

-   Use Mentimeter, Slido, or a shared document.
-   Show 2--3 prompts for the same task and ask Geniuses to vote on which one would perform best.
-   Example:
    -   Weak prompt: "Help with homework."
    -   Strong prompt: "You are a study coach helping a high school Genius organize four assignments by urgency and estimated time. Respond in a checklist format."
-   Discuss why one prompt is clearly stronger.

#### **Transition**

-   Say:
    -   "The model matters, but the instructions matter too. Product builders shape AI behavior through prompts, structure, and boundaries."
-   Ask:
    -   What makes an AI response feel useful?
    -   What makes an AI response feel random or weak?

### 2. **Direct Instruction (Time: 55 minutes)**

-   **Objective:** Help Geniuses understand how prompt engineering and product behavior influence output quality, trust, and user experience.
-   Use slides to guide the lesson and pause often for questions and examples.

#### **Suggested Slide Flow**

-   **Slide 1: Day 4 Focus --- Improve the Intelligence of the Product**
    -   A strong product does not just have an idea and workflow.
    -   It also needs strong behavior and quality outputs.
-   **Slide 2: What Is Prompt Engineering?**
    -   Prompt engineering is the process of designing instructions that help AI generate better results.
    -   It is part of product design.
-   **Slide 3: Weak Prompt vs Strong Prompt**
    -   Weak: vague, short, unclear, missing audience or goal
    -   Strong: clear role, task, format, tone, audience, and constraints
-   **Slide 4: Core Parts of a Strong Product Prompt**
    -   Role
    -   User context
    -   Task
    -   Format
    -   Tone
    -   Boundaries
    -   Success criteria
-   **Slide 5: Product Behavior Matters**
    -   Should the AI be encouraging, concise, formal, step-by-step, cautious, or conversational?
    -   Product teams define behavior on purpose.
-   **Slide 6: Output Structure Creates Trust**
    -   Lists
    -   Steps
    -   Sections
    -   Warnings
    -   Summaries
    -   Next actions
-   **Slide 7: Responsible Prompt Design**
    -   Avoid pretending certainty when uncertainty exists
    -   Encourage human review in high-impact situations
    -   Use clear language
    -   Avoid harmful assumptions
    -   Give limitations when needed
-   **Slide 8: Iteration Is Normal**
    -   Product teams test and revise prompts constantly
    -   Better prompts often come from comparing results
-   **Slide 9: Prompt Design Is Business Design**
    -   Better outputs can improve retention, trust, usefulness, and product value
-   **Slide 10: Mini-Project Goal for Today**
    -   Improve your product's behavior and output so it feels more real, more useful, and more trustworthy

#### **Discussion Questions**

-   Why can the same model produce weak or excellent output depending on the prompt?
-   What kind of tone would build trust in your product?
-   What output format would make your product more useful?
-   Where should your product be cautious or transparent?
-   What would make a user want to come back to your product again?

#### **Reflection Prompt**

-   Have Geniuses write for 4 minutes:
    -   "Think about your product. What kind of personality, structure, and tone should it have to serve your user well?"

### 3. **Guided Practice (Time: 50 minutes)**

-   **Objective:** Help Geniuses build a Python tool in VS Code that compares weak prompts and strong prompts for the same product scenario and shows how prompt design changes output quality.
-   Explain that today they will build a testing tool that product teams could really use.
-   The class will create `prompt_tester.py`.

#### **Guided Practice Build**

Use the existing project folder or create a new folder called `prompt-tester`.

#### **Project Goal**

Build a Python script that:

-   Takes in a product goal
-   Creates a weak prompt and a stronger prompt
-   Sends both to the OpenAI API
-   Prints both results
-   Helps the class compare quality, structure, and usefulness

#### **Setup Steps**

1.  Open the project in VS Code.
2.  Confirm `.env` is still configured.
3.  Confirm required packages are installed:
```
pip install openai python-dotenv
```
1.  Create a file called `prompt_tester.py`

#### **Sample Code**
```
# prompt_tester.py
# Applied AI Week 1 Day 4
# This script compares a weak prompt and a strong prompt
# for the same product goal using the OpenAI API.

import os
from dotenv import load_dotenv
from openai import OpenAI

# Load environment variables
load_dotenv()

# Create the OpenAI client
client = OpenAI(api_key=os.getenv("OPENAI_API_KEY"))

print("Welcome to the Prompt Tester\n")

# Product goal for the prompt comparison
product_goal = input("What is the product goal? ")

# Weak prompt example
weak_prompt = f"""
Help with this: {product_goal}
"""

# Strong prompt example
strong_prompt = f"""
You are a helpful and responsible AI product assistant.

A Genius is building an Applied AI product with this goal:
{product_goal}

Please respond with:
1. A clear response for the end user
2. A step-by-step format
3. A helpful and encouraging tone
4. One note about what the user should double-check if needed

Keep the response clear, practical, and trustworthy.
"""

# Send weak prompt to the API
weak_response = client.responses.create(
    model="gpt-4.1-mini",
    input=weak_prompt
)

# Send strong prompt to the API
strong_response = client.responses.create(
    model="gpt-4.1-mini",
    input=strong_prompt
)

# Print results\
print("\n--- Weak Prompt Output ---")\
print(weak_response.output_text)

print("\n--- Strong Prompt Output ---")\
print(strong_response.output_text)
```
#### **Guided Practice Teaching Points**

-   Why prompt structure changes output
-   Why role and audience matter
-   Why format can improve usability
-   Why trustworthy products often include limitations or caution
-   Why testing prompts is part of product development

#### **Guided Practice Discussion**

-   Which response was more useful?
-   Which one felt more product-ready?
-   What parts of the strong prompt made the biggest difference?
-   How might your own product benefit from more structure or caution?

### 4. **Independent Practice (Time: 35 minutes)**

-   **Objective:** Geniuses independently improve their mini-project by refining the main prompt, output structure, and overall behavior of their AI product.
-   Geniuses continue building toward a completed Day 4 prototype.

#### **Mini-Project Title**

**Ethical AI Business Starter --- Day 4 Product Build**

#### **Independent Task**

Each Genius updates their product by designing:

-   A main product prompt
-   A clear user-facing output format
-   A product tone or behavior style
-   At least one trust-building or safety instruction
-   A stronger working demo in Python using the OpenAI API

#### **Required Deliverables**

-   A working Python file called `my_product_build.py` or an updated previous project file
-   A product build with:
    -   Product name
    -   Target user
    -   Main product prompt
    -   Output structure
    -   Tone or behavior description
    -   One trust or safety feature
-   A short written reflection:
    -   What changed when you improved the prompt?
    -   What makes your product feel more real now?

#### **Independent Practice Starter Code**
```
# my_product_build.py
# Day 4 independent practice
# This script represents a Genius's improved AI product build
# using a stronger product prompt.

import os
from dotenv import load_dotenv
from openai import OpenAI

# Load environment variables
load_dotenv()

# Create the API client
client = OpenAI(api_key=os.getenv("OPENAI_API_KEY"))

product_name = "CareerPath AI"
target_user = "High school Geniuses exploring future careers"
product_goal = "Help users discover career paths that match their interests and strengths"

prompt = f"""
You are CareerPath AI, a helpful and responsible career exploration assistant.

Your target user is: {target_user}
Your goal is: {product_goal}

When responding:
1\. Be encouraging and clear
2\. Give step-by-step suggestions
3\. Keep the language simple and practical
4\. Do not pretend to know the user's future
5\. Remind the user that this is guidance, not a final decision

Now respond to this user question:
'I like technology, helping people, and solving problems. What are some careers I should explore?'\
"""

response = client.responses.create(
    model="gpt-4.1-mini",
    input=prompt
)

print("Applied AI Product Build\n")
print(f"Product Name: {product_name}")
print(f"Target User: {target_user}")
print(f"Product Goal: {product_goal}")

print("\n--- Product Output ---")
print(response.output_text)
```
#### **Facilitator Support Moves**

-   Push Geniuses to make their prompts more specific
-   Ask:
    -   What should the AI sound like?
    -   What should it never do?
    -   How should it organize its response?
    -   What would make a user trust this output?
-   Help Geniuses revise prompts multiple times and compare results

### 5. **Closure (Time: 15 minutes)**

-   **Objective:** Reinforce the idea that prompt design and output quality are essential parts of building a real Applied AI product.
-   Bring the class together for a final share-out.
-   Ask 3--5 Geniuses to share:
    -   Their product name
    -   Their improved prompt
    -   One behavior or tone choice they made
    -   One trust-building feature they added
-   Lead a closing discussion:
    -   What changed when you got more specific with the prompt?
    -   How did output structure affect usefulness?
    -   Why should product teams test prompts instead of just using the first version?
-   Preview the next lesson:
    -   Day 5 will be a flex and enhancement day where Geniuses strengthen, polish, and extend their product builds.

**Assessment:**
---------------

Student learning will be assessed through:

-   Participation in the icebreaker and discussion
-   Reflection responses during direct instruction
-   Completion of the guided prompt comparison build in VS Code
-   Independent mini-project updates with improved prompts and product behavior
-   Final share-out and closing reflection

### **Exit Ticket**

1.  What makes a prompt strong?
2.  How can prompt design affect user trust?
3.  What improved in your product today?

**Extra Activities:**
---------------------

-   Geniuses who finish early can let the user type their own question into the script
-   Add multiple prompt versions and compare three outputs instead of two
-   Ask the model to score the output for clarity and usefulness
-   Return the answer in JSON and print each section clearly
-   Add basic error handling for missing API keys
-   Create a version that stores the final product prompt in a variable and reuses it for different user questions

**Reflection / Takeaways:**
---------------------------

This lesson works best when Geniuses realize that the difference between a weak AI experience and a strong one often comes down to product decisions that happen before the user ever sees the output. Prompt engineering is not just a technical trick. It is a product design skill that shapes usefulness, trust, and quality. By the end of Day 4, Geniuses should have a much more complete and believable Applied AI prototype that reflects not only a strong idea, but also strong behavior, structure, and responsibility.

**Facilitator Notes**
---------------------

-   Keep using **Geniuses** consistently in every example and prompt.
-   Reinforce that prompts are part of the product, not separate from it.
-   Encourage multiple rounds of revision and comparison.
-   Keep product behavior tied to user trust and business value.
-   Remind Geniuses that iteration is a normal and powerful part of building.

**Day 4 Mini-Project Connection**
---------------------------------

By the end of Day 4, each Genius should have:

-   A product concept
-   A clear target user
-   A defined problem
-   A workflow
-   A main product prompt
-   A defined tone or behavior style
-   A clear output structure
-   At least one trust-building or safety instruction
-   A stronger OpenAI-powered working prototype in Python
