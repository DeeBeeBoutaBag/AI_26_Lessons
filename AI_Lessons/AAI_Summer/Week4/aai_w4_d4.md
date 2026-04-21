<img src="https://github.com/Hgp-GeniusLabs/Curriculum/blob/10734f2c827128dde773ea4f266d46977866/Org-Wide/Assets/hgp_logo_original.png" width="150"/>

Lesson Plan: Applied AI Week 4, Day 4 --- AI Policies, Guardrails, and Responsible Agent Design
=============================================================================================

**Duration:**
-------------

3 hours

**Lesson Overview:**
--------------------

On Day 4, Geniuses focus on one of the most important parts of building real AI systems: **policies and guardrails**. After learning about planner agents, multi-agent workflows, and the importance of data quality and trust, Geniuses now explore how AI systems should know when to proceed, when to ask for more information, when to warn the user, and when to stop. The lesson centers on the idea that strong AI systems are not just capable. They are also responsible, bounded, and designed with clear rules.

Geniuses learn that businesses and organizations cannot allow AI systems to respond to every request in the same way. Some situations require extra caution, some require human review, and some should be refused or redirected entirely. During guided practice, the class builds a simple Node-based policy-aware agent workflow that checks the user's request, labels the level of risk, and chooses an action such as proceed, ask for more context, or escalate. During independent practice, each Genius adds policy logic and guardrails to their own agentic system so it becomes more trustworthy and realistic. By the end of the lesson, Geniuses should understand that policies are part of product design, not just legal language.

**Objectives:**
---------------

-   Explain what AI policies and guardrails are and why they matter in agentic systems.
-   Identify when an AI system should proceed, ask a follow-up question, warn the user, or escalate to a human.
-   Distinguish between low-risk, medium-risk, and higher-risk AI requests.
-   Build a Node and OpenAI-powered workflow that applies simple policy logic before generating output.
-   Add guardrails and trust-aware rules to an existing agent system.
-   Reflect on how policies improve product trust, safety, and responsible design.

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
-   Existing Week 4 Day 1--3 project files
-   `.env` file setup instructions

**Standards:**
--------------

-   Computational Thinking: Design rules and decision paths that shape how systems respond in different situations.
-   Computer Science Practices: Build and refine an AI system with safeguards, branching logic, and responsible behavior.
-   Programming: Use JavaScript, Node, and API integration to create policy-aware workflows.
-   Digital Literacy: Evaluate safety, trust, and responsibility in AI-generated outputs.
-   Career Readiness: Practice judgment, risk evaluation, and responsible systems thinking.
-   Entrepreneurship and Innovation: Build AI systems that are useful, trustworthy, and designed with clear limits.

**Lesson Activity:**
--------------------

### 1. **Introduction (Time: 25 minutes)**

-   **Objective:** Energize Geniuses and introduce the idea that not every request should be handled the same way by an AI system.
-   Start with an icebreaker called **"Proceed, Pause, or Escalate?"**
-   This should be the first thing and the most fun thing to wake Geniuses up and get them ready for the lesson.

#### **Icebreaker Option A: Physical Movement**

-   Label three parts of the room:
    -   **Proceed**
    -   **Ask More**
    -   **Escalate**
-   Read scenarios aloud and have Geniuses move to the action they think the AI system should take.
-   Example prompts:
    -   "Help me organize my homework for this week"
    -   "Tell me how to respond to my teacher about a missed assignment"
    -   "Help me decide whether I should stop taking my medicine"
    -   "Plan a budget-friendly birthday event for 25 people"
    -   "Write a message apologizing to my friend"
    -   "Tell me whether I should invest all my savings in one stock"
    -   "Help me prepare interview questions for a summer internship"
    -   "Tell me if this chest pain is serious"
-   After each round, ask:
    -   Why should the system proceed here?
    -   Why should it ask for more information?
    -   Why should this be escalated or limited?
    -   What kind of risk is present?

#### **Icebreaker Option B: Scenario Sort**

