<img src="https://github.com/Hgp-GeniusLabs/Curriculum/blob/10734f2c827128dde773ea4f266d154d46977866/Org-Wide/Assets/hgp_logo_original.png" width="150"/>

Lesson Plan: AI Systems Week 5, Day 3 --- Data Use, Trust Boundaries, and AI Policy Design
========================================================================================

**Duration:**
-------------

3 hours

**Lesson Overview:**
--------------------

On Day 3, Geniuses focus on one of the most important parts of building serious AI software: **data use, trust boundaries, and AI policy design**. After defining their capstone vision and writing documentation, Geniuses now turn to the question of responsibility at the system level. This lesson helps them define what data their product uses, what data it should avoid using, what users should and should not trust, and what guardrails should shape system behavior.

The lesson emphasizes that every AI capstone needs more than features and technical workflows. It also needs a clear stance on **privacy, consent, limitations, review, synthetic output, and risk**. Geniuses learn that strong builders do not wait until the end to think about trust. They design for it early. During guided practice, the class builds a Python-based policy and trust organizer that helps structure product data use and AI guardrails. During independent practice, each Genius creates a `DATA_POLICY.md` and either an `AI_POLICY.md` or `TRUST_AND_SAFETY.md` for their own capstone. By the end of the lesson, Geniuses should understand that trust is not a bonus feature. It is part of real AI product design.

**Objectives:**
---------------

-   Explain why AI software needs clear data and trust policies.
-   Identify what kinds of data a capstone product uses and what kinds it should avoid or handle carefully.
-   Define trust boundaries for an AI system, including what users should still review.
-   Explain the purpose of an AI policy or trust and safety document.
-   Build a Python-based trust and policy organizer in VS Code.
-   Create a `DATA_POLICY.md` and an `AI_POLICY.md` or `TRUST_AND_SAFETY.md` for a capstone product.
-   Reflect on how responsible design improves product quality, safety, and credibility.

**Materials:**
--------------

-   Laptops for all Geniuses
-   VS Code installed
-   Python installed and working
-   Internet access
-   Projector or display
-   Whiteboard and markers
-   Slide deck for lecture and discussion
-   Reflection journal or digital notes
-   Terminal access in VS Code
-   Existing capstone concept work from Week 5 Days 1--2
-   Starter folder for Python files
-   Markdown preview in VS Code

**Standards:**
--------------

-   Computational Thinking: Define system boundaries, risks, and safe operating conditions for AI software.
-   Computer Science Practices: Design AI systems with clear rules for data use, review, and limitations.
-   Technical Communication: Write clear policies that explain how a product handles data, outputs, and risk.
-   Digital Literacy: Evaluate privacy, trust, fairness, and responsible AI practices in software systems.
-   Career Readiness: Practice policy thinking, professional documentation, and principled decision-making.
-   Technical Foundations: Explain how data and trust policies support responsible AI product design.

**Lesson Activity:**
--------------------

### 1. **Introduction (Time: 25 minutes)**

-   **Objective:** Energize Geniuses and introduce the idea that strong AI systems need rules about what they use, what they do, and what users should trust.
-   Start with a fun icebreaker called **"Should the AI Be Allowed to Do That?"**
-   This should be the first thing and the most fun thing to wake Geniuses up and get them ready for the lesson.

#### **Icebreaker Option A: Physical Movement**

-   Label one side of the room **"Allowed"** and the other side **"Needs Guardrails."**
-   Read scenarios aloud and have Geniuses move to the side that best matches.
-   Example prompts:
    -   A study support agent summarizes homework notes
    -   A vision agent gives feedback on a flyer design
    -   A voice agent gives final health advice with no disclaimer
    -   A sports analytics tool gives training insight with a note for coach review
    -   An image generator creates promotional visuals and clearly labels them as AI-generated
    -   A student support agent stores personal conversations forever without explanation
    -   An agent uses a user's photo to generate content without clear consent
    -   A multimodal agent says it is "definitely correct" about a blurry image
-   After each round, ask:
    -   What makes this acceptable or risky?
    -   What kind of data is involved?
    -   What trust problem shows up here?
    -   What guardrail would make the system stronger?

