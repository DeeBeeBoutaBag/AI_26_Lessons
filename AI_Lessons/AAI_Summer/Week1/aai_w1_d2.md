<img src="https://github.com/Hgp-GeniusLabs/Curriculum/blob/10734f2c827128dde773ea4f266d154d46977866/Org-Wide/Assets/hgp_logo_original.png" width="150"/>

Lesson Plan: Applied AI Week 1, Day 2 --- Problem Discovery, Customer Needs, and Ethical AI Opportunity Mapping
=============================================================================================================

**Duration:**
-------------

3 hours

**Lesson Overview:**
--------------------

In Day 2, Geniuses move from broad responsible AI thinking into sharper product thinking. They explore how strong Applied AI products begin with real user problems, not just cool technology. Geniuses learn how to identify a target user, define a pain point, and evaluate whether AI is actually the right solution. They also continue grounding their work in responsible AI by examining which users benefit, which users may be excluded, and what harm could come from a weak solution. During guided practice, the class builds a Python-based OpenAI-powered Customer Problem Explorer in VS Code that helps analyze a user type, their pain points, and possible AI-supported solutions. In independent practice, each Genius expands their Day 1 mini-project by defining a sharper customer persona, a stronger problem statement, and an improved AI product concept that better fits real business and community needs.

**Objectives:**
---------------

-   Explain why strong Applied AI products begin with real user problems and clear customer needs.
-   Identify the difference between a vague idea and a specific, valuable AI use case.
-   Define a target user, a pain point, and a reason that user would care about the solution.
-   Evaluate whether AI is the right tool for solving a problem.
-   Build a Python program in VS Code that uses the OpenAI API to explore customer pain points and solution opportunities.
-   Expand a mini-project by refining an AI business idea with stronger user focus and clearer value.

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
-   Existing Day 1 project files
-   `.env` file with OpenAI API key configured

**Standards:**
--------------

-   Computational Thinking: Break down real-world problems into users, needs, inputs, and outputs.
-   Computer Science Practices: Design computational solutions based on real human needs and constraints.
-   Digital Literacy: Evaluate the impact of digital products on users and communities.
-   Career Readiness: Practice empathy, communication, and strategic problem-solving.
-   Entrepreneurship and Innovation: Identify customer needs and design responsible products that create value.

**Lesson Activity:**
--------------------

### 1. **Introduction (Time: 25 minutes)**

-   **Objective:** Wake Geniuses up with energy and help them recognize that the best products solve real problems, not random ideas.
-   Start with an icebreaker called **"Bad Product or Brilliant Product?"**
-   This should be the first and most energetic part of the lesson.

#### **Icebreaker Option A: Physical Corners**

-   Label four corners of the room:
    -   **Need This**
    -   **Maybe Useful**
    -   **Cool But Pointless**
    -   **Absolutely Not**
-   Read product ideas aloud and have Geniuses move to a corner.
-   Example prompts:
    -   AI that writes apology texts for you
    -   AI that helps students plan homework schedules
    -   AI that picks outfits based on weather
    -   AI that automatically rejects job applicants
    -   AI that helps elders remember medications
    -   AI that summarizes class notes
    -   AI that generates fake influencer comments
-   After each one, ask:
    -   Who is this actually for?
    -   What real problem does it solve?
    -   Is AI even needed here?
    -   What could go wrong?

#### **Icebreaker Option B: Website Activity**

-   Use Mentimeter, Slido, or a polling board where Geniuses rank each idea from:
    -   Very valuable
    -   Somewhat useful
    -   Weak idea
    -   Harmful idea
-   Discuss which ideas got split opinions and why.

#### **Transition**

-   Say:
    -   "A lot of people start with the technology. Strong builders start with the problem."
-   Ask:
    -   What makes a product actually useful?
    -   What is the difference between a fun AI demo and a real AI product?

### 2. **Direct Instruction (Time: 55 minutes)**

-   **Objective:** Help Geniuses understand how customer problems, business value, and responsible design connect in Applied AI.
-   Use slides to lead the lesson and pause often for discussion.

#### **Suggested Slide Flow**

-   **Slide 1: Day 2 Focus --- Build for a Real Problem**
    -   Strong Applied AI starts with people, needs, and pain points.
    -   AI is not the goal. Solving the right problem is the goal.
-   **Slide 2: What Is a Customer Problem?**
    -   A customer problem is something frustrating, slow, expensive, confusing, repetitive, or hard.
    -   Good products reduce pain or create value.
-   **Slide 3: Vague Idea vs Specific Problem**
    -   Weak: "An AI app for school"
    -   Strong: "An AI study helper for high school students who struggle to organize assignments across multiple classes"
-   **Slide 4: Customer Persona Basics**
    -   Who is the user?
    -   What do they need?
    -   What do they struggle with?
    -   What do they care about most?
-   **Slide 5: Pain Points and Friction**
    -   Time
    -   Cost
    -   Confusion
    -   Access
    -   Consistency
    -   Motivation
    -   Accuracy