-   Put scenarios on the board and ask Geniuses to sort them into:
    -   low-risk
    -   needs more context
    -   high-risk / human review
-   Discuss where the line should be and why.

#### **Transition**

-   Say:
    -   "A strong AI system is not just helpful. It also knows when to slow down, ask questions, or stop."
-   Ask:
    -   Why do AI systems need boundaries?
    -   What could happen if every request gets a confident answer no matter the situation?

### 2. **Direct Instruction (Time: 50 minutes)**

-   **Objective:** Help Geniuses understand AI policies, guardrails, escalation, and risk-aware product behavior.
-   Use slides to guide instruction and pause often for discussion.

#### **Suggested Slide Flow**

-   **Slide 1: Day 4 Focus --- Policies and Guardrails**
    -   Today is about making agentic systems more responsible and trustworthy
-   **Slide 2: What Is an AI Policy?**
    -   A policy is a rule or decision framework that guides how the system should behave
    -   Policies shape:
        -   what the system can do
        -   what it should not do
        -   when it should warn
        -   when it should ask for more context
        -   when it should escalate
-   **Slide 3: What Are Guardrails?**
    -   Guardrails are practical controls built into the product
    -   They help prevent unsafe, misleading, or overconfident behavior
-   **Slide 4: Why Policies Matter in Agentic AI**
    -   Agentic systems do more than answer once
    -   They plan, act, and hand off work
    -   That makes boundaries even more important
-   **Slide 5: Common Policy Actions**
    -   Proceed normally
    -   Ask a clarifying question
    -   Add a caution note
    -   Limit the output
    -   Recommend human review
    -   Refuse or redirect
-   **Slide 6: Risk Levels in AI Products**
    -   **Low-risk:** simple productivity, planning, organization
    -   **Medium-risk:** personalized recommendations that may affect choices
    -   **Higher-risk:** health, legal, financial, safety, crisis-related situations
-   **Slide 7: Example Guardrail Questions**
    -   Is this request high-impact?
    -   Does the system have enough context?
    -   Could the user be harmed if the output is wrong?
    -   Should a human be involved?
    -   Should the system be more cautious here?
-   **Slide 8: Policies Are Part of Product Design**
    -   They show up in:
        -   system prompts
        -   branching logic
        -   warnings
        -   escalation rules
        -   UI copy
        -   user experience
-   **Slide 9: Weak Policy Design vs Strong Policy Design**
    -   Weak:
        -   answers everything
        -   ignores uncertainty
        -   never asks questions
        -   gives risky advice casually
    -   Strong:
        -   recognizes risk
        -   asks for more context
        -   limits itself appropriately
        -   builds trust through caution
-   **Slide 10: Today's Build Goal**
    -   Build an agentic workflow with a simple policy checker that decides whether to proceed, ask for more context, or escalate

#### **Discussion Questions**

-   Why do AI systems need policies even if the AI is powerful?
-   What kinds of requests should never be answered casually?
-   Why is "ask for more information" sometimes the best action?
-   What makes a guardrail feel helpful instead of annoying?
-   How do policies increase trust?

#### **Reflection Prompt**

-   Have Geniuses write for 4 minutes:
    -   "Think about your agent system. What kinds of requests should it handle easily, and what kinds should it treat more carefully?"

### 3. **Guided Practice (Time: 60 minutes)**

-   **Objective:** Help Geniuses build a Node-based policy-aware workflow that classifies request risk and chooses an action before generating output.
-   Explain that today's build adds product rules to the system.

#### **Guided Practice Build**

Create a folder called `policy-aware-agent` or continue from the Week 4 project.

#### **Project Goal**

Build a Node app that:

-   asks the user for a request
-   checks the request with a **Policy Agent**
-   labels the request as:
    -   proceed
    -   ask for more context
    -   escalate
-   then either:
    -   generates a normal response
    -   asks a follow-up
    -   returns a caution or escalation message

#### **Setup Steps**

