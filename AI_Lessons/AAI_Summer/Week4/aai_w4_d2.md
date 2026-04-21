<img src="https://github.com/Hgp-GeniusLabs/Curriculum/blob/10734f2c827128dde773ea4f266d154d46977866/Org-Wide/Assets/hgp_logo_original.png" width="150"/>

Lesson Plan: Applied AI Week 4, Day 2 --- Building Multi-Agent Workflows
======================================================================

**Duration:**
-------------

3 hours

**Lesson Overview:**
--------------------

On Day 2, Geniuses expand from a single planning agent into a **multi-agent workflow**. The focus of the lesson is understanding how different AI agents can take on different roles and work together as a system. Instead of one agent trying to do everything, Geniuses learn how modern AI products often use specialized agents that each handle a specific part of the job, such as planning, researching, organizing, checking, or drafting.

During guided practice, the class builds a simple multi-agent workflow in Node using the OpenAI API. The system will include multiple role-based agents such as a **Planner Agent**, a **Writer Agent**, and a **Checker Agent**. Each agent will receive the output of the previous one and contribute its own part of the workflow. During independent practice, each Genius designs their own multi-agent system around a real-world use case and begins building the first version of that workflow. This continues the Week 4 mini-project by moving from one intelligent role into coordinated AI teamwork.

**Objectives:**
---------------

-   Define a multi-agent workflow and explain how it differs from a single-agent system.
-   Identify how specialized AI agents can divide work by role.
-   Explain why businesses may use multiple agents instead of one general-purpose agent.
-   Build a Node and OpenAI-powered workflow with multiple agents passing work between roles.
-   Design a multi-agent system for a real business, school, or community problem.
-   Reflect on how coordination, role clarity, and handoffs improve AI system design.

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
-   Existing Week 4 Day 1 project files
-   `.env` file setup instructions

**Standards:**
--------------

-   Computational Thinking: Break down a large problem into smaller role-based tasks and handoffs.
-   Computer Science Practices: Design and build a coordinated AI workflow with specialized components.
-   Programming: Use JavaScript, Node, and API integration to create multi-step intelligent systems.
-   Digital Literacy: Evaluate how role specialization can improve AI quality and usefulness.
-   Career Readiness: Practice systems thinking, coordination, debugging, and structured problem-solving.
-   Entrepreneurship and Innovation: Build AI systems that use specialist roles to create stronger product outcomes.

**Lesson Activity:**
--------------------

### 1. **Introduction (Time: 25 minutes)**

-   **Objective:** Energize Geniuses and introduce the idea that one AI agent does not always need to do everything alone.
-   Start with an icebreaker called **"One Expert or a Team?"**
-   This should be the first thing and the most fun thing to wake Geniuses up and get them ready for the lesson.

#### **Icebreaker Option A: Physical Movement**

-   Label one side of the room **"One Agent"** and the other side **"Multiple Agents."**
-   Read different task scenarios aloud and have Geniuses move to the side that best matches.
-   Example prompts:
    -   Write one short thank-you email
    -   Plan a community event, write an announcement, and double-check the clarity
    -   Summarize one paragraph
    -   Help a Genius organize a study plan, explain the tasks, and check the final output
    -   Generate one product slogan
    -   Break down a business goal, create a plan, and verify that the plan is realistic
    -   Rewrite one sentence
    -   Prepare interview questions, suggest answers, and review for confidence and tone
-   After each round, ask:
    -   Why is one agent enough here?
    -   Why would multiple agents help here?
    -   What different jobs need to happen?
    -   What might improve when roles are separated?

#### **Icebreaker Option B: Role Sort**

-   Write roles on the board such as:
    -   Planner
    -   Researcher
    -   Writer
    -   Reviewer
    -   Organizer
    -   Safety Checker
-   Give a task scenario and ask Geniuses which roles are needed and in what order.
-   Discuss why role order matters.

#### **Transition**

