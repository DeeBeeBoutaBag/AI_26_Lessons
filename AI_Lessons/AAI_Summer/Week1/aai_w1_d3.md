<img src="https://github.com/Hgp-GeniusLabs/Curriculum/blob/10734f2c827128dde773ea4f266d154d46977866/Org-Wide/Assets/hgp_logo_original.png" width="150"/>

Lesson Plan: Applied AI Week 1, Day 3 --- AI Workflows, System Design, and Responsible User Experience
====================================================================================================

**Duration:**
-------------

3 hours

**Lesson Overview:**
--------------------

In Day 3, Geniuses move from identifying a strong AI opportunity into designing how the product actually works. The focus of the lesson is on AI workflows, system thinking, and responsible user experience. Geniuses learn that good Applied AI products are not just single prompts. They are systems with inputs, processing steps, outputs, feedback loops, and human oversight. During guided practice, the class builds a Python-based OpenAI-powered AI Workflow Designer in VS Code that takes a product idea and generates a step-by-step workflow for how the AI system should function. In independent practice, each Genius expands their mini-project by mapping the user journey, defining what the AI does at each step, and identifying where responsibility and human review should be built in. By the end of the lesson, Geniuses will have moved from idea-stage thinking into product architecture thinking.

**Objectives:**
---------------

-   Explain the difference between an AI idea and an AI workflow.
-   Identify the key parts of an Applied AI system, including input, processing, output, feedback, and oversight.
-   Design a step-by-step AI workflow for a real user problem.
-   Evaluate where human review, transparency, and trust should appear in an AI product.
-   Build a Python tool in VS Code that uses the OpenAI API to generate and improve AI product workflows.
-   Expand a mini-project by creating a clear user flow and system design for an ethical AI product.

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
-   Existing Day 1 and Day 2 project files
-   `.env` file with OpenAI API key configured

**Standards:**
--------------

-   Computational Thinking: Model systems using inputs, processes, outputs, and feedback.
-   Computer Science Practices: Design and test computational workflows that solve real-world problems.
-   Digital Literacy: Evaluate how digital systems shape user decisions and experiences.
-   Career Readiness: Practice systems thinking, communication, and structured problem-solving.
-   Entrepreneurship and Innovation: Design AI-powered products with clear value, logic, and responsible user flow.

**Lesson Activity:**
--------------------

### 1. **Introduction (Time: 25 minutes)**

-   **Objective:** Energize Geniuses and introduce the idea that strong AI products are built as systems, not just one good prompt.
-   Start with an icebreaker called **"Human Workflow Machine."**
-   This should be the first and most energizing part of the lesson.

#### **Icebreaker Option A: Physical Activity**

-   Select 5--7 Geniuses to stand at the front of the room.
-   Tell the class they are going to act out a product workflow as if they are the parts of an AI system.
-   Assign each Genius a role:
    -   User
    -   Input Collector
    -   AI Model
    -   Output Checker
    -   Human Reviewer
    -   Final Product
-   Give the class a scenario like:
    -   "A Genius wants help choosing a career path."
    -   "A family wants an easier way to understand medical instructions."
    -   "A student wants support organizing assignments."
-   Have each person act out their step one by one.
-   After the activity, ask:
    -   What broke down in the workflow?
    -   Which step mattered most?
    -   What happens if one step is weak?
    -   Where should human review happen?

#### **Icebreaker Option B: Website Activity**

-   Use a collaborative board like Jamboard, FigJam, or Miro.
-   Present a product idea and ask Geniuses to drag labels into order:
    -   Input
    -   AI Processing
    -   Output
    -   Human Review
    -   Feedback
-   Discuss why different groups may sequence things differently.

#### **Transition**

-   Say:
    -   "A good AI product is not just one smart response. It is a system that moves information, decisions, and trust through multiple steps."
-   Ask:
    -   What makes a system strong?
    -   What happens when one part of the system is weak?

### 2. **Direct Instruction (Time: 55 minutes)**

-   **Objective:** Help Geniuses understand how Applied AI products are designed as systems with workflows, user journeys, and responsible checkpoints.
-   Use slides to guide the instruction and stop often for discussion.

#### **Suggested Slide Flow**

-   **Slide 1: Day 3 Focus --- From Idea to Workflow**
    -   Good ideas need good systems.
    -   Today is about how the AI product actually works.
-   **Slide 2: What Is a Workflow?**
    -   A workflow is the step-by-step path from user need to system response.
    -   It includes what the user gives, what the AI does, and what the user gets back.
-   **Slide 3: Core Parts of an AI Workflow**
    -   Input
    -   Processing
    -   Output
    -   Feedback
    -   Human oversight
-   **Slide 4: A Prompt Is Not the Whole Product**
    -   The product also includes:
        -   interface
        -   logic
        -   decision rules
        -   safety checks
        -   retries
        -   follow-up actions