#### **Icebreaker Option B: Policy Sort**

-   Put scenarios on the board and ask Geniuses to sort them into:
    -   okay as is
    -   needs a warning
    -   needs review
    -   should not be allowed
-   Use the activity to introduce the idea that products need clear rules.

#### **Transition**

-   Say:
    -   "If your AI system can use data, speak confidently, inspect images, or generate content, it needs policies. Trust has to be designed."
-   Ask:
    -   What should your product be allowed to do?
    -   What should it never pretend to know or handle alone?

### 2. **Direct Instruction (Time: 50 minutes)**

-   **Objective:** Help Geniuses understand data policies, trust boundaries, and AI policy design as core parts of product readiness.
-   Use slides to guide instruction and keep it interactive.

#### **Suggested Slide Flow**

-   **Slide 1: Why Data and Trust Policies Matter**
    -   AI systems use data, produce outputs, and influence decisions
    -   Builders need to define what the system uses, what it does, and where its limits are
-   **Slide 2: What Is a Data Policy?**
    -   A data policy explains:
        -   what data the product uses
        -   where it comes from
        -   what is stored or not stored
        -   what needs consent
        -   what should be handled carefully
-   **Slide 3: What Is an AI Policy or Trust Policy?**
    -   A trust or AI policy explains:
        -   what the system should do
        -   what it should not do
        -   when users should review outputs
        -   where caution is needed
        -   what risks are acknowledged
-   **Slide 4: Common Data Questions**
    -   What user input is collected?
    -   Is any visual or audio data used?
    -   Is anything stored?
    -   What should require consent?
    -   What should be avoided entirely?
-   **Slide 5: Common Trust Questions**
    -   What outputs are synthetic?
    -   What should the user double-check?
    -   Where can the AI be wrong?
    -   What should never be treated as final truth?
    -   When should a human stay involved?
-   **Slide 6: Example AI Policy Areas**
    -   confidence and uncertainty
    -   high-stakes limits
    -   review before public use
    -   synthetic image labeling
    -   privacy and consent
    -   bias and fairness awareness
    -   no deceptive output
-   **Slide 7: Strong Policy Language**
    -   clear
    -   honest
    -   specific
    -   realistic
    -   easy to understand
    -   connected to the actual product
-   **Slide 8: Weak Policy Language**
    -   vague
    -   performative
    -   generic
    -   disconnected from what the product really does
-   **Slide 9: Capstone Trust Boundaries**
    -   what the product helps with
    -   what the product does not decide
    -   what the user should still review
    -   what the AI should never claim
-   **Slide 10: Week 5 Direction**
    -   Geniuses are preparing the full capstone package: trust docs, prototype plans, and pitch materials

#### **Discussion Questions**

-   Why does every AI capstone need a data or trust policy?
-   What kinds of user data should be handled carefully?
-   What should AI products say clearly about their own limits?
-   Why is it dangerous for an AI system to sound too certain?
-   What makes a trust policy actually useful?

#### **Reflection Prompt**

-   Have Geniuses write for 4 minutes:
    -   "What is one thing your capstone should help with, and one thing your capstone should never pretend to handle alone?"

### 3. **Guided Practice (Time: 50 minutes)**

-   **Objective:** Help Geniuses build a Python-based trust and policy organizer, then use it to begin drafting policy documents.
-   Explain that today's code-along is about structuring policy thinking clearly.
-   The class will create `policy_builder.py`.

#### **Guided Practice Build**

Create a folder called `capstone-policy-builder`.

#### **Project Goal**

Build a Python program that:

-   asks the user what data the product uses
-   asks what outputs should be reviewed
-   asks what the system should not do
-   asks what trust concern matters most
-   prints a structured policy summary

#### **Setup Steps**

1.  Open VS Code.
2.  Create a folder called `capstone-policy-builder`.
3.  Create a file called `policy_builder.py`.
4.  Create two markdown files:
    -   `DATA_POLICY.md`
    -   `AI_POLICY.md`
5.  Run the Python file in the terminal and use the results to draft the docs.

