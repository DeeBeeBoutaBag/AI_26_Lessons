<img src="https://github.com/Hgp-GeniusLabs/Curriculum/blob/10734f2c827128dde773ea4f266d154d46977866/Org-Wide/Assets/hgp_logo_original.png" width="150"/>

Lesson Plan: Applied AI Week 4, Day 3 --- Data Quality, Context, and Trust in AI Systems
======================================================================================

**Duration:**
-------------

3 hours

**Lesson Overview:**
--------------------

On Day 3, Geniuses focus on one of the most important parts of building trustworthy AI systems: **data and context**. After exploring single-agent and multi-agent workflows, Geniuses now examine what those systems depend on in order to produce strong results. This lesson centers on a key idea: even smart agents can produce weak, misleading, or harmful outputs if they are given weak inputs, unclear context, poor data, or untrustworthy information.

Geniuses explore how data quality affects AI systems, why context changes results, and how product builders should think about trust when designing agentic workflows. During guided practice, the class builds a small Node-based workflow that compares what happens when an agent receives **low-quality** context versus **high-quality** context. During independent practice, each Genius improves their own multi-agent system by adding structured context, clearer inputs, and a basic trust-aware design choice. By the end of the lesson, Geniuses should understand that stronger AI systems require stronger information.

**Objectives:**
---------------

-   Explain why data quality and context matter in AI systems.
-   Identify how weak, vague, or untrustworthy inputs can lead to poor AI output.
-   Compare low-quality and high-quality context in an agent workflow.
-   Explain why trust is shaped not only by the interface, but also by the quality of information behind the system.
-   Build a Node and OpenAI-powered context comparison workflow.
-   Improve an agentic system by adding better structured context and trust-aware logic.
-   Reflect on how trustworthy inputs create more useful and responsible outputs.

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
-   Existing Week 4 Day 1 and Day 2 project files
-   `.env` file setup instructions

**Standards:**
--------------

-   Computational Thinking: Analyze how information quality affects system performance and outcomes.
-   Computer Science Practices: Design, compare, and improve AI system behavior using better structured inputs.
-   Programming: Use JavaScript, Node, and API integration to model context-aware AI workflows.
-   Digital Literacy: Evaluate trust, reliability, and quality in AI-generated outputs.
-   Career Readiness: Practice critical thinking, systems analysis, and decision-making around information quality.
-   Entrepreneurship and Innovation: Build AI systems that are not only functional, but also trustworthy and informed by stronger data.

**Lesson Activity:**
--------------------

### 1. **Introduction (Time: 25 minutes)**

-   **Objective:** Energize Geniuses and introduce the idea that even strong AI systems can fail when the information going into them is weak.
-   Start with an icebreaker called **"Good Data or Bad Data?"**
-   This should be the first thing and the most fun thing to wake Geniuses up and get them ready for the lesson.

#### **Icebreaker Option A: Physical Movement**

-   Label one side of the room **"Stronger Input"** and the other side **"Weaker Input."**
-   Read examples aloud and have Geniuses move to the side that best matches.
-   Example prompts:
    -   "Help me with my homework"
    -   "I have a biology quiz Friday on cell division and I have 45 minutes tonight to study"
    -   "Plan something for me"
    -   "I need to organize a youth event for 40 people, and I already have a venue but no food plan or volunteer schedule"
    -   "Write a message"
    -   "Write a respectful follow-up email to a mentor after a job shadow, and keep it under 120 words"
    -   "These notes are from a meeting"
    -   "These notes are from a meeting about a school fundraiser, and the team still needs sponsorship outreach, flyer design, and parent volunteers"
-   After each round, ask:
    -   What makes one input stronger?
    -   How does more context help?
    -   Can too little information make the AI guess?
    -   What would you need to trust the result more?

#### **Icebreaker Option B: Output Comparison**

-   Show two prompts and ask Geniuses which one would produce better output.
-   Discuss why better context creates better system behavior.

#### **Transition**

-   Say:
    -   "An agent is only as strong as the information it receives and the context it understands."
-   Ask:
    -   What happens when the AI has to guess?
    -   Why should builders care about the quality of the data going in?

### 2. **Direct Instruction (Time: 50 minutes)**

-   **Objective:** Help Geniuses understand how data quality, context, and trust affect AI systems and agent workflows.
-   Use slides to guide instruction and pause often for discussion.

#### **Suggested Slide Flow**

-   **Slide 1: Day 3 Focus --- Better Data, Better Systems**
    -   Agentic systems depend on the quality of the information they receive
-   **Slide 2: What Do We Mean by Data and Context?**
    -   Data can mean:
        -   user input
        -   structured details
        -   task information
        -   notes
        -   records
        -   knowledge sources
    -   Context means:
        -   what the system knows about the situation
        -   what the user is trying to do
        -   what constraints matter
