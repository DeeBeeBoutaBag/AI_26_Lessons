<img src="https://github.com/Hgp-GeniusLabs/Curriculum/blob/10734f2c827128dde773ea4f266d154d46977866/Org-Wide/Assets/hgp_logo_original.png" width="150"/>

Lesson Plan: Applied AI Week 1, Day 5 --- Flex Day, Product Polish, and Applied AI Showcase
=========================================================================================

**Duration:**
-------------

3 hours

**Lesson Overview:**
--------------------

Day 5 is a flex day focused on strengthening, extending, and showcasing the Applied AI products Geniuses have been building all week. By this point, Geniuses have explored responsible AI, clarified user problems, designed workflows, and improved product prompts and behavior. Today they use that foundation to make their products more complete, more polished, and more realistic. Geniuses choose from a menu of meaningful upgrades such as improving the interface, adding more user input, increasing trust and safety features, structuring outputs more clearly, or making their code more dynamic. During guided practice, the class builds a reusable Python improvement pattern that helps turn a basic prototype into a stronger product. During independent practice, each Genius applies selected improvements to their own project and prepares a short presentation or demo. The lesson ends with a showcase and reflection on what it means to build AI products that are useful, thoughtful, and responsible.

**Objectives:**
---------------

-   Reflect on how an Applied AI product improves through iteration.
-   Identify meaningful ways to strengthen a prototype beyond the first working version.
-   Improve an AI product by adding features, polish, structure, safety, or flexibility.
-   Practice explaining a product's value, workflow, and responsible design choices.
-   Build on an existing Python OpenAI project in VS Code by making targeted product improvements.
-   Present a more complete Applied AI prototype to peers.

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
-   Existing project files from Days 1--4
-   `.env` file with OpenAI API key configured
-   Optional presentation rubric or showcase checklist

**Standards:**
--------------

-   Computational Thinking: Refine and improve a system through testing and iteration.
-   Computer Science Practices: Debug, revise, and strengthen computational solutions.
-   Digital Literacy: Evaluate whether a digital product is useful, understandable, and trustworthy.
-   Career Readiness: Communicate product ideas clearly and respond to feedback.
-   Entrepreneurship and Innovation: Improve a product based on usability, trust, and value.

**Lesson Activity:**
--------------------

### 1. **Introduction (Time: 20 minutes)**

-   **Objective:** Energize Geniuses and shift the class into builder mode by showing that strong products are improved through iteration, not born perfect.
-   Start with an icebreaker called **"Upgrade or Delete?"**
-   This should be the first and most energetic part of the lesson.

#### **Icebreaker Option A: Physical Movement**

-   Label one side of the room **"Upgrade It"** and the other side **"Delete It."**
-   Read product feature ideas aloud and have Geniuses move quickly.
-   Example prompts:
    -   A chatbot that remembers your last conversation
    -   An AI career tool that gives one career and no explanation
    -   An AI study helper that shows steps and lets you edit the plan
    -   An AI app that gives answers but never explains why
    -   A product that warns users when confidence is low
    -   An AI product that feels smart but confusing
    -   An AI tool that asks better follow-up questions before answering
-   After each one, ask:
    -   What makes this worth upgrading?
    -   What makes this weak enough to delete?
    -   What would make this more trustworthy?
    -   What would make this more useful?

#### **Icebreaker Option B: Website Activity**

-   Use Mentimeter, Slido, or a quick vote board.
-   Present features or product decisions and have Geniuses vote:
    -   Keep it
    -   Upgrade it
    -   Delete it
-   Discuss why some features add real value and others do not.

#### **Transition**

-   Say:
    -   "A first version proves the idea. A polished version proves the builder."
-   Ask:
    -   What makes a prototype feel unfinished?
    -   What makes a product feel real?

### 2\. **Direct Instruction (Time: 40 minutes)**

-   **Objective:** Help Geniuses understand how product iteration works and identify specific ways to improve their Applied AI projects.
-   Use slides to guide the lesson and frame improvement as a normal and important part of building.

#### **Suggested Slide Flow**

-   **Slide 1: Day 5 Focus --- Improve, Extend, Showcase**
    -   Today is about making your product stronger, clearer, and more complete.
-   **Slide 2: What Does Product Polish Mean?**
    -   Better usability
    -   Better clarity
    -   Better trust
    -   Better structure
    -   Better flexibility
    -   Better code quality
-   **Slide 3: Signs a Product Needs Improvement**
    -   The output is too vague
    -   The user cannot control enough
    -   The workflow feels incomplete
    -   The product is hard to understand
    -   The product does not explain limitations
    -   The product only works for one hard-coded example
