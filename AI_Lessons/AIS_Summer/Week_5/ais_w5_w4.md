<img src="https://github.com/Hgp-GeniusLabs/Curriculum/blob/10734f2c827128dde773ea4f266d154d46977866/Org-Wide/Assets/hgp_logo_original.png" width="150"/>

Lesson Plan: AI Systems Week 5, Day 4 --- Prototype Planning, MVP Scope, and Capstone Build Roadmaps
==================================================================================================

**Duration:**
-------------

3 hours

**Lesson Overview:**
--------------------

On Day 4, Geniuses shift from concept, documentation, and policy into **build planning**. After defining their capstone vision, writing READMEs and technical docs, and creating data and trust policies, Geniuses now focus on the question that matters most before the capstone phase begins: **What are we actually building first?** This lesson is about turning a strong idea into a realistic prototype plan and a focused roadmap for Weeks 6 and 7.

The lesson introduces **MVP thinking** and prototype planning as essential technical product skills. Geniuses learn that strong builders do not try to build everything at once. They identify the core user flow, the most important AI system behavior, and the minimum useful version of the product that can still be demoed and pitched convincingly. During guided practice, the class builds a Python-based prototype planner that helps organize features, priorities, scope, and build order. During independent practice, each Genius creates a `PROTOTYPE_PLAN.md` and a `CAPSTONE_BUILD_PLAN.md` for their own project. By the end of the lesson, Geniuses should know what they are building, what can wait, what the MVP is, and how they will use their capstone weeks effectively.

**Objectives:**
---------------

-   Explain what an MVP is and why it matters in software product development.
-   Distinguish between core features, stretch features, and unnecessary extras.
-   Identify the most important user flow in a capstone AI software project.
-   Create a clear prototype plan for an AI product.
-   Build a Python-based prototype planning tool in VS Code.
-   Create a `PROTOTYPE_PLAN.md` and `CAPSTONE_BUILD_PLAN.md`.
-   Reflect on how realistic scope improves build quality, confidence, and pitch strength.

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
-   Existing Week 5 capstone files
-   Starter folder for Python files
-   Markdown preview in VS Code

**Standards:**
--------------

-   Computational Thinking: Break complex software ideas into essential features, flows, and priorities.
-   Computer Science Practices: Plan a realistic implementation path for an AI system prototype.
-   Technical Communication: Explain what the product will build first and why.
-   Digital Literacy: Evaluate scope, feasibility, and user value in technical product design.
-   Career Readiness: Practice planning, prioritization, decision-making, and product execution.
-   Technical Foundations: Translate an AI software concept into a realistic prototype roadmap.

**Lesson Activity:**
--------------------

### 1. **Introduction (Time: 25 minutes)**

-   **Objective:** Energize Geniuses and introduce the idea that great products are not built by trying to build everything at once.
-   Start with a fun icebreaker called **"Need It Now or Build It Later?"**
-   This should be the first thing and the most fun thing to wake Geniuses up and get them ready for the lesson.

#### **Icebreaker Option A: Physical Movement**

-   Label one side of the room **"MVP Now"** and the other side **"Later Feature."**
-   Read feature ideas aloud and have Geniuses move to the side that best matches whether the feature belongs in the first prototype or later.
-   Example prompts:
    -   A login system with full account profiles
    -   The core image upload feature
    -   Basic AI output for the main use case
    -   Five different voice personalities
    -   A simple text-to-speech output
    -   User analytics dashboard
    -   The main results screen
    -   A full social sharing system
    -   One clean demo-ready user flow
-   After each round, ask:
    -   Why does this belong in the MVP or not?
    -   Does this feature create the core value?
    -   Is this necessary for the demo?
    -   What is flashy but not essential?

#### **Icebreaker Option B: Feature Sort**

-   Put feature ideas on the board.
-   Ask Geniuses to sort them into:
    -   must build
    -   nice to have
    -   not needed yet
-   Discuss how overbuilding can weaken a capstone.

#### **Transition**

-   Say:
    -   "A strong prototype is not the version with the most features. It is the version that proves the idea clearly."
-   Ask:
    -   What is the one thing your product absolutely needs to do?
    -   What could wait until after the first working version?