-   **Slide 6: When Is AI the Right Tool?**
    -   AI is strong when:
        -   Language is involved
        -   Recommendations are needed
        -   Summarization helps
        -   Pattern-based support helps
        -   Personalization matters
    -   AI may not be needed when:
        -   A simple form works
        -   A checklist works
        -   Rules are fixed and predictable
-   **Slide 7: Business Value + User Value**
    -   Good Applied AI products should help users and create value for organizations.
    -   Ask:
        -   Does this save time?
        -   Does this improve quality?
        -   Does this reduce cost?
        -   Does this improve access?
-   **Slide 8: Responsible Opportunity Mapping**
    -   Who benefits?
    -   Who might be left out?
    -   What assumptions are being made?
    -   What happens if the AI is wrong?
-   **Slide 9: Great Builders Ask Better Questions**
    -   What is the real user struggle?
    -   Why does it matter now?
    -   Why would someone trust this?
    -   Is AI the best solution or just the trendiest one?
-   **Slide 10: Mini-Project Growth**
    -   Yesterday: ethical AI idea
    -   Today: sharpen the user, problem, and product fit

#### **Discussion Questions**

-   Why do weak products often start with features instead of problems?
-   What is a real problem you see in school, work, family, or community life?
-   When might AI make a product better?
-   When might AI just make a product more complicated?
-   How can we tell whether an idea has real value?

#### **Reflection Prompt**

-   Have Geniuses write for 4 minutes:
    -   "Describe a real frustration people deal with often. Who experiences it, and why does it matter?"

### 3. **Guided Practice (Time: 50 minutes)**

-   **Objective:** Help Geniuses build a Python tool in VS Code that uses the OpenAI API to analyze a target user, their pain points, and possible Applied AI opportunities.
-   Explain that real product teams often study users before building.
-   Today's code-along will create a tool called `customer_problem_explorer.py`.

#### **Guided Practice Build**

Create or continue using the existing project folder from Day 1, or create a new folder called `customer-problem-explorer`.

#### **Project Goal**

Build a Python script that:

-   Asks for a target user
-   Asks for a pain point
-   Asks for a setting or context
-   Sends that information to the OpenAI API
-   Gets back:
    -   a clearer problem definition
    -   why the problem matters
    -   whether AI is a strong fit
    -   one ethical concern
    -   one suggested product direction

#### **Setup Steps**

1.  Open the project in VS Code.
2.  Confirm `.env` is still working.
3.  Confirm required packages are installed:
```
pip install openai python-dotenv
```
1.  Create a file called `customer_problem_explorer.py`

#### **Sample Code**
```
# customer_problem_explorer.py
# Applied AI Week 1 Day 2
# This script helps a Genius explore a customer problem
# and determine whether AI is a good fit for the solution.

import os
from dotenv import load_dotenv
from openai import OpenAI

# Load the API key from the .env file
load_dotenv()

# Create the OpenAI client
client = OpenAI(api_key=os.getenv("OPENAI_API_KEY"))

print("Welcome to the Customer Problem Explorer\n")

# Collect user input
target_user = input("Who is the target user? ")
pain_point = input("What is the main problem they face? ")
context = input("What situation or environment does this happen in? ")

# Build the prompt
prompt = f"""
You are an Applied AI product advisor helping a Genius refine an AI business idea.

Target User: {target_user}
Pain Point: {pain_point}
Context: {context}

Please respond in the following format:
1. Clear Problem Statement
2. Why This Problem Matters
3. Is AI a good fit? Why or why not?
4. One ethical concern to watch for
5. One strong product direction

Keep the response clear, practical, and student-friendly.
"""

# Send the request to the OpenAI API
response = client.responses.create(
    model="gpt-4.1-mini",
    input=prompt
)

# Print the result
print("\n--- Product Opportunity Analysis ---")
print(response.output_text)
```
#### **Guided Practice Teaching Points**

-   Why user input matters in product thinking
-   Why a problem statement should be specific
-   Why not every problem needs AI
-   How prompt structure changes output quality
-   Why product builders need both creativity and judgment

#### **Guided Practice Discussion**

-   Was the AI's advice too broad or helpful?
-   Did the AI explain clearly whether AI is actually needed?
-   What would make this tool more useful for a real startup team?
-   How could we improve the prompt to get stronger results?

### 4. **Independent Practice (Time: 35 minutes)**

-   **Objective:** Geniuses independently sharpen their mini-project by defining a clear target user, real pain point, and stronger AI opportunity.
-   Geniuses continue the mini-project from Day 1 and build toward Day 4.

#### **Mini-Project Title**

**Ethical AI Business Starter --- Day 2 Expansion**

#### **Independent Task**

Each Genius updates their project by defining:

-   A sharper target user
-   A clearer customer pain point
-   A better explanation of why the problem matters
-   Whether AI is truly the right solution
-   One new ethical concern connected to the specific user and problem