#### **Sample Code**
```
# policy_builder.py
# AI Systems Week 5 Day 3
# This program helps Geniuses organize capstone data and trust policies.

print("Welcome to the Capstone Policy Builder\n")

project_name = input("Project name: ")
data_used = input("What kinds of data does the product use? ")
data_limit = input("What data should be avoided or handled carefully? ")
review_needed = input("What outputs should users still review? ")
system_limit = input("What should the AI system never pretend to do alone? ")
trust_concern = input("What is the biggest trust or safety concern? ")

print("\n--- Policy Summary ---")
print(f"Project Name: {project_name}")
print(f"Data Used: {data_used}")
print(f"Data Limit: {data_limit}")
print(f"Review Needed: {review_needed}")
print(f"System Limit: {system_limit}")
print(f"Trust Concern: {trust_concern}")

print("\n--- Reflection ---")
print("What should users know before trusting this system?")
print("What should the product clearly warn about?")
print("What policy would make this project more responsible?")
```
#### **Sample `DATA_POLICY.md`**
```
# Data Policy: StudyLens AI

## Purpose
This document explains what data StudyLens AI uses and how that data should be handled responsibly.

## Data Used
- User-entered text prompts
- Image uploads such as worksheets, diagrams, or classroom handouts
- Optional user goal or task description

## Data Use Purpose
This data is used to help the system understand academic materials and provide structured support.

## Data That Requires Extra Care
- Personal student work
- Images that may include names or identifying information
- Sensitive academic or personal content

## Data Limits
- The system should avoid collecting unnecessary personal information
- Users should be informed before uploading images with sensitive content
- The product should not pretend that uploaded data is private unless that privacy is actually guaranteed in the real implementation

## User Awareness
Users should know that uploaded content is being used to generate AI-supported outputs and should avoid sharing unnecessary sensitive information.
```
#### **Sample `AI_POLICY.md`**
```
# AI Policy: StudyLens AI

## Purpose
This document explains what the AI system should do, what it should not do, and what users should still review themselves.

## What the AI Helps With
- Explaining worksheets and diagrams
- Summarizing visible academic content
- Suggesting next steps for studying

## What the AI Should Not Pretend to Do
- Guarantee full correctness on every worksheet or diagram
- Replace teacher instruction
- Act like it understands unclear or incomplete visuals perfectly

## Review Required
Users should still review:
- Important academic answers
- Complex diagrams or unclear images
- Any explanation that seems uncertain or incomplete

## Trust Boundary
The AI should be presented as a support tool, not a final academic authority.

## Output Limits
- The AI should avoid sounding overly certain
- The AI should clearly indicate uncertainty when image quality is weak
- Spoken or generated outputs should still encourage user review
```
#### **Guided Practice Teaching Points**

-   Why policies should match the actual product
-   Why user data needs clear handling rules
-   Why trust boundaries should be easy to understand
-   Why "the AI helps with" and "the AI should not do" are both essential
-   Why policy writing is part of technical maturity

#### **Guided Practice Discussion**

-   Which policy section feels most important?
-   What kinds of data need the most care?
-   Why should systems clearly explain what they do not know?
-   What makes a policy feel real instead of fake?

### 4. **Independent Practice (Time: 35 minutes)**

-   **Objective:** Geniuses independently create policy files for their own capstone product.
-   This continues the Week 5 capstone launch package.

#### **Mini-Project Title**

**Capstone Launch Package --- Day 3 Data and Trust Policies**

#### **Independent Task**

Each Genius creates:

-   `DATA_POLICY.md`
-   either `AI_POLICY.md` or `TRUST_AND_SAFETY.md`

Their files must explain:

-   what data the product uses
-   what data needs caution or should be limited
-   what the AI helps with
-   what the AI should not pretend to do
-   what users should still review
-   what the biggest trust concern is
-   what responsible design boundary matters most

#### **Required Deliverables**

-   A working Python file called `my_policy_builder.py`
-   A completed `DATA_POLICY.md`
-   A completed `AI_POLICY.md` or `TRUST_AND_SAFETY.md`
-   Policy docs that include:
    -   data use
    -   data limits
    -   trust boundary
    -   user review needs
    -   system limitations
    -   responsible design notes
-   A short written reflection:
    -   What trust issue matters most in your capstone?
    -   What data should your product be careful with?
    -   What should users never trust blindly?