-   **Slide 4: Ways to Improve an Applied AI Product**
    -   Add user input
    -   Add multiple prompt options
    -   Improve output formatting
    -   Add follow-up questions
    -   Add safety or trust messaging
    -   Add error handling
    -   Add scoring or evaluation
    -   Add multiple use cases
-   **Slide 5: Product Improvement Categories**
    -   **Functionality:** What it can do
    -   **User Experience:** How it feels to use
    -   **Trust and Safety:** How it handles risk and limitations
    -   **Code Quality:** How clean and reusable it is
-   **Slide 6: Strong Builders Iterate on Purpose**
    -   They do not just add random features
    -   They improve what matters most for the user
-   **Slide 7: Showcase Thinking**
    -   Can you explain:
        -   the problem?
        -   the user?
        -   the workflow?
        -   why AI is the right fit?
        -   what makes your product responsible?
-   **Slide 8: Build Priorities**
    -   Fix weak areas first
    -   Improve the core experience
    -   Do not try to add everything
-   **Slide 9: Today's Flex Menu**
    -   Choose 2--3 meaningful improvements
    -   Build them well
    -   Prepare to demo
-   **Slide 10: Applied AI Builders Finish Strong**
    -   A polished prototype shows product thinking, not just code completion

#### **Discussion Questions**

-   What part of your product still feels weakest?
-   What would make your product feel more useful for a real user?
-   What would make your product more trustworthy?
-   What is one improvement that adds real value instead of just complexity?
-   How do you know when a product is ready to show?

#### **Reflection Prompt**

-   Have Geniuses write for 4 minutes:
    -   "What is the most important improvement your product still needs, and why?"

### 3. **Guided Practice (Time: 40 minutes)**

-   **Objective:** Help Geniuses learn a reusable improvement pattern they can apply to their own product builds.
-   Explain that today's code-along is not a brand new project. It is a product upgrade pattern.
-   The class will create `product_upgrade_demo.py`.

#### **Guided Practice Build**

Use an existing project folder or create a new file called `product_upgrade_demo.py`.

#### **Project Goal**

Build a Python script that improves a basic product by:

-   Taking real user input
-   Sending that input to the OpenAI API
-   Using a stronger structured prompt
-   Printing a cleaner response
-   Including a trust or limitation note
-   Adding basic error handling

#### **Setup Steps**

1.  Open the project in VS Code.
2.  Confirm `.env` is configured.
3.  Confirm required packages are installed:
```
pip install openai python-dotenv
```
1.  Create a file called `product_upgrade_demo.py`

#### **Sample Code**
```
# product_upgrade_demo.py
# Applied AI Week 1 Day 5
# This script demonstrates how to upgrade a basic Applied AI product
# by adding user input, stronger structure, and a trust-building note.

import os
from dotenv import load_dotenv
from openai import OpenAI

# Load environment variables from the .env file
load_dotenv()

# Get the API key from the environment
api_key = os.getenv("OPENAI_API_KEY")

# Check that the API key exists before creating the client
if not api_key:
    print("Error: OPENAI_API_KEY was not found. Check your .env file.")
    raise SystemExit

# Create the OpenAI client
client = OpenAI(api_key=api_key)

print("Welcome to the Product Upgrade Demo\n")

# Ask the user for real input
user_goal = input("What do you want help with today? ")
user_context = input("Give a little context about your situation: ")

# Build a stronger structured prompt
prompt = f"""
You are a helpful and responsible AI assistant.

A Genius is using this product.

User Goal: {user_goal}
User Context: {user_context}

Please respond in this format:
1. Best Next Step
2. 2-3 Helpful Suggestions
3. One thing the user should double-check
4. A short encouraging closing line

Keep the response practical, clear, and supportive.
Do not pretend to know information you do not have.
"""

try:
    # Send the request to the OpenAI API
    response = client.responses.create(
        model="gpt-4.1-mini",
        input=prompt
    )

    # Print the result clearly
    print("\n--- Improved Product Output ---")
    print(response.output_text)

    # Add a trust-building note
    print("\n--- Product Note ---")
    print("This tool gives guidance based on the information you entered. Always review important decisions carefully.")

except Exception as error:
    print("\nSomething went wrong while calling the API.")
    print(f"Error details: {error}")
```
#### **Guided Practice Teaching Points**

-   Why real user input makes a product feel more alive
-   Why structure improves output quality
-   Why limitation notes help build trust
-   Why error handling matters in real products
-   Why product improvement should focus on user value, not just adding more code

#### **Guided Practice Discussion**

-   What made this version stronger than a hard-coded prototype?
-   What part of the upgrade would matter most to a real user?
-   How did the limitation note change the product experience?
-   What other improvements could be reused across many products?