-   **Slide 3: Why Data Quality Matters**
    -   vague input leads to vague output
    -   misleading input leads to misleading output
    -   missing context leads to guessing
    -   untrusted sources can create false confidence
-   **Slide 4: Good Data vs Bad Data**
    -   Good data is:
        -   relevant
        -   specific
        -   clear
        -   timely
        -   organized
    -   Bad data is:
        -   vague
        -   outdated
        -   incomplete
        -   messy
        -   unverified
-   **Slide 5: Why Context Changes Everything**
    -   The same task can produce very different results depending on:
        -   user age
        -   setting
        -   deadlines
        -   constraints
        -   goals
        -   available resources
-   **Slide 6: Trust in AI Systems**
    -   Users trust systems more when:
        -   outputs are grounded
        -   assumptions are limited
        -   context is clear
        -   uncertainty is acknowledged
        -   the product avoids pretending to know too much
-   **Slide 7: Agent Systems Need Better Inputs**
    -   multi-agent systems do not remove the need for good data
    -   they often make it even more important
    -   weak handoffs plus weak data create weak systems
-   **Slide 8: Example of Context Improvement**
    -   Weak input:
        -   "Help me plan"
    -   Strong input:
        -   "Help me plan a two-hour after-school workshop for 20 middle school students about AI basics using laptops and a projector"
-   **Slide 9: What Builders Should Ask**
    -   What does the system know?
    -   What does it not know?
    -   What information matters most?
    -   What assumptions is the system making?
    -   Should the system ask for more context first?
-   **Slide 10: Week 4 Mini-Project Growth**
    -   Day 1: planner agent
    -   Day 2: multi-agent workflow
    -   Day 3: better context, better trust

#### **Discussion Questions**

-   Why can strong models still produce weak results?
-   What makes input trustworthy?
-   Why is missing context dangerous in AI systems?
-   Should an AI system sometimes ask for more information before acting?
-   How can better data improve trust?

#### **Reflection Prompt**

-   Have Geniuses write for 4 minutes:
    -   "Think about your multi-agent system. What information does it need in order to give a truly useful and trustworthy result?"

### 3. **Guided Practice (Time: 60 minutes)**

-   **Objective:** Help Geniuses build a Node-based workflow that compares weak context and strong context for the same task.
-   Explain that today's code-along helps make invisible system quality visible.

#### **Guided Practice Build**

Create a folder called `context-trust-lab` or continue from the Week 4 project.

#### **Project Goal**

Build a Node app that:

-   takes the same task
-   sends a **low-context version** to an agent
-   sends a **high-context version** to an agent
-   compares the outputs
-   prints a short trust reflection at the end

#### **Setup Steps**

1.  Open VS Code.
2.  Create or open a folder called `context-trust-lab`.
3.  Open the terminal and run:
```
npm init -y\
npm install openai dotenv
```
1.  Create a `.env` file:
```
OPENAI_API_KEY=your_key_here
```
1.  Create a file called `contextTrustLab.js`

#### **Sample `contextTrustLab.js`**
```
// contextTrustLab.js
// Applied AI Week 4 Day 3
// This script compares low-context and high-context AI outputs
// to show why data quality and context matter.

require("dotenv").config();
const OpenAI = require("openai");

const client = new OpenAI({
  apiKey: process.env.OPENAI_API_KEY,
});

// Helper function to run the AI
async function runAgent(prompt) {
  const response = await client.responses.create({
    model: "gpt-4.1-mini",
    input: prompt,
  });

  return response.output_text;
}

async function main() {
  const lowContextTask = "Help me plan a study routine.";

  const highContextTask = `
Help me plan a study routine.

Context:
- I am a high school Genius
- I have a biology quiz on Friday
- I have 45 minutes tonight and 1 hour tomorrow
- I struggle most with vocabulary and diagrams
- I want a simple plan that does not feel overwhelming
`;

  try {
    const lowContextPrompt = `
You are a study support agent.

A Genius said:
"${lowContextTask}"

Create a short study plan.
`;

    const highContextPrompt = `
You are a study support agent.

A Genius said:
"${highContextTask}"

Create a short study plan that uses the specific context provided.
`;

    const lowContextOutput = await runAgent(lowContextPrompt);
    const highContextOutput = await runAgent(highContextPrompt);

    const comparisonPrompt = `
You are a trust and context reviewer.

Compare these two outputs:

Low-Context Output:
${lowContextOutput}

High-Context Output:
${highContextOutput}

Please answer in this format:

Better Output:
- ...

Why It Is Better:
- ...

Trust Insight:
- ...
`;

    const comparisonOutput = await runAgent(comparisonPrompt);

    console.log("\n--- Low-Context Output ---");
    console.log(lowContextOutput);

    console.log("\n--- High-Context Output ---");
    console.log(highContextOutput);

    console.log("\n--- Comparison and Trust Insight ---");
    console.log(comparisonOutput);\
  } catch (error) {
    console.log("Something went wrong while running the context trust lab.");
    console.error(error);
  }
}

main();
```
#### **How to Run the App**
```
node contextTrustLab.js
```
#### **Guided Practice Teaching Points**