-   Say:
    -   "One strong agent can help a lot. But when the work has different stages, a system of agents can do the job more clearly."
-   Ask:
    -   Why might a business want specialist agents instead of one general AI?
    -   What kinds of roles naturally belong in a workflow?

### 2. **Direct Instruction (Time: 50 minutes)**

-   **Objective:** Help Geniuses understand what multi-agent systems are, how they work, and why role-based workflows matter.
-   Use slides to guide instruction and stop often for discussion.

#### **Suggested Slide Flow**

-   **Slide 1: Day 2 Focus --- From One Agent to a Team of Agents**
    -   Today is about AI coordination, role specialization, and handoffs
-   **Slide 2: What Is a Multi-Agent Workflow?**
    -   A multi-agent workflow is a system where different AI agents handle different parts of a larger task
    -   Each agent has a role and passes work forward
-   **Slide 3: Single-Agent vs Multi-Agent**
    -   Single-agent:
        -   one role
        -   one response flow
    -   Multi-agent:
        -   multiple roles
        -   handoffs
        -   specialization
        -   layered outputs
-   **Slide 4: Why Use Multiple Agents?**
    -   better focus
    -   clearer structure
    -   easier role design
    -   stronger quality control
    -   easier scaling and improvement
-   **Slide 5: Common Agent Roles**
    -   Planner Agent
    -   Research Agent
    -   Writer Agent
    -   Reviewer Agent
    -   Policy Agent
    -   Safety Agent
    -   Formatter Agent
-   **Slide 6: Example Multi-Agent Workflow**
    -   User goal: "Help me prepare for a school event"
    -   Planner Agent creates task structure
    -   Writer Agent turns plan into messaging
    -   Checker Agent reviews clarity and usefulness
-   **Slide 7: Handoffs Matter**
    -   Each agent needs:
        -   clear role
        -   clear input
        -   clear expected output
    -   Bad handoffs create messy systems
-   **Slide 8: Weak Multi-Agent Design vs Strong Multi-Agent Design**
    -   Weak:
        -   overlapping roles
        -   vague tasks
        -   random order
        -   messy outputs
    -   Strong:
        -   clear jobs
        -   clear sequence
        -   useful outputs
        -   role-specific strengths
-   **Slide 9: Today's Build Goal**
    -   Build a simple three-agent workflow:
        -   Planner
        -   Writer
        -   Checker
-   **Slide 10: Week 4 Mini-Project Growth**
    -   Day 1: one planning agent
    -   Day 2: coordinated team of agents

#### **Discussion Questions**

-   Why might multiple agents outperform one general answer?
-   What kinds of tasks benefit from role specialization?
-   What makes a handoff between agents strong?
-   What could go wrong if the roles overlap too much?
-   Why do businesses often rely on workflows instead of one-step outputs?

#### **Reflection Prompt**

-   Have Geniuses write for 4 minutes:
    -   "Describe a real-world task that would benefit from three different AI roles. What would each role do?"

### 3. **Guided Practice (Time: 60 minutes)**

-   **Objective:** Help Geniuses build a simple multi-agent workflow in Node using the OpenAI API.
-   Explain that today's code-along creates a team of role-based agents working in sequence.

#### **Guided Practice Build**

Create a folder called `multi-agent-workflow` or continue from the Week 4 project.

#### **Project Goal**

Build a Node app that:

-   asks the user for a goal
-   sends the goal to a **Planner Agent**
-   sends the planner output to a **Writer Agent**
-   sends the writer output to a **Checker Agent**
-   prints the full workflow result in the terminal

#### **Setup Steps**

1.  Open VS Code.
2.  Create or open a folder called `multi-agent-workflow`.
3.  Open the terminal and run:
```
npm init -y\
npm install openai dotenv
```
1.  Create a `.env` file:
```
OPENAI_API_KEY=your_key_here
```
1.  Create a file called `multiAgentWorkflow.js`