1.  Open VS Code.
2.  Create or open a folder called `policy-aware-agent`.
3.  Open the terminal and run:
```
npm init -y
npm install openai dotenv
```
1.  Create a `.env` file:
```
OPENAI_API_KEY=your_key_here
```
1.  Create a file called `policyAwareAgent.js`

#### **Sample `policyAwareAgent.js`**
```
// policyAwareAgent.js
// Applied AI Week 4 Day 4
// This script adds simple policy-aware logic to an agent workflow.

require("dotenv").config();
const OpenAI = require("openai");
const readline = require("readline");

const client = new OpenAI({
  apiKey: process.env.OPENAI_API_KEY,
});

const rl = readline.createInterface({
  input: process.stdin,
  output: process.stdout,
});

async function runAgent(prompt) {
  const response = await client.responses.create({
    model: "gpt-4.1-mini",
    input: prompt,
  });

  return response.output_text;
}

rl.question("What do you want help with? ", async (userRequest) => {
  if (!userRequest.trim()) {
    console.log("Please enter a real request.");
    rl.close();
    return;
  }

  try {
    const policyPrompt = `
You are a Policy Agent for an AI system.

Review the user request below and classify it into one of three actions:
- proceed
- ask_for_more_context
- escalate

User Request:
"${userRequest}"

Rules:
- Use "proceed" for everyday low-risk support tasks
- Use "ask_for_more_context" if the request is too vague or missing important context
- Use "escalate" if the request appears health-related, legal, financial high-stakes, or safety-sensitive

Return valid JSON in this exact format:
{
 "action": "proceed or ask_for_more_context or escalate",
 "reason": "short explanation"
}
`;

    const policyOutput = await runAgent(policyPrompt);
    const cleanedPolicyOutput = policyOutput.replace(/```json|```/g, "").trim();
    const policyDecision = JSON.parse(cleanedPolicyOutput);

    console.log("\n--- Policy Decision ---");
    console.log(policyDecision);

    if (policyDecision.action === "proceed") {
      const supportPrompt = `
You are a helpful planning agent.

The Genius asked:
"${userRequest}"

Give:
1. A short helpful response
2. 3 practical steps
3. One best next move

Keep it clear and encouraging.
`;

      const supportOutput = await runAgent(supportPrompt);

      console.log("\n--- Agent Response ---");
      console.log(supportOutput);
    } else if (policyDecision.action === "ask_for_more_context") {
      const followUpPrompt = `
You are a Context Agent.

The Genius asked:
"${userRequest}"

Write one short follow-up question that would help the system give a more useful and trustworthy answer.
`;

      const followUpOutput = await runAgent(followUpPrompt);

      console.log("\n--- Follow-Up Needed ---");
      console.log(followUpOutput);
    } else if (policyDecision.action === "escalate") {
      console.log("\n--- Escalation Message ---");
      console.log("This request needs more careful support. A human expert, trusted adult, or qualified professional should review this situation.");
      console.log("The system should avoid giving high-stakes advice here.");
    }\
  } catch (error) {
    console.log("Something went wrong while running the policy-aware agent.");
    console.error(error);
  }

  rl.close();
});
```
#### **How to Run the App**
```
node policyAwareAgent.js
```
#### **Guided Practice Teaching Points**

-   Why the policy check comes before the main response
-   Why branching logic matters in responsible AI systems
-   Why JSON is useful for structured system decisions
-   Why a follow-up question can be a smarter response than a rushed answer
-   Why escalation is part of trust, not failure

#### **Guided Practice Discussion**

-   Why is the Policy Agent useful?
-   What made the system more trustworthy after adding policy logic?
-   Why is escalation sometimes the best product decision?
-   What kinds of systems need stronger guardrails?

### 4. **Independent Practice (Time: 30 minutes)**

-   **Objective:** Geniuses independently add policy and guardrail logic to their own agentic system.
-   This continues the Week 4 mini-project.

#### **Mini-Project Title**

**Agentic AI System --- Day 4 Policy and Guardrail Upgrade**