### 2. **Direct Instruction (Time: 50 minutes)**

-   **Objective:** Help Geniuses understand MVP scope, prototype planning, and capstone execution strategy.
-   Use slides to guide instruction and keep it interactive.

#### **Suggested Slide Flow**

-   **Slide 1: Why Prototype Planning Matters**
    -   Ideas become real when builders decide what to build first
    -   Good planning helps avoid overbuilding, confusion, and unfinished products
-   **Slide 2: What Is an MVP?**
    -   MVP means minimum viable product
    -   It is the smallest version of the product that still proves the value clearly
    -   It should:
        -   solve the core problem
        -   show the main AI behavior
        -   be understandable in a demo
-   **Slide 3: MVP vs Full Vision**
    -   **Full vision:** everything the product may become
    -   **MVP:** what needs to work first
    -   Strong builders know the difference
-   **Slide 4: Core Questions for Scope**
    -   What is the main user flow?
    -   What is the one feature that proves the value?
    -   What AI behavior matters most?
    -   What can be simplified?
    -   What can wait?
-   **Slide 5: Core Features vs Stretch Features**
    -   **Core features:** must exist for the product to make sense
    -   **Stretch features:** would improve it, but are not required for a strong prototype
    -   **Extra features:** may distract or waste time
-   **Slide 6: What a Strong Prototype Plan Includes**
    -   product goal
    -   core user flow
    -   core features
    -   stretch features
    -   AI workflow
    -   what is in scope
    -   what is out of scope
-   **Slide 7: What a Strong Build Plan Includes**
    -   what to build first
    -   what order to build in
    -   what success looks like by the end of Week 6
    -   what success looks like by the end of Week 7
-   **Slide 8: Common Build Mistakes**
    -   too many features
    -   unclear first milestone
    -   no clear MVP
    -   overfocusing on visuals before the workflow works
    -   trying to build everything equally at once
-   **Slide 9: Capstone Readiness**
    -   a good capstone build plan makes pitching easier too
    -   builders should know:
        -   what is already real
        -   what is still planned
        -   what the prototype proves
-   **Slide 10: Week 5 Direction**
    -   tomorrow Geniuses will pitch and present their capstone direction more clearly because they will know exactly what they are building

#### **Discussion Questions**

-   What makes an MVP strong?
-   Why is it dangerous to build too many features at once?
-   What should a capstone prototype prove first?
-   How do you know whether a feature is core or extra?
-   Why does good planning make demos stronger?

#### **Reflection Prompt**

-   Have Geniuses write for 4 minutes:
    -   "What is the one feature or user flow your capstone must get right for the product to make sense?"

### 3. **Guided Practice (Time: 50 minutes)**

-   **Objective:** Help Geniuses build a Python-based prototype planner and use it to organize MVP scope and build order.
-   Explain that today's code-along is about turning the capstone into a realistic build roadmap.
-   The class will create `prototype_planner.py`.

#### **Guided Practice Build**

Create a folder called `prototype-planner`.

#### **Project Goal**

Build a Python program that:

-   asks for the capstone name
-   asks for the core user goal
-   asks for the main AI behavior
-   asks for core features
-   asks for stretch features
-   asks for the first thing to build
-   prints a structured MVP and build summary

#### **Setup Steps**

1.  Open VS Code.
2.  Create a folder called `prototype-planner`.
3.  Create a file called `prototype_planner.py`.
4.  Create two markdown files:
    -   `PROTOTYPE_PLAN.md`
    -   `CAPSTONE_BUILD_PLAN.md`
5.  Run the Python file in the terminal and use the answers to draft both docs.