#### **Required Deliverables**

-   A working Python file called `my_customer_problem.py` or an updated Day 1 file
-   A product concept with:
    -   Product name
    -   Target user
    -   Customer pain point
    -   Why the problem matters
    -   Why AI is or is not a strong fit
    -   One ethical concern
    -   One improved product direction
-   A short written reflection:
    -   What makes this a real problem worth solving?
    -   Why would a user trust this solution?

#### **Independent Practice Starter Code**
```
# my_customer_problem.py
# Day 2 independent practice
# This script stores a Genius's customer problem
# and asks the OpenAI API to help refine the opportunity.

import os
from dotenv import load_dotenv
from openai import OpenAI

# Load environment variables
load_dotenv()

# Create API client
client = OpenAI(api_key=os.getenv("OPENAI_API_KEY"))

product_name = "CareerPath AI"
target_user = "High school students who are unsure what jobs fit their strengths"
pain_point = "They do not know where to start when exploring careers and often feel overwhelmed"
why_it_matters = "Without guidance, students may miss opportunities, lose confidence, or choose paths that do not fit them"

prompt = f"""
You are an Applied AI advisor helping a Genius improve a business idea.

Product Name: {product_name}
Target User: {target_user}
Pain Point: {pain_point}
Why It Matters: {why_it_matters}

Please provide:
1. A sharper one-sentence problem statement
2. Whether AI is a strong fit and why
3. One ethical concern
4. One recommendation to improve the product idea

Use clear and practical language.
"""

response = client.responses.create(
    model="gpt-4.1-mini",
    input=prompt
)

print("Applied AI Product Refinement\n")
print(f"Product Name: {product_name}")
print(f"Target User: {target_user}")
print(f"Pain Point: {pain_point}")
print(f"Why It Matters: {why_it_matters}")

print("\n--- AI Feedback ---")
print(response.output_text)

#### **Facilitator Support Moves**

-   Push Geniuses to avoid broad target users like "everyone"
-   Help them move from generic pain points to specific ones
-   Ask:
    -   When does this problem happen?
    -   Why is it frustrating?
    -   What would success look like?
-   Challenge Geniuses to explain why AI is necessary, not just exciting

### 5. **Closure (Time: 15 minutes)**

-   **Objective:** Reinforce the idea that strong Applied AI products begin with empathy, specificity, and problem clarity.
-   Bring the class together for a final share-out.
-   Ask 3--5 Geniuses to share:
    -   Their product name
    -   Their target user
    -   Their customer pain point
    -   Whether AI is really the right solution
-   Lead a closing discussion:
    -   What was harder today: finding a problem or thinking of a solution?
    -   Did any ideas become stronger after focusing on the user?
    -   Why do businesses need to understand people before building products?
-   Preview the next lesson:
    -   Geniuses will move into designing stronger product workflows and thinking about what the AI actually does step by step.

**Assessment:**
---------------

Student learning will be assessed through:

-   Participation in the icebreaker and discussion
-   Reflection responses during direct instruction
-   Completion of the guided OpenAI API build in VS Code
-   Independent mini-project updates with stronger user and problem definition
-   Final share-out and closing reflection

### **Exit Ticket**

1.  Why should product builders start with the problem instead of the technology?
2.  What makes a customer problem specific and useful?
3.  How can a builder tell whether AI is the right tool?

**Extra Activities:**
---------------------

-   Geniuses who finish early can update their script to ask follow-up questions
-   Add a second prompt that generates three alternate product directions
-   Ask the model to rate the problem's urgency from 1 to 10 and explain why
-   Add user input instead of hard-coded values
-   Return the result in JSON and print each section clearly
-   Compare two customer problems and decide which is stronger for an AI business idea

**Reflection / Takeaways:**
---------------------------

This lesson works best when Geniuses leave understanding that strong Applied AI is not about starting with a model or a cool feature. It is about starting with a real person, a real frustration, and a clear reason the solution matters. The OpenAI API helps Geniuses explore and refine opportunities faster, but the real skill is judgment. By the end of Day 2, Geniuses should see that better user understanding leads to better products, stronger trust, and more meaningful innovation.

**Facilitator Notes**
---------------------

-   Keep using **Geniuses** throughout examples and discussion.
-   Reinforce that not every product idea needs AI.
-   Keep the conversation grounded in real people and real situations.
-   Encourage Geniuses to use examples from school, family, community, sports, work, and daily life.
-   Remind Geniuses that sharper inputs often lead to sharper outputs.

**Day 2 Mini-Project Connection**
---------------------------------

By the end of Day 2, each Genius should have:

-   A stronger product name or concept
-   A clearly defined target user
-   A clear customer pain point
-   A stronger explanation of why the problem matters
-   A clearer answer to whether AI is actually a good fit
-   At least one new ethical concern based on the specific user and use case
-   A working OpenAI-powered product opportunity analysis tool
