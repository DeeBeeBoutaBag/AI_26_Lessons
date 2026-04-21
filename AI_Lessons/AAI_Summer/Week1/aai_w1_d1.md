<img src="https://github.com/Hgp-GeniusLabs/Curriculum/blob/10734f2c827128dde773ea4f266d154d46977866/Org-Wide/Assets/hgp_logo_original.png" width="150"/>

Lesson Plan: Applied AI Week 1, Day 1 --- Business Ethics, Responsible AI, and Real-World AI Products
===================================================================================================

**Duration:**
-------------

3 hours

**Lesson Overview:**
--------------------

In this first Applied AI lesson, Geniuses are introduced to Applied AI as the business application of artificial intelligence in the modern world. The lesson is grounded in ethics, responsibility, and product thinking. Geniuses explore where AI shows up in real businesses and communities, discuss why responsible AI matters, and begin thinking like builders who must balance innovation with trust. During guided practice, the class sets up a simple OpenAI-powered Python project in VS Code and builds a basic Responsible AI Idea Reviewer that uses the OpenAI API to analyze an AI product idea for ethical considerations. In independent practice, each Genius begins a mini-project that will grow through Day 4: an ethical AI business concept supported by both their own thinking and an API-powered reflection tool.

**Objectives:**
---------------

-   Define Applied AI and explain how businesses use AI to solve modern problems.
-   Identify key responsible AI concepts including fairness, bias, privacy, transparency, accountability, and human oversight.
-   Analyze an AI product idea through both a business lens and an ethical lens.
-   Build a simple Python program in VS Code that uses the OpenAI API to review an AI idea for risks and responsibility.
-   Begin a multi-day mini-project by creating an ethical AI business concept.

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
-   A `.env` file setup guide or environment variable instructions

**Standards:**
--------------

-   Computational Thinking: Analyze the impacts of computing systems on people, communities, and society.
-   Computer Science Practices: Evaluate how computing tools can introduce bias or unequal outcomes.
-   Digital Literacy: Use emerging technology ethically and responsibly.
-   Career Readiness: Apply collaboration, critical thinking, and communication to real-world innovation.
-   Entrepreneurship and Innovation: Design products that create value while considering user trust and safety.

**Lesson Activity:**
--------------------

### 1\. **Introduction (Time: 25 minutes)**

-   **Objective:** Energize Geniuses, activate curiosity, and introduce the idea that Applied AI is about building useful and responsible products for the real world.
-   Start with a fun icebreaker called **"Would You Trust This AI?"**
-   This should be the first thing and the highest-energy part of the lesson.

#### **Icebreaker Option A: Physical Movement**

-   Label one side of the room **"Trust It"** and the other **"Don't Trust It."**
-   Read AI scenarios out loud and have Geniuses move to a side quickly.
-   Example scenarios:
    -   An AI helps you choose what shoes to buy.
    -   An AI gives feedback on your resume.
    -   An AI decides whether you get hired.
    -   An AI helps an elder in your family learn how to use a phone.
    -   An AI approves or denies a loan.
    -   An AI suggests which students need discipline support.
    -   An AI plans your workout for the week.
-   After each one, ask a few Geniuses:
    -   Why did you choose that side?
    -   What would make you trust it more?
    -   What would make it dangerous?

#### **Icebreaker Option B: Digital Poll**

-   Use Mentimeter, Slido, or a quick polling site.
-   Let Geniuses vote live on trust levels for each scenario.
-   Show the class results and discuss patterns.

#### **Transition**

-   Say:
    -   "Applied AI is not just about making cool tools. It is about making useful tools people can trust."
-   Ask:
    -   Where have you already seen AI in real life?
    -   What makes one AI use feel exciting and another feel risky?

### 2\. **Direct Instruction (Time: 55 minutes)**

-   **Objective:** Build core knowledge around Applied AI, responsible AI, and ethical product design in a way that is discussion-based and business-centered.
-   Use slides to guide the lecture and keep it interactive.

#### **Suggested Slide Flow**

-   **Slide 1: What Is Applied AI?**
    -   Applied AI means using AI to solve real-world business and community problems.
    -   It is not just research. It is product, service, workflow, automation, and customer impact.
-   **Slide 2: Where Applied AI Shows Up**
    -   Customer support
    -   Recommendation systems
    -   Tutoring tools
    -   Scheduling assistants
    -   Content generation
    -   Risk detection
    -   Search and knowledge assistants
-   **Slide 3: AI in Business Means Decisions at Scale**
    -   AI can sort, rank, recommend, generate, predict, and automate.
    -   Businesses use AI to save time, personalize experiences, reduce costs, and create new value.