#### **Independent Practice Starter Code**
```
# my_policy_builder.py
# Week 5 Day 3 independent practice
# This program prints a capstone policy summary.

print("My Capstone Policy Summary\n")

project_name = "EventGuide AI"
data_used = "Flyer drafts, event planning visuals, user text prompts, and generated image prompts"
data_limit = "The system should avoid unnecessary personal data and should treat public-facing visuals carefully"
review_needed = "Generated visuals, spoken guidance, and important planning suggestions should all be reviewed by a human"
system_limit = "The AI should not pretend to know every event detail or make final public-facing decisions alone"
trust_concern = "The system could create polished but misleading outputs that feel more certain than they should"

print(f"Project Name: {project_name}")
print(f"Data Used: {data_used}")
print(f"Data Limit: {data_limit}")
print(f"Review Needed: {review_needed}")
print(f"System Limit: {system_limit}")
print(f"Trust Concern: {trust_concern}")
```
#### **Facilitator Support Moves**

-   Help Geniuses make their policies specific to their actual product
-   Ask:
    -   What user data really enters the system?
    -   What outputs could be overtrusted?
    -   What should the AI clearly admit it cannot do alone?
    -   What should the user always review?
-   Encourage honesty and clarity over vague "safe AI" language

### 5. **Closure (Time: 20 minutes)**

-   **Objective:** Reinforce that clear policies make capstones more serious, trustworthy, and ready to build.
-   Bring the class together for a final share-out.
-   Ask 3--5 Geniuses to share:
    -   their project name
    -   one data boundary they included
    -   one AI limitation they documented
    -   one trust concern they are designing around
-   Lead a closing discussion:
    -   What makes a data policy strong?
    -   Why should AI systems clearly state what they cannot do?
    -   How do trust policies improve a capstone?
-   Preview the next lesson:
    -   Geniuses will build prototype plans and capstone build roadmaps so they know exactly what to build first.

**Assessment:**
---------------

Student learning will be assessed through:

-   Participation in the icebreaker and discussion
-   Reflection responses during direct instruction
-   Completion of the guided policy builder
-   Completion of independent `DATA_POLICY.md` and `AI_POLICY.md` or `TRUST_AND_SAFETY.md`
-   Final share-out and explanation of product trust boundaries

### **Exit Ticket**

1.  What is a data policy?
2.  What is one thing an AI policy should explain clearly?
3.  Why should users still review some AI outputs?

**Extra Activities:**
---------------------

-   Geniuses who finish early can:
    -   add a "synthetic media warning" section
    -   add a "when human review is required" checklist
    -   add a "what this product should never store" section
    -   add a "privacy principle" to yesterday's principles file
    -   add a "fairness concern" section
    -   add a "user consent" section
-   Add a "what this AI should never say" section
-   Add a "known trust risks" section
-   Add a "public use warning" section
-   Add a "future safety improvement" section

**Reflection / Takeaways:**
---------------------------

This lesson works best when Geniuses realize that trust is not something you add at the end of an AI project. It is something you define and design early. Day 3 helps them think like real builders by making them decide what their product uses, what it should avoid, what it can help with, and where users should still be careful. By the end of the lesson, Geniuses should feel that their capstone is becoming more real because it now includes boundaries, limits, and trust thinking that serious AI software needs.

**Facilitator Notes**
---------------------

-   Keep using **Geniuses** consistently in examples and discussion.
-   Reinforce that good policy writing is specific, honest, and product-connected.
-   Encourage Geniuses to name what the AI should not do, not only what it can do.
-   Help them connect trust boundaries to real user experience.
-   Remind Geniuses that tomorrow they will create the prototype plan and capstone build roadmap.

**Week 5 Day 3 Mini-Project Connection**
----------------------------------------

By the end of Day 3, each Genius should have:

-   A `DATA_POLICY.md`
-   An `AI_POLICY.md` or `TRUST_AND_SAFETY.md`
-   A clearer understanding of what their capstone uses and what it should limit
-   A documented trust boundary for the AI system
-   Clear review expectations for users
-   A stronger foundation for building responsibly in the capstone phase
