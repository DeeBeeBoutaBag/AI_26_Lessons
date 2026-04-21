<img src="https://github.com/Hgp-GeniusLabs/Curriculum/blob/10734f2c827128dde773ea4f266d154d46977866/Org-Wide/Assets/hgp_logo_original.png" width="150"/>

Lesson Plan: Applied AI Week 4, Day 1 --- What Is Agentic AI?
===========================================================

**Duration:**
-------------

3 hours

**Lesson Overview:**
--------------------

In Week 4, Geniuses move from building AI features to designing AI systems. Day 1 introduces **Agentic AI**, which means AI systems that do more than generate one answer. Agentic systems can receive a goal, break the work into steps, make decisions, complete actions in sequence, and respond based on what happens along the way. Geniuses explore the difference between a normal AI interaction and an agent workflow, and they begin thinking like system designers instead of only interface builders.

During guided practice, Geniuses will build a simple agent workflow in JavaScript and Node that takes a user goal, breaks it into steps, and produces a structured output. The class will use OpenAI API access to create a basic "planner agent" that turns a big task into smaller actions. During independent practice, each Genius creates the first version of an agentic AI tool that solves a real problem through planning and step-by-step reasoning. This begins the Week 4 mini-project: designing an AI system with task flow, trust, and structure.

**Objectives:**
---------------

-   Define Agentic AI and explain how it differs from a basic AI response.
-   Identify the parts of an agent workflow, including goal, task breakdown, actions, and output.
-   Explain why agentic systems are useful in modern AI products and businesses.
-   Build a simple Node and OpenAI-powered planner agent in VS Code.
-   Design an agent that takes a user goal and turns it into a structured plan.
-   Begin the Week 4 mini-project by creating a simple agentic AI workflow.

**Materials:**
--------------

-   Laptops for all Geniuses
-   VS Code installed
-   Internet access
-   Node.js and NPM installed
-   OpenAI API key for each Genius or team
-   Projector or display
-   Whiteboard and markers
-   Slide deck for lecture and discussion
-   Reflection journal or digital notes
-   Browser or terminal for testing Node apps
-   Starter project folder
-   `.env` file setup instructions

**Standards:**
--------------

-   Computational Thinking: Break complex goals into smaller steps, actions, and decision paths.
-   Computer Science Practices: Design and implement an AI-powered workflow that solves a task in sequence.
-   Web Development and Programming: Use JavaScript, Node, and API integration to build an intelligent system.
-   Digital Literacy: Evaluate how AI systems make decisions and why structure matters.
-   Career Readiness: Practice systems thinking, logic, iteration, and communication.
-   Entrepreneurship and Innovation: Design AI systems that move beyond a single response and create useful action-oriented output.

**Lesson Activity:**
--------------------

### 1. **Introduction (Time: 25 minutes)**

-   **Objective:** Energize Geniuses and introduce the idea that some AI systems do more than answer one question. They can pursue a goal through multiple steps.
-   Start with an icebreaker called **"Answer or Agent?"**
-   This should be the first thing and the most fun thing to wake Geniuses up and get them ready for the lesson.

#### **Icebreaker Option A: Physical Movement**

-   Label one side of the room **"Just an Answer"** and the other side **"Acts Like an Agent."**
-   Read different AI behaviors aloud and have Geniuses move to the side that best matches.
-   Example prompts:
    -   An AI gives one paragraph explaining climate change
    -   An AI turns a big school project into a checklist with deadlines
    -   An AI writes one email draft when asked
    -   An AI receives a business goal and creates a step-by-step action plan
    -   An AI summarizes one article
    -   An AI looks at a task, decides what should happen first, and organizes the workflow
    -   An AI gives a motivational quote
    -   An AI helps a user plan, revise, and prioritize multiple actions
-   After each round, ask:
    -   Why is this just an answer?
    -   Why does this feel more agentic?
    -   What makes something an actual system instead of one output?
    -   Where might businesses want agent-like behavior?

#### **Icebreaker Option B: Quick Scenario Sort**

-   Put example scenarios on the board and ask Geniuses to sort them into:
    -   one-time AI response
    -   agent workflow
-   Discuss why task breakdown, next actions, and decision-making matter.

#### **Transition**

-   Say:
    -   "A chatbot can answer. An agent can work through a goal."
-   Ask:
    -   What happens when the task is too big for one answer?
    -   Why might businesses want AI that can organize work instead of only respond?

### 2. **Direct Instruction (Time: 50 minutes)**

-   **Objective:** Help Geniuses understand what Agentic AI is, how it works, and why it matters in modern products and business systems.
-   Use slides to guide instruction and stop often for discussion.

#### **Suggested Slide Flow**