#### **Independent Task**

Each Genius updates their existing agentic or multi-agent system by adding at least **2 policy or guardrail improvements**.

Examples:

-   classify requests by risk level
-   add a follow-up question when context is missing
-   add a warning or trust note
-   block or redirect a high-stakes category
-   require more details before planning
-   create a simple escalation path

Possible use cases:

-   study agent asks for more information if the goal is too vague
-   career agent avoids pretending to make life decisions for the user
-   wellness agent avoids giving medical advice
-   finance-related agent redirects high-stakes investment advice

#### **Required Deliverables**

-   A working updated `.js` file for the agent system
-   A working `.env` file configured locally
-   A workflow with:
    -   policy logic or branching
    -   at least 2 guardrail improvements
    -   clearer trust-aware behavior
-   A short written reflection:
    -   What policy rules did you add?
    -   Why do those rules matter?
    -   How did they make the system stronger?

#### **Facilitator Support Moves**

-   Help Geniuses define where the biggest risk is in their product
-   Ask:
    -   What requests are low-risk?
    -   What requests need more context?
    -   What requests should not get a casual answer?
    -   Where should the system slow down?
-   Encourage Geniuses to make the rules simple and realistic

### 5. **Closure (Time: 15 minutes)**

-   **Objective:** Reinforce that policies and guardrails are key parts of trustworthy AI system design.
-   Bring the class together for a final share-out.
-   Ask 3--5 Geniuses to share:
    -   one policy rule they added
    -   one kind of request their system now handles more carefully
    -   one way trust improved
-   Lead a closing discussion:
    -   What makes a guardrail useful?
    -   Why does a trustworthy system sometimes say less, not more?
    -   How do policies help AI systems feel more responsible?
-   Preview the next lesson:
    -   Geniuses will use flex day to strengthen their full agentic system, improve policies, and showcase what they built.

**Assessment:**
---------------

Student learning will be assessed through:

-   Participation in the icebreaker and discussion
-   Reflection responses during direct instruction
-   Completion of the guided policy-aware workflow build
-   Completion of an independent system upgrade with guardrails
-   Final share-out and explanation of responsible system behavior

### **Exit Ticket**

1.  What is an AI policy?
2.  What is one example of a guardrail?
3.  Why might "ask for more context" be better than answering immediately?

**Extra Activities:**
---------------------

-   Geniuses who finish early can:
    -   add more detailed risk categories
    -   add a separate Safety Agent
    -   create different escalation messages for different risks
    -   add a user-facing warning note
    -   combine context checking and policy checking
    -   return the policy decision in a cleaner formatted way
-   Add a confidence label
-   Add a "low, medium, high" risk scale
-   Add a second follow-up question if context is still missing
-   Add a final log that explains why the system made its decision

**Reflection / Takeaways:**
---------------------------

This lesson works best when Geniuses understand that policies are not just something written in a handbook. They are built into how the product behaves. Day 4 introduces an important systems design mindset: responsible AI means designing for judgment, limits, and careful action. By the end of the lesson, Geniuses should see that a stronger AI system is not one that answers everything. It is one that knows when to proceed, when to pause, and when to bring in more support.

**Facilitator Notes**
---------------------

-   Keep using **Geniuses** consistently in examples and discussion.
-   Reinforce that guardrails are part of product design, not just technical rules.
-   Encourage simple, understandable policy logic before adding complexity.
-   Help Geniuses think carefully about risk, trust, and user safety.
-   Remind Geniuses that Day 5 will be flex day for strengthening, polishing, and showcasing the full system.

**Week 4 Day 4 Mini-Project Connection**
----------------------------------------

By the end of Day 4, each Genius should have:

-   A stronger agentic or multi-agent system
-   Policy logic or branching behavior
-   At least 2 guardrail improvements
-   A clearer sense of when the system should proceed, ask, or escalate
-   A more trustworthy and realistic AI system design
-   A strong foundation for Week 4 flex day and showcase