-   **Slide 4: Just Because You Can Build It Does Not Mean You Should**
    -   Product power must be balanced with human impact.
-   **Slide 5: Responsible AI Core Concepts**
    -   Fairness
    -   Bias
    -   Privacy
    -   Transparency
    -   Accountability
    -   Safety
    -   Human oversight
-   **Slide 6: Real Risks of AI Products**
    -   Biased hiring tools
    -   Facial recognition problems
    -   False or harmful recommendations
    -   Over-automation
    -   Misuse of personal data
-   **Slide 7: Responsible AI Is Also Good Business**
    -   Trust helps adoption
    -   Trust helps retention
    -   Trust helps reputation
    -   Responsible design reduces harm and product failure
-   **Slide 8: What Questions Should Builders Ask?**
    -   Who is this helping?
    -   Who could be harmed?
    -   What data is being used?
    -   Who checks the AI when it is wrong?
    -   How will users understand what the AI is doing?
-   **Slide 9: Applied AI Today with APIs**
    -   Businesses do not always train their own models.
    -   Many businesses build with APIs from companies like OpenAI.
    -   This means product design, prompting, safety, and user experience matter a lot.
-   **Slide 10: This Week's Build Path**
    -   Geniuses will begin designing an AI business idea that is useful, ethical, and realistic.

#### **Discussion Questions**

-   What makes an AI product feel trustworthy?
-   Can an AI product be useful and still harmful?
-   Why might businesses ignore ethics when moving fast?
-   How can ethics become a competitive advantage?
-   What responsibilities do builders have when using someone else's AI model through an API?

#### **Reflection Prompt**

-   Have Geniuses write for 3 minutes:
    -   "Describe one AI use case you think could really help people and one AI use case that worries you. Why?"

### 3\. **Guided Practice (Time: 50 minutes)**

-   **Objective:** Help Geniuses build a simple OpenAI-powered Python tool in VS Code that reviews an AI business idea for ethical concerns and responsible design choices.
-   Explain that today they are not training a model from scratch. They are learning an important real-world Applied AI skill:
    -   building a product on top of an AI API.

#### **Guided Practice Build**

Create a project called `responsible-ai-reviewer`.

#### **Project Goal**

Build a Python script that:

-   Takes in an AI business idea
-   Sends the idea to the OpenAI API
-   Asks the model to identify risks, affected users, and responsible design suggestions
-   Prints the results clearly

#### **Setup Steps**

1.  Open VS Code.
2.  Create a new folder called `responsible-ai-reviewer`.
3.  Open the terminal in VS Code.
4.  Install dependencies:

```
npm init -y
npm install dotenv
```
-   Explain that since this day is Python-based, the class will also install the Python OpenAI package:
```
pip install openai python-dotenv
```
1.  Create a `.env` file:
```
OPENAI_API_KEY=your_key_here
```
1.  Create a file called `ai_ethics_reviewer.py`

#### **Sample Code**
```
# ai_ethics_reviewer.py
# Applied AI Week 1 Day 1
# This script uses the OpenAI API to review an AI business idea
# for possible ethical risks and responsible design suggestions.

import os
from dotenv import load_dotenv
from openai import OpenAI

# Load environment variables from the .env file

load_dotenv()

# Create the OpenAI client using the API key

client = OpenAI(api_key=os.getenv("OPENAI_API_KEY"))
print("Welcome to the Responsible AI Reviewer\n")

# Ask the user for an AI idea

idea_name = input("What is the name of your AI idea? ")
idea_description = input("Describe your AI idea in 2-3 sentences: ")

# Create a prompt for the model

prompt = f"""
You are a responsible AI product advisor.

A Genius is building this AI business idea:

Idea Name: {idea_name}
Description: {idea_description}

Please respond in this format:
1. Main benefit
2. One possible risk
3. Who could be harmed if it fails
4. One responsible design recommendation
5. A trust score from 1 to 10 with a short explanation

Keep your response clear and student-friendly.

# Send the request to the OpenAI API
response = client.responses.create(
    model="gpt-4.1-mini",
    input=prompt
)

# Print the model's feedback
print("\n--- Responsible AI Review ---")
print(response.output_text)
```

#### **Guided Practice Teaching Points**

-   What is an API?
-   Why do businesses often build with APIs instead of training models?
-   Why should we protect API keys?
-   Why is the prompt part of the product design?
-   What happens if the model gives incomplete or weak answers?

#### **Guided Practice Discussion**

-   What did the AI do well?
-   What did it miss?
-   Would you trust this tool by itself?
-   Why should a human still review important decisions?

### 4\. **Independent Practice (Time: 35 minutes)**