-   **Slide 1: Week 4 Focus --- From AI Features to AI Systems**
    -   This week is about agentic AI, multi-agent workflows, trust, data, and policy
    -   Geniuses are moving from building features to designing systems
-   **Slide 2: What Is Agentic AI?**
    -   Agentic AI is AI that works toward a goal through multiple steps
    -   It can:
        -   receive a goal
        -   plan
        -   choose actions
        -   produce structured progress
        -   respond based on what happens next
-   **Slide 3: AI Response vs Agent Workflow**
    -   Response:
        -   one prompt
        -   one answer
    -   Agent:
        -   goal
        -   steps
        -   sequence
        -   structure
        -   follow-through
-   **Slide 4: Key Parts of an Agent**
    -   Goal
    -   Input
    -   Plan
    -   Actions
    -   Output
    -   Next step
    -   Sometimes memory or feedback
-   **Slide 5: Why Businesses Care About Agentic AI**
    -   task planning
    -   customer workflows
    -   operations support
    -   productivity systems
    -   research assistance
    -   scheduling and coordination
    -   decision support
-   **Slide 6: Example Agent Workflow**
    -   User goal: "Help me prepare for a job fair"
    -   Agent:
        -   identifies what the user needs
        -   breaks the goal into steps
        -   creates preparation tasks
        -   prioritizes the tasks
        -   gives a suggested starting action
-   **Slide 7: Agentic AI Is Not Magic**
    -   It still depends on:
        -   good prompts
        -   clear goals
        -   structured outputs
        -   trustworthy data
        -   rules and guardrails
-   **Slide 8: Weak Agent Design vs Strong Agent Design**
    -   Weak:
        -   vague goal
        -   messy output
        -   no structure
        -   no next step
    -   Strong:
        -   clear purpose
        -   organized steps
        -   useful sequence
        -   actionable result
-   **Slide 9: Today's Build Goal**
    -   Build a simple planner agent that takes a goal and turns it into a step-by-step plan
-   **Slide 10: Week 4 Mini-Project**
    -   Build an AI system that uses task flow, structure, and trust-aware decisions

#### **Discussion Questions**

-   What makes an AI tool feel more like an agent than a chatbot?
-   Why is step-by-step planning useful in business or everyday life?
-   What kinds of tasks are too large for one answer?
-   Why does structure matter in agent systems?
-   What could go wrong if an agent has a vague goal?

#### **Reflection Prompt**

-   Have Geniuses write for 4 minutes:
    -   "Describe a real task in school, work, family, or community life that would be better solved by an AI agent than by one single response."

### 3. **Guided Practice (Time: 60 minutes)**

-   **Objective:** Help Geniuses build a simple planner agent in Node using the OpenAI API.
-   Explain that today's code-along is about building the first piece of an agent system: planning.

#### **Guided Practice Build**

Create a folder called `planner-agent`.

#### **Project Goal**

Build a Node app that:

-   asks the user for a goal
-   sends that goal to the OpenAI API
-   asks the model to act like a planning agent
-   returns:
    -   a short goal summary
    -   3--5 action steps
    -   one recommended first move

#### **Setup Steps**

1.  Open VS Code.
2.  Create a folder called `planner-agent`.
3.  Open the terminal and run:
```
npm init -y\
npm install openai dotenv
```
1.  Create a `.env` file:
```
OPENAI_API_KEY=your_key_here
```
1.  Create a file called `plannerAgent.js`

#### **Sample `plannerAgent.js`**
```
// plannerAgent.js
// Applied AI Week 4 Day 1
// This script builds a simple planner agent using the OpenAI API.

require("dotenv").config();
const OpenAI = require("openai");
const readline = require("readline");

// Create the OpenAI client
const client = new OpenAI({
  apiKey: process.env.OPENAI_API_KEY,
});

// Create a readline interface so the Genius can type a goal in the terminal
const rl = readline.createInterface({
  input: process.stdin,
  output: process.stdout,
});

// Ask the user for a goal
rl.question("What goal do you want the planner agent to help with? ", async (goal) => {
  if (!goal.trim()) {
    console.log("Please enter a real goal.");
    rl.close();
    return;
  }

  try {
    const prompt = `
You are a planning agent.

A Genius has this goal:
"${goal}"

Your job is to:
1. Summarize the goal in one clear sentence
2. Break the goal into 3 to 5 action steps
3. Recommend the best first move
4. Keep the language practical, clear, and encouraging

Return your answer in this exact format:

Goal Summary:
- ...

Action Steps:
1. ...
2. ...
3. ...

Best First Move:
- ...
`;

    const response = await client.responses.create({
      model: "gpt-4.1-mini",
      input: prompt,
    });

    console.log("\n--- Planner Agent Output ---");
    console.log(response.output_text);
  } catch (error) {
    console.log("Something went wrong while running the planner agent.");
    console.error(error);
  }

  rl.close();
});
```
#### **How to Run the App**
```
node plannerAgent.js
```
#### **Guided Practice Teaching Points**