-   Why context improves relevance
-   Why vague requests often force the AI to generalize
-   Why stronger inputs help users trust the result more
-   Why comparison is a useful systems design tool
-   Why agent systems may need context gathering before action

#### **Guided Practice Discussion**

-   Which output felt more useful?
-   Which output felt more trustworthy?
-   What details made the high-context version stronger?
-   Should the system ask a follow-up question when context is missing?
-   What role could a context-gathering agent play in a larger system?

### 4. **Independent Practice (Time: 30 minutes)**

-   **Objective:** Geniuses independently improve their multi-agent system by adding stronger context and a trust-aware input design choice.
-   This continues the Week 4 mini-project.

#### **Mini-Project Title**

**Agentic AI System --- Day 3 Data, Context, and Trust Upgrade**

#### **Independent Task**

Each Genius updates their multi-agent system so it uses better information before the workflow begins.

They must do at least **2 of the following**:

-   add more structured user input
-   add a second question to gather context
-   add a "constraints" field
-   add a "deadline" field
-   add a "user type" field
-   add a trust or caution message
-   add a comparison between vague and structured input
-   add a simple "ask for more information" step before running the workflow

Examples:

-   a study agent asks for subject and available time
-   an event planner agent asks for number of attendees and budget
-   a career agent asks for interests and current grade level
-   a business workflow agent asks for team size and deadline

#### **Required Deliverables**

-   A working updated `.js` file for the agent system
-   A working `.env` file configured locally
-   A workflow with:
    -   stronger context gathering
    -   at least 2 trust-aware input improvements
    -   more structured output
-   A short written reflection:
    -   What new context did your system collect?
    -   How did that improve the output?
    -   What made the system feel more trustworthy?

#### **Facilitator Support Moves**

-   Help Geniuses identify what information their system truly needs
-   Ask:
    -   What does your agent need to know before it acts?
    -   What details matter most?
    -   What happens when that information is missing?
    -   Should your system ask a follow-up before moving on?
-   Encourage Geniuses to test weak versus strong context

### 5. **Closure (Time: 15 minutes)**

-   **Objective:** Reinforce that strong AI systems depend on strong information, not only strong models.
-   Bring the class together for a final share-out.
-   Ask 3--5 Geniuses to share:
    -   one context improvement they added
    -   one way the output got better
    -   one trust-related lesson they learned
-   Lead a closing discussion:
    -   Why does context matter in agent systems?
    -   What is the relationship between data quality and trust?
    -   What kinds of systems need to ask more questions before acting?
-   Preview the next lesson:
    -   Geniuses will explore AI policies, guardrails, and how systems should know when to proceed, warn, or stop.

**Assessment:**
---------------

Student learning will be assessed through:

-   Participation in the icebreaker and discussion
-   Reflection responses during direct instruction
-   Completion of the guided context comparison build
-   Completion of an independent system upgrade with better context
-   Final share-out and explanation of trust improvements

### **Exit Ticket**

1.  Why does context matter in AI systems?
2.  What makes input stronger or weaker?
3.  What is one improvement you made to make your system more trustworthy today?

**Extra Activities:**
---------------------

-   Geniuses who finish early can:
    -   add a "missing info" detector
    -   build a context-gathering agent before the planner
    -   return structured JSON for context fields
    -   add different outputs depending on user type
    -   add a "confidence note" at the end of the workflow
    -   compare three levels of context instead of two
-   Add a budget field for planning systems
-   Add a priority level field
-   Add an "unknowns" section in the final output
-   Add a final reminder that better results depend on better input

**Reflection / Takeaways:**
---------------------------

This lesson works best when Geniuses realize that the intelligence of an AI system is not only about the model. It is also about the quality of the information the system receives and the discipline of how that information is structured. Day 3 introduces an important systems truth: trust is shaped by inputs, not just outputs. By the end of the lesson, Geniuses should understand that stronger data and clearer context are essential parts of building agentic systems that are actually useful and responsible.

**Facilitator Notes**
---------------------

-   Keep using **Geniuses** consistently in examples and discussion.
-   Reinforce that vague goals often lead to vague systems.
-   Encourage Geniuses to think like system designers who gather the right information before acting.
-   Help Geniuses connect context quality to trust and usefulness.
-   Remind Geniuses that tomorrow they will add policy thinking and guardrails to these systems.

**Week 4 Day 3 Mini-Project Connection**
----------------------------------------

By the end of Day 3, each Genius should have:

-   A stronger multi-agent system
-   Better structured context or input gathering
-   At least 2 trust-aware input improvements
-   A clearer sense of what information their system needs
-   A better understanding of why data quality shapes AI quality
-   A strong foundation for adding guardrails and AI policy logic on Day 4