-   **Objective:** Geniuses independently begin their mini-project by designing an ethical AI business concept and using the API reviewer to think through risk and trust.
-   Geniuses start a mini-project that will build through Day 4.

#### **Mini-Project Title**

**Ethical AI Business Starter**

#### **Independent Task**

Each Genius creates a Python file for their own AI concept and does the following:

-   Names the product
-   Defines the target user
-   Explains the problem solved
-   Writes a short business value statement
-   Uses the OpenAI API to review the idea
-   Adds their own reflection on what should change to make the product more responsible

#### **Required Deliverables**

-   A working Python file
-   A product concept with:
    -   Product name
    -   Target user
    -   Problem solved
    -   Business value
    -   One major risk
    -   One responsible design decision
-   A short written reflection:
    -   What responsibility do I have as the builder?
    -   What would make users trust this product?

#### **Independent Practice Starter Code**
```
# my_ai_business_idea.py
# Day 1 independent practice
# This script stores an AI product concept and asks the OpenAI API
# for responsible AI feedback.

import os
from dotenv import load_dotenv
from openai import OpenAI

load_dotenv()
client = OpenAI(api_key=os.getenv("OPENAI_API_KEY"))

product_name = "CareerPath AI"
target_user = "High school students exploring jobs and internships"
problem_solved = "Helps Geniuses practice interview questions and discover career paths"
business_value = "Saves time for mentors and gives students faster access to support"

prompt = f"""
Review this AI product idea.

Product Name: {product_name}
Target User: {target_user}
Problem Solved: {problem_solved}
Business Value: {business_value}

Please give:
1. One major strength
2. One ethical risk
3. One group that could be impacted negatively
4. One way to make the product more responsible

Use short, clear language.
"""

response = client.responses.create(
    model="gpt-4.1-mini",
    input=prompt
)

print("My Applied AI Business Idea\n")
print(f"Product Name: {product_name}")
print(f"Target User: {target_user}")
print(f"Problem Solved: {problem_solved}")
print(f"Business Value: {business_value}")

print("\n--- API Review ---")
print(response.output_text)
```

### 5\. **Closure (Time: 15 minutes)**

-   **Objective:** Reinforce the idea that strong Applied AI builders think about both usefulness and responsibility.
-   Bring the class together for a final share-out.
-   Ask 3--5 Geniuses to share:
    -   Their product name
    -   The problem it solves
    -   One ethical risk they identified
    -   One responsible design improvement
-   Lead a closing discussion:
    -   What surprised you today about building with AI?
    -   What is the difference between a cool AI idea and a trustworthy AI product?
    -   Why should business builders care about ethics early instead of later?
-   Preview next lesson:
    -   Geniuses will move from ethics and opportunity into stronger problem definition and customer-centered thinking.

**Assessment:**
---------------

Student learning will be assessed through:

-   Participation in the icebreaker and discussion
-   Responses during lecture and reflection
-   Completion of the guided OpenAI API build in VS Code
-   Completion of an independent AI business concept with responsible AI analysis
-   Final reflection and share-out

### **Exit Ticket**

1.  What is Applied AI?
2.  Name one ethical risk that can appear in an AI product.
3.  Why should a builder think about trust before launching?

**Extra Activities:**
---------------------

-   Geniuses who finish early can improve their script by asking the model for:
    -   a privacy warning
    -   a fairness warning
    -   a safer product version
-   Add user input instead of hard-coded values
-   Ask the model to return results in JSON and print each part cleanly
-   Create a version that compares two AI business ideas and identifies which one is more trustworthy
-   Add error handling for missing API keys

**Reflection / Takeaways:**
---------------------------

This lesson is strongest when Geniuses leave seeing that Applied AI is not just about coding or using trendy tools. It is about building products that create value in the real world while protecting people from harm. The OpenAI API component makes the lesson feel modern and real, while the responsible AI framing makes it clear that builders still have to think critically. Day 1 sets the tone for the rest of the summer by showing that the best builders are not only creative, but accountable.

**Facilitator Notes**
---------------------

-   Keep saying **Geniuses** consistently in discussion, prompts, and examples.
-   Emphasize that APIs make AI accessible, but they do not remove responsibility.
-   Keep the coding accessible and explain each line.
-   If API setup becomes a blocker for some Geniuses, pair them up or provide a demo key/projected walkthrough.
-   Reinforce that prompt design is product design.

**Day 1 Mini-Project Connection**
---------------------------------

By the end of Day 1, each Genius should have:

-   A named AI business idea
-   A target user
-   A problem worth solving
-   A business value statement
-   At least one ethical risk
-   At least one responsible design choice
-   A working OpenAI-powered Python reviewer or a working guided version with support