### 4. **Independent Practice (Time: 60 minutes)**

-   **Objective:** Give Geniuses time to make meaningful improvements to their own projects and prepare for a short showcase.
-   Geniuses continue and strengthen their mini-projects from Days 1--4.

#### **Mini-Project Title**

**Ethical AI Business Starter --- Day 5 Flex Build and Showcase Prep**

#### **Independent Task**

Each Genius chooses **2--3 meaningful upgrades** to apply to their product.

#### **Improvement Menu**

Geniuses can choose from the following:

-   Add real user input instead of hard-coded content
-   Improve the main prompt with better structure
-   Add output formatting with sections or steps
-   Add a trust or safety note
-   Add a warning or human review note
-   Add basic error handling
-   Add a second feature or use case
-   Add a follow-up question before the final response
-   Add a scoring system or recommendation rating
-   Refactor the code into functions
-   Return structured data and print it clearly
-   Create a stronger demo scenario for their product

#### **Required Deliverables**

-   A working improved Python file
-   At least 2 meaningful product upgrades
-   A short product summary with:
    -   Product name
    -   Target user
    -   Problem solved
    -   Main workflow
    -   Key prompt design choice
    -   One trust or safety feature
    -   Two upgrades made today
-   A short presentation or demo plan

#### **Showcase Prep Prompt**

Ask Geniuses to prepare a 1--2 minute share-out that answers:

-   What is your product called?
-   Who is it for?
-   What problem does it solve?
-   Why is AI a good fit?
-   What makes your product trustworthy?
-   What did you improve today?

#### **Facilitator Support Moves**

-   Help Geniuses choose upgrades that actually improve the experience
-   Push them to avoid shallow add-ons that do not matter
-   Ask:
    -   What is your weakest part right now?
    -   What would matter most to the user?
    -   What would make your demo stronger?
-   Encourage Geniuses to test their product more than once

### 5. **Closure (Time: 20 minutes)**

-   **Objective:** Celebrate the week's work, reinforce growth, and help Geniuses practice explaining their product clearly.
-   Bring the class together for a showcase.
-   Invite Geniuses to present individually or in small groups.
-   Each Genius should share:
    -   Their product name
    -   Their target user
    -   The problem solved
    -   One important workflow or prompt decision
    -   One trust or safety feature
    -   Two improvements they made today
-   After each share, invite quick audience feedback:
    -   What feels strongest?
    -   What would you want to see next?
-   Lead a final reflection discussion:
    -   What did you learn this week about building AI products?
    -   What part of the process was hardest?
    -   What part felt most exciting?
    -   How did ethics, product thinking, and AI connect across the week?

**Assessment:**
---------------

Student learning will be assessed through:

-   Participation in the icebreaker and discussion
-   Reflection responses during direct instruction
-   Completion of the guided product upgrade build in VS Code
-   Completion of at least 2 meaningful improvements to the independent project
-   Final product showcase and explanation
-   End-of-week reflection on growth and product thinking

### **Exit Ticket**

1.  What is one improvement that made your product stronger today?
2.  What makes your product more trustworthy now than it was on Day 1?
3.  What is one thing you would still improve next?

**Extra Activities:**
---------------------

-   Geniuses who finish early can turn repeated code into functions
-   Add multiple user scenarios and test outputs
-   Compare outputs before and after upgrades
-   Add a menu system so the user can choose different product features
-   Create a second version of the product for another target user
-   Add a basic text file export of the AI output for future review

**Reflection / Takeaways:**
---------------------------

This lesson works best when Geniuses feel ownership over the products they have been building and see that strong innovation comes from revision, not just invention. Day 5 should feel like a studio day where Geniuses make their work stronger, more polished, and more real. The goal is not perfection. The goal is meaningful progress, better thinking, and clearer product choices. By the end of the lesson, Geniuses should see that Applied AI is not just about calling a model. It is about creating something useful, understandable, and responsible for real people.

**Facilitator Notes**
---------------------

-   Keep using **Geniuses** consistently in prompts, examples, and discussion.
-   Let the flex time feel open, but keep Geniuses focused on meaningful upgrades.
-   Encourage quality over quantity.
-   Help Geniuses prepare to explain not just what they built, but why they built it that way.
-   Reinforce that polishing a product is part of real-world product development.

**Day 5 Week 1 Wrap-Up**
------------------------

By the end of Day 5, each Genius should have:

-   A defined Applied AI product concept
-   A clear target user
-   A real problem being solved
-   A product workflow
-   A main product prompt
-   A product behavior style
-   At least one trust or safety feature
-   At least 2 meaningful upgrades made on flex day
-   A more complete OpenAI-powered Python prototype
-   A short presentation or demo explanation