-   **Slide 5: Example Workflow**
    -   Product: AI study helper
    -   User enters assignments
    -   AI organizes them by urgency
    -   User reviews plan
    -   Human teacher or mentor can adjust important advice
    -   User gives feedback on whether plan worked
-   **Slide 6: User Experience Matters**
    -   Is the system easy to understand?
    -   Does the user know what the AI is doing?
    -   Does the user know when to trust it and when to double-check?
-   **Slide 7: Responsible System Design**
    -   Where should users be warned?
    -   Where should humans review?
    -   Where could errors have the biggest impact?
    -   What happens when the AI does not know?
-   **Slide 8: Inputs Shape Outputs**
    -   Better inputs create better outputs.
    -   Weak inputs can create confusion, bias, or poor recommendations.
-   **Slide 9: Great Applied AI Products Have Clear Flows**
    -   What happens first?
    -   What happens next?
    -   What does the user do?
    -   What does the AI do?
    -   What happens if something goes wrong?
-   **Slide 10: Mini-Project Growth**
    -   Day 1: ethical product idea
    -   Day 2: user and problem clarity
    -   Day 3: workflow and system design

#### **Discussion Questions**

-   Why is one good prompt not enough to make a good product?
-   What parts of an AI system matter besides the model?
-   Where should a human be involved in your product?
-   How can workflow design improve trust?
-   What could go wrong if a system is too automated?

#### **Reflection Prompt**

-   Have Geniuses write for 4 minutes:
    -   "Think about a real app or website you use. What steps happen between your action and the final result?"

### 3. **Guided Practice (Time: 50 minutes)**

-   **Objective:** Help Geniuses build a Python tool in VS Code that uses the OpenAI API to generate an AI workflow for a product idea and identify responsible design checkpoints.
-   Explain that product teams often map workflows before building full products.
-   Today's code-along will create `ai_workflow_designer.py`.

#### **Guided Practice Build**

Use the existing project folder or create a new folder called `ai-workflow-designer`.

#### **Project Goal**

Build a Python script that:

-   Takes in a product name
-   Takes in a target user
-   Takes in a problem solved
-   Sends that information to the OpenAI API
-   Gets back:
    -   a step-by-step workflow
    -   where the AI acts
    -   where the user acts
    -   one human review checkpoint
    -   one ethical risk in the workflow
    -   one improvement suggestion

#### **Setup Steps**

1.  Open the project in VS Code.
2.  Confirm `.env` is still configured.
3.  Confirm required packages are installed:
```
pip install openai python-dotenv
```
1.  Create a file called `ai_workflow_designer.py`

#### **Sample Code**
```
# ai_workflow_designer.py
# Applied AI Week 1 Day 3
# This script helps a Genius design an AI workflow
# for a product idea using the OpenAI API.

import os
from dotenv import load_dotenv
from openai import OpenAI

# Load environment variables
load_dotenv()

# Create the OpenAI client
client = OpenAI(api_key=os.getenv("OPENAI_API_KEY"))

print("Welcome to the AI Workflow Designer\n")

# Collect information about the product idea
product_name = input("What is the product name? ")
target_user = input("Who is the target user? ")
problem_solved = input("What problem does the product solve? ")

# Build the prompt
prompt = f"""
You are an Applied AI workflow advisor helping a Genius design an ethical AI product.

Product Name: {product_name}
Target User: {target_user}
Problem Solved: {problem_solved}

Please respond in the following format:
1. Step-by-step workflow with 5 steps
2. Where the AI acts in the workflow
3. Where the user acts in the workflow
4. One place where human review should be added
5. One ethical risk in this workflow
6. One suggestion to improve trust and user experience

Keep the response clear, practical, and student-friendly.
"""

# Send the request to the OpenAI API
response = client.responses.create(
    model="gpt-4.1-mini",
    input=prompt
)

# Print the workflow analysis
print("\n--- AI Workflow Analysis ---")
print(response.output_text)
```
#### **Guided Practice Teaching Points**

-   Why systems need step-by-step logic
-   How user actions and AI actions connect
-   Why workflows should include review and feedback
-   How responsible design shows up inside the workflow
-   Why product builders need to design for mistakes, not just success

#### **Guided Practice Discussion**

-   Was the workflow too broad or useful?
-   Did the response make the product easier to imagine?
-   Where should more detail be added?
-   How could the workflow become safer or more trustworthy?

### 4. **Independent Practice (Time: 35 minutes)**

-   **Objective:** Geniuses independently expand their mini-project by designing a clear workflow and responsible user journey for their product.
-   Geniuses continue building toward Day 4.

#### **Mini-Project Title**

**Ethical AI Business Starter --- Day 3 Workflow Expansion**

#### **Independent Task**

Each Genius updates their product concept by designing the workflow for how the system works from beginning to end.