#### **Sample Code**
```
# prototype_planner.py
# AI Systems Week 5 Day 4
# This program helps Geniuses define MVP scope and capstone build priorities.

print("Welcome to the Prototype Planner\n")

project_name = input("Project name: ")
core_goal = input("What is the main user goal? ")
ai_behavior = input("What is the core AI system behavior? ")
core_features = input("List 2 to 3 core features: ")
stretch_features = input("List 1 to 3 stretch features: ")
first_build = input("What should be built first? ")
success_week6 = input("What should be working by the end of Week 6? ")
success_week7 = input("What should be ready by the end of Week 7? ")

print("\n--- Prototype Planning Summary ---")
print(f"Project Name: {project_name}")
print(f"Core User Goal: {core_goal}")
print(f"Core AI Behavior: {ai_behavior}")
print(f"Core Features: {core_features}")
print(f"Stretch Features: {stretch_features}")
print(f"Build First: {first_build}")
print(f"Week 6 Success: {success_week6}")
print(f"Week 7 Success: {success_week7}")

print("\n--- Reflection ---")
print("What makes this an MVP instead of a full final product?")
print("What feature could wait until later?")
print("What will prove the product's value fastest?")
```
#### **Sample `PROTOTYPE_PLAN.md`**
```
# Prototype Plan: StudyLens AI

## Product Goal
Build a multimodal AI support tool that helps Geniuses understand worksheets and diagrams through visual reasoning and spoken support.

## Core User Flow
1. User uploads or describes a worksheet or diagram
2. The system analyzes the visual content
3. The agent returns key findings and a suggested next step
4. The system can optionally speak the response aloud

## Core Features
- Visual input or image description support
- Structured explanation output
- One helpful next step
- Optional text-to-speech output

## Stretch Features
- Multiple response modes
- Better voice customization
- More polished interface
- Saved session history

## In Scope for MVP
- One strong end-to-end academic support flow
- Clear image-aware reasoning
- Demo-ready spoken output

## Out of Scope for MVP
- Full user account system
- Advanced dashboards
- Complex personalization
- Multiple unrelated modes
```
#### **Sample `CAPSTONE_BUILD_PLAN.md`**
```
# Capstone Build Plan: StudyLens AI

## Build First
Start with the main worksheet explanation flow:
- user input
- image or scene description
- structured explanation
- next step output

## Week 6 Goal
By the end of Week 6:
- the core workflow should run
- the AI output should be usable
- one spoken output mode should work
- the product should be testable

## Week 7 Goal
By the end of Week 7:
- the prototype should be polished enough to demo
- the README and technical docs should be updated
- the trust policy should match the final prototype
- the team should be ready to pitch clearly

## Biggest Risks
- trying to build too many features
- weak image reasoning flow
- unclear output formatting
- not leaving enough time for polish and demo prep

## Build Priority Order
1. Core user flow
2. Useful AI output
3. Output formatting
4. Voice or extra multimodal feature
5. Polish and pitch prep
```
#### **Guided Practice Teaching Points**

-   Why one strong user flow is better than many weak ones
-   Why the AI behavior must be central in the prototype
-   Why stretch features should not distract from the MVP
-   Why Week 6 and Week 7 goals should be different
-   Why good planning makes the final pitch much stronger

#### **Guided Practice Discussion**

-   Which features felt clearly core?
-   Which features felt tempting but unnecessary?
-   What should most teams build first?
-   What makes a prototype demo-ready even if it is not complete?

### 4. **Independent Practice (Time: 35 minutes)**

-   **Objective:** Geniuses independently create a prototype plan and capstone build roadmap for their project.
-   This continues the Week 5 capstone launch package.

#### **Mini-Project Title**

**Capstone Launch Package --- Day 4 Prototype Plan and Build Roadmap**

#### **Independent Task**

Each Genius creates:

-   `PROTOTYPE_PLAN.md`
-   `CAPSTONE_BUILD_PLAN.md`

Their files must define:

-   the product goal
-   the main user flow
-   core features
-   stretch features
-   MVP scope
-   what is out of scope
-   what to build first
-   what success looks like by the end of Week 6
-   what success looks like by the end of Week 7

#### **Required Deliverables**

-   A working Python file called `my_prototype_planner.py`
-   A completed `PROTOTYPE_PLAN.md`
-   A completed `CAPSTONE_BUILD_PLAN.md`
-   Planning docs that include:
    -   MVP definition
    -   user flow
    -   feature priorities
    -   build order
    -   weekly success goals
    -   biggest build risk
-   A short written reflection:
    -   What is your MVP?
    -   What feature is intentionally not in scope yet?
    -   What part of the build plan feels most important?