-   Why the AI is being asked to take on a role
-   Why a goal is different from a question
-   Why structured output makes the agent more useful
-   Why action steps and next moves matter in agent workflows
-   Why even a simple planner agent is already different from a one-answer chatbot

#### **Guided Practice Discussion**

-   What part of this felt most agentic?
-   Why is "best first move" an important part of the output?
-   How would this feel different if the AI only gave one paragraph?
-   What else might a stronger agent need later in the week?

### 4. **Independent Practice (Time: 30 minutes)**

-   **Objective:** Geniuses independently build their own simple agentic AI workflow based on a real goal or use case.
-   This begins the Week 4 mini-project.

#### **Mini-Project Title**

**Agentic AI System --- Day 1 Planner Agent Foundation**

#### **Independent Task**

Each Genius creates their own planning agent around a real use case.

Examples:

-   study planning agent
-   event planning agent
-   career preparation agent
-   community project planning agent
-   wellness routine agent
-   small business task planner

Their agent must:

-   take in a user goal
-   summarize the goal
-   break it into steps
-   suggest a first move
-   use a clear structured format

#### **Required Deliverables**

-   A working `plannerAgent.js`
-   A working `.env` file configured locally
-   A planning agent with:
    -   a defined use case
    -   a clear goal input
    -   a structured output
    -   at least 3 action steps
    -   one best first move
-   A short written reflection:
    -   What goal does your agent help with?
    -   Why is an agent better than one single answer for this task?
    -   What would make your agent stronger later?

#### **Facilitator Support Moves**

-   Help Geniuses choose a use case with a real goal
-   Ask:
    -   What is the goal?
    -   What kind of steps would be useful?
    -   What should the first move help the user do?
    -   Why does this need planning instead of one quick answer?
-   Encourage Geniuses to test multiple goals

### 5. **Closure (Time: 15 minutes)**

-   **Objective:** Reinforce the idea that agentic AI is about systems that pursue goals through structure and action.
-   Bring the class together for a final share-out.
-   Ask 3--5 Geniuses to share:
    -   their agent name
    -   the kind of goal it helps with
    -   one action step it generated
    -   why the workflow feels more like an agent
-   Lead a closing discussion:
    -   What makes agentic AI different from a normal AI response?
    -   Why might businesses want agent-style systems?
    -   What kinds of tasks work well for planner agents?
-   Preview the next lesson:
    -   Geniuses will expand from one agent into multi-agent workflows where different agents have different roles.

**Assessment:**
---------------

Student learning will be assessed through:

-   Participation in the icebreaker and discussion
-   Reflection responses during direct instruction
-   Completion of the guided planner agent build
-   Completion of an independent agent workflow in Node
-   Final share-out and explanation of why the tool is agentic

### **Exit Ticket**

1.  What is Agentic AI?
2.  What makes an agent different from one AI answer?
3.  What is one real-world goal your agent could help with?

**Extra Activities:**
---------------------

-   Geniuses who finish early can:
    -   add a custom agent name
    -   make the planner more specific to a target user
    -   improve the output formatting
    -   add a second mode like "quick plan" versus "detailed plan"
    -   ask the agent to include possible obstacles
    -   add a second question for deadline or urgency
-   Add color output in the terminal using a simple package
-   Return the output in JSON format
-   Ask the agent to prioritize the steps by urgency
-   Add a "why this first move matters" section

**Reflection / Takeaways:**
---------------------------

This lesson works best when Geniuses realize that AI systems can do more than respond. They can organize work around a goal. Day 1 of Week 4 introduces a major shift in thinking: the product is no longer just an AI feature or interface. It is becoming a system with flow, structure, and purpose. By the end of the lesson, Geniuses should understand that even a simple planner agent shows the beginning of what agentic AI can do in real products and real businesses.

**Facilitator Notes**
---------------------

-   Keep using **Geniuses** consistently in examples and discussion.
-   Reinforce that agentic AI still depends on clear prompts and structure.
-   Encourage Geniuses to think in terms of goals, steps, and actions.
-   Keep the first build focused and manageable.
-   Remind Geniuses that tomorrow they will move from one planning agent to multiple agents with different jobs.

**Week 4 Day 1 Mini-Project Connection**
----------------------------------------

By the end of Day 1, each Genius should have:

-   A defined agent use case
-   A Node project with OpenAI API integration
-   A simple planner agent that takes a goal
-   Structured output with action steps
-   A recommended first move
-   A stronger understanding of what makes an AI system agentic
-   A clear foundation for building multi-agent workflows on Day 2