#### **Sample `multiAgentWorkflow.js`**
```
// multiAgentWorkflow.js
// Applied AI Week 4 Day 2
// This script builds a simple multi-agent workflow using the OpenAI API.

require("dotenv").config();
const OpenAI = require("openai");
const readline = require("readline");

// Create the OpenAI client
const client = new OpenAI({
  apiKey: process.env.OPENAI_API_KEY,
});

// Create a readline interface so the Genius can type a goal
const rl = readline.createInterface({
  input: process.stdin,
  output: process.stdout,
});

// Helper function to run an agent with a prompt
async function runAgent(prompt) {
  const response = await client.responses.create({
    model: "gpt-4.1-mini",
    input: prompt,
  });

  return response.output_text;
}

// Ask the Genius for a goal
rl.question("What goal should the multi-agent system help with? ", async (goal) => {
  if (!goal.trim()) {
    console.log("Please enter a real goal.");
    rl.close();
    return;
  }

  try {
    // Agent 1: Planner Agent
    const plannerPrompt = `
You are a Planner Agent.

A Genius has this goal:
"${goal}"

Your job is to:
1. Summarize the goal clearly
2. Break it into 3 to 5 steps
3. Keep the plan practical and well organized

Return in this format:

Goal Summary:
- ...

Plan:
1. ...
2. ...
3. ...
`;

    const plannerOutput = await runAgent(plannerPrompt);

    // Agent 2: Writer Agent
    const writerPrompt = `
You are a Writer Agent.

Use the planner output below to create a polished action guide for a Genius.

Planner Output:
${plannerOutput}

Your job is to:
1. Rewrite the plan in clear, encouraging language
2. Make the steps easy to follow
3. Add a short motivating closing line

Return in this format:

Action Guide:
1. ...
2. ...
3. ...

Closing Line:
- ...
`;

    const writerOutput = await runAgent(writerPrompt);

    // Agent 3: Checker Agent
    const checkerPrompt = `
You are a Checker Agent.

Review the action guide below.

Action Guide Output:
${writerOutput}

Your job is to:
1. Point out one strength of the guide
2. Point out one thing that could be clearer
3. Recommend one improvement

Return in this format:

Strength:
- ...

Could Be Clearer:
- ...

Improvement:
- ...
`;

    const checkerOutput = await runAgent(checkerPrompt);

    console.log("\n--- Planner Agent Output ---");
    console.log(plannerOutput);

    console.log("\n--- Writer Agent Output ---");
    console.log(writerOutput);

    console.log("\n--- Checker Agent Output ---");
    console.log(checkerOutput);
  } catch (error) {
    console.log("Something went wrong while running the multi-agent workflow.");
    console.error(error);
  }

  rl.close();
});
```
#### **How to Run the App**
```
node multiAgentWorkflow.js
```
#### **Guided Practice Teaching Points**

-   Why each agent has a different job
-   Why the output of one agent becomes the input for the next
-   Why role clarity improves the workflow
-   Why checking and reviewing is useful in agent systems
-   Why a sequence of specialized outputs feels more like a system than a single response

#### **Guided Practice Discussion**

-   Which agent added the most value?
-   What happened when the Writer Agent used the Planner Agent's work?
-   Why is the Checker Agent important?
-   What would happen if the prompts were vague?
-   How might this workflow help in a real product?

### 4. **Independent Practice (Time: 30 minutes)**

-   **Objective:** Geniuses independently build their own first version of a multi-agent workflow for a real use case.
-   This continues the Week 4 mini-project.

#### **Mini-Project Title**

**Agentic AI System --- Day 2 Multi-Agent Workflow Foundation**

#### **Independent Task**

Each Genius creates a multi-agent system around a real-world use case.

Examples:

-   study support workflow
-   career preparation workflow
-   event planning workflow
-   small business content workflow
-   community resource support workflow
-   personal productivity workflow