#### **Independent Practice Starter Code**
```
# my_prototype_planner.py
# Week 5 Day 4 independent practice
# This program prints a simple capstone prototype planning summary.

print("My Prototype Planning Summary\n")

project_name = "EventGuide AI"
core_goal = "Help youth organizers review event visuals, get spoken guidance, and generate new promotional concepts"
ai_behavior = "Multimodal agent with vision, voice, and image generation"
core_features = "Visual review, spoken guidance, structured next-step output"
stretch_features = "Multiple visual styles, extra voice modes, saved project history"
first_build = "The main visual review and next-step feedback workflow"
success_week6 = "A working end-to-end visual review flow with useful AI output"
success_week7 = "A demo-ready multimodal prototype with docs, policy alignment, and pitch readiness"

print(f"Project Name: {project_name}")
print(f"Core Goal: {core_goal}")
print(f"AI Behavior: {ai_behavior}")
print(f"Core Features: {core_features}")
print(f"Stretch Features: {stretch_features}")
print(f"Build First: {first_build}")
print(f"Week 6 Success: {success_week6}")
print(f"Week 7 Success: {success_week7}")
```
#### **Facilitator Support Moves**

-   Help Geniuses cut features that do not prove the product
-   Ask:
    -   What does the user absolutely need first?
    -   What is the cleanest demoable user flow?
    -   What can wait until after the capstone?
    -   What is the biggest risk if the build loses focus?
-   Encourage strong MVP thinking over feature overload

### 5. **Closure (Time: 20 minutes)**

-   **Objective:** Reinforce that strong prototypes are focused, realistic, and built to prove value clearly.
-   Bring the class together for a final share-out.
-   Ask 3--5 Geniuses to share:
    -   their project name
    -   their MVP
    -   one stretch feature they are intentionally delaying
    -   one build priority they know must happen first
-   Lead a closing discussion:
    -   What makes an MVP strong?
    -   Why is narrowing scope a sign of maturity, not weakness?
    -   How does a build roadmap make capstone work more manageable?
-   Preview the next lesson:
    -   Geniuses will create pitches, demo stories, and final launch-ready communication for their capstone direction.

**Assessment:**
---------------

Student learning will be assessed through:

-   Participation in the icebreaker and discussion
-   Reflection responses during direct instruction
-   Completion of the guided prototype planner
-   Completion of independent `PROTOTYPE_PLAN.md` and `CAPSTONE_BUILD_PLAN.md`
-   Final share-out and explanation of MVP scope and build choices

### **Exit Ticket**

1.  What is an MVP?
2.  What is one difference between a core feature and a stretch feature?
3.  Why does narrowing scope improve a capstone?

**Extra Activities:**
---------------------

-   Geniuses who finish early can:
    -   add a milestone timeline
    -   add a "biggest blocker" section
    -   add a "fallback plan if a feature fails" section
    -   add a basic user flow diagram in markdown
    -   add a demo checklist
    -   add a "what must be ready for pitch day" section
-   Add a "not building yet" section
-   Add a "polish priorities" section
-   Add a "testing goals" section
-   Add a "team role plan" section if applicable

**Reflection / Takeaways:**
---------------------------

This lesson works best when Geniuses realize that strong capstones are not built by doing everything. They are built by proving one strong idea clearly and then expanding with intention. Day 4 helps them move from vision into execution by defining the MVP, the build order, and the success criteria for the capstone phase. By the end of the lesson, Geniuses should feel more confident because they know what to build first, what can wait, and what a strong prototype actually needs to prove.

**Facilitator Notes**
---------------------

-   Keep using **Geniuses** consistently in examples and discussion.
-   Reinforce that MVP scope is about clarity and proof of value.
-   Encourage Geniuses to protect their core user flow from feature creep.
-   Help them write realistic Week 6 and Week 7 goals.
-   Remind Geniuses that tomorrow they will turn all of this into a stronger pitch and demo story.

**Week 5 Day 4 Mini-Project Connection**
----------------------------------------

By the end of Day 4, each Genius should have:

-   A clear MVP definition
-   A `PROTOTYPE_PLAN.md`
-   A `CAPSTONE_BUILD_PLAN.md`
-   Defined core features and stretch features
-   A clear build-first priority
-   Week 6 and Week 7 success goals
-   A stronger sense of how to actually execute the capstone build