They must define:

-   What the user does first
-   What information the system collects
-   What the AI does
-   What output the user receives
-   Where feedback happens
-   Where human review or transparency should be added

#### **Required Deliverables**

-   A working Python file called `my_ai_workflow.py` or an updated previous file
-   A workflow with:
    -   Product name
    -   Target user
    -   Problem solved
    -   4--6 workflow steps
    -   One human review checkpoint
    -   One ethical risk in the workflow
    -   One trust-building feature
-   A short written reflection:
    -   What step in your workflow matters most?
    -   Where could your system fail or confuse users?

#### **Independent Practice Starter Code**
```
# my_ai_workflow.py
# Day 3 independent practice
# This script stores a Genius's product information
# and asks the OpenAI API to help design a workflow.

import os
from dotenv import load_dotenv
from openai import OpenAI

# Load environment variables
load_dotenv()

# Create the API client
client = OpenAI(api_key=os.getenv("OPENAI_API_KEY"))

product_name = "CareerPath AI"
target_user = "High school students exploring careers"
problem_solved = "Helps students discover career paths that match their strengths and interests"

prompt = f"""
You are helping a Genius design an ethical Applied AI workflow.

Product Name: {product_name}
Target User: {target_user}
Problem Solved: {problem_solved}

Please provide:
1. A 5-step user workflow
2. One place where the AI makes a recommendation
3. One place where the user reviews or edits the result
4. One human oversight checkpoint
5. One ethical risk in the workflow
6. One trust-building product feature

Use clear and practical language.
"""

response = client.responses.create(
    model="gpt-4.1-mini",
    input=prompt
)

print("Applied AI Workflow Design\n")
print(f"Product Name: {product_name}")
print(f"Target User: {target_user}")
print(f"Problem Solved: {problem_solved}")

print("\n--- Workflow Feedback ---")
print(response.output_text)
```
#### **Facilitator Support Moves**

-   Push Geniuses to think beyond "the AI gives an answer"
-   Ask:
    -   What happens before the AI responds?
    -   What happens after?
    -   Can the user edit or question the output?
    -   What happens if the AI is wrong?
-   Help Geniuses build workflows that feel realistic and trustworthy

### 5. **Closure (Time: 15 minutes)**

-   **Objective:** Reinforce the idea that great Applied AI products are carefully designed systems, not just smart outputs.
-   Bring the class together for a final share-out.
-   Ask 3--5 Geniuses to share:
    -   Their product name
    -   Their workflow
    -   One place where human review happens
    -   One trust-building feature they added
-   Lead a closing discussion:
    -   What changed when you started thinking step by step?
    -   What part of workflow design was most challenging?
    -   Why do strong AI products need both smart outputs and smart structure?
-   Preview the next lesson:
    -   Geniuses will move into improving the output itself by designing better prompts, response structures, and product behavior.

**Assessment:**
---------------

Student learning will be assessed through:

-   Participation in the icebreaker and discussion
-   Reflection responses during direct instruction
-   Completion of the guided OpenAI API workflow build in VS Code
-   Independent mini-project updates with workflow and system design
-   Final share-out and closing reflection

### **Exit Ticket**

1.  What is an AI workflow?
2.  Why is one good prompt not enough to make a strong product?
3.  Where should human review appear in an AI system?

**Extra Activities:**
---------------------

-   Geniuses who finish early can add user input instead of hard-coded values
-   Ask the model to generate alternate workflows for the same product
-   Return the workflow as JSON and print each part clearly
-   Add a second prompt that asks the AI to critique the first workflow
-   Compare two workflow designs and decide which one is more trustworthy
-   Add basic error handling for missing API keys

**Reflection / Takeaways:**
---------------------------

This lesson works best when Geniuses realize that product quality is not just about having a capable AI model. It is about designing a full experience that guides the user, handles uncertainty, and builds trust step by step. By mapping workflows, Geniuses begin thinking like real product builders who design systems instead of isolated features. Day 3 helps move the mini-project from concept into structure, making the final product more realistic, useful, and responsible.

**Facilitator Notes**
---------------------

-   Keep using **Geniuses** consistently in all examples and discussion.
-   Reinforce that workflows should include both user actions and AI actions.
-   Encourage Geniuses to think about what happens when the system is wrong, unclear, or incomplete.
-   Keep the lesson grounded in product design and business value, not just code.
-   Remind Geniuses that a trustworthy workflow is a competitive advantage.

**Day 3 Mini-Project Connection**
---------------------------------

By the end of Day 3, each Genius should have:

-   A product concept
-   A target user
-   A clear problem being solved
-   A step-by-step workflow
-   A clear place where the AI acts
-   A clear place where the user acts
-   At least one human oversight checkpoint
-   At least one ethical risk inside the workflow
-   At least one trust-building feature
-   A working OpenAI-powered workflow design tool