Their workflow must include at least **3 agents** with different roles.

Possible roles:

-   Planner Agent
-   Organizer Agent
-   Writer Agent
-   Coach Agent
-   Reviewer Agent
-   Trust Checker Agent

Their system must:

-   take in a user goal
-   pass the goal through multiple role-based agents
-   print each stage clearly
-   show how each agent contributes differently

#### **Required Deliverables**

-   A working `multiAgentWorkflow.js`
-   A working `.env` file configured locally
-   A multi-agent system with:
    -   a defined use case
    -   at least 3 agent roles
    -   clear handoffs between agents
    -   structured output at each stage
-   A short written reflection:
    -   What does each agent do?
    -   Why are multiple agents better than one for this task?
    -   What handoff was most important in your workflow?

#### **Facilitator Support Moves**

-   Help Geniuses choose a use case with multiple stages
-   Ask:
    -   What roles are needed?
    -   What should the first agent produce?
    -   What does the next agent need as input?
    -   What role checks or improves the quality?
-   Encourage Geniuses to keep the workflow simple and role-based

### 5. **Closure (Time: 15 minutes)**

-   **Objective:** Reinforce that multi-agent systems are coordinated teams, not just larger prompts.
-   Bring the class together for a final share-out.
-   Ask 3--5 Geniuses to share:
    -   their system name
    -   their 3 agent roles
    -   one important handoff in the workflow
    -   why the workflow feels more powerful than a single-agent system
-   Lead a closing discussion:
    -   What makes a multi-agent system strong?
    -   Why does role specialization matter?
    -   What kinds of products or businesses could benefit from this?
-   Preview the next lesson:
    -   Geniuses will focus on data, context, and trust, and how bad or strong information changes what agents produce.

**Assessment:**
---------------

Student learning will be assessed through:

-   Participation in the icebreaker and discussion
-   Reflection responses during direct instruction
-   Completion of the guided multi-agent workflow build
-   Completion of an independent multi-agent system in Node
-   Final share-out and explanation of role specialization and handoffs

### **Exit Ticket**

1.  What is a multi-agent workflow?
2.  Why might multiple agents be better than one agent for some tasks?
3.  What is one agent role you used today?

**Extra Activities:**
---------------------

-   Geniuses who finish early can:
    -   add a fourth agent
    -   create different workflow modes for different user goals
    -   improve output formatting
    -   add a final "Manager Agent" that combines all results
    -   ask the Checker Agent to assign a quality score
    -   return structured JSON instead of plain text
-   Add a deadline input to make the planner more specific
-   Add a user type input to make the workflow more personalized
-   Create a themed workflow for a specific industry or community
-   Add a "final recommendation" stage after the checker

**Reflection / Takeaways:**
---------------------------

This lesson works best when Geniuses realize that multi-agent AI is really about coordination and specialization. One agent can do a lot, but a team of agents can break a larger task into clearer roles and better outputs. Day 2 introduces an important systems mindset: the strength of the system depends not only on the agents themselves, but on the handoffs between them. By the end of the lesson, Geniuses should understand that multi-agent design is a powerful way to build more capable and organized AI products.

**Facilitator Notes**
---------------------

-   Keep using **Geniuses** consistently in examples and discussion.
-   Reinforce that each agent should have a clear role, not a vague job.
-   Encourage Geniuses to think about handoffs carefully.
-   Keep the systems simple enough to understand while still showing role coordination.
-   Remind Geniuses that tomorrow they will explore how data quality and trust affect what these systems produce.

**Week 4 Day 2 Mini-Project Connection**
----------------------------------------

By the end of Day 2, each Genius should have:

-   A defined multi-agent use case
-   A Node project with OpenAI API integration
-   At least 3 role-based agents
-   Clear handoffs between agents
-   Structured outputs at each stage
-   A stronger understanding of how AI systems can coordinate specialized roles
-   A clear foundation for exploring data, context, and trust on Day 3
