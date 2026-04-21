<img src="https://github.com/Hgp-GeniusLabs/Curriculum/blob/10734f2c827128dde773ea4f266d154d46977866/Org-Wide/Assets/hgp_logo_original.png" width="150"/>

Lesson Plan: Applied AI Week 4, Day 5 --- Agent System Studio, Guardrail Polish, and Showcase
===========================================================================================

**Duration:**
-------------

3 hours

**Lesson Overview:**
--------------------

Day 5 is a flex day focused on strengthening, extending, and showcasing the agentic AI systems Geniuses have been building all week. By this point, Geniuses have explored planner agents, multi-agent workflows, data quality and trust, and policy-aware guardrails. Today is about turning those ideas into a stronger, more complete AI system. Geniuses will use studio-style work time to improve the parts of their systems that matter most: clearer agent roles, better handoffs, stronger context gathering, smarter policy behavior, cleaner outputs, and more trustworthy system design.

During guided practice, the class will apply a system review framework to an agentic workflow and then improve it using targeted upgrades. During independent practice, each Genius will choose meaningful improvements for their own agentic system and prepare a short showcase. The lesson ends with demos, reflection, and discussion around what makes an AI system not just capable, but well-designed, trustworthy, and useful in the real world.

**Objectives:**
---------------

-   Reflect on how agentic AI systems improve through iteration, critique, and stronger system design.
-   Identify meaningful upgrades that improve multi-agent coordination, trust, and usefulness.
-   Improve an AI system by refining agent roles, handoffs, context, policy logic, or output structure.
-   Strengthen a Node and OpenAI-powered workflow into a more polished system.
-   Practice presenting an AI system clearly in terms of goal, agents, trust, and policy behavior.
-   Showcase a more complete and responsible agentic AI system.

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
-   Existing Week 4 Day 1--4 project files
-   Optional critique worksheet or system review checklist

**Standards:**
--------------

-   Computational Thinking: Improve a system by refining steps, handoffs, logic, and decision rules.
-   Computer Science Practices: Test, critique, and strengthen a multi-step AI workflow.
-   Programming: Refine a Node and OpenAI-powered system with clearer orchestration and safer behavior.
-   Digital Literacy: Evaluate whether an AI system is useful, trustworthy, and appropriately bounded.
-   Career Readiness: Practice systems thinking, critique, iteration, and technical communication.
-   Entrepreneurship and Innovation: Improve an AI system so it better solves a real task with structure, trust, and clear product logic.

**Lesson Activity:**
--------------------

### 1. **Introduction (Time: 20 minutes)**

-   **Objective:** Energize Geniuses and frame the day around meaningful system improvement, not random feature adding.
-   Start with an icebreaker called **"Keep It, Fix It, or Add a Guardrail?"**
-   This should be the first thing and the most fun thing to wake Geniuses up and get them ready for the lesson.

#### **Icebreaker Option A: Physical Movement**

-   Label three parts of the room:
    -   **Keep It**
    -   **Fix It**
    -   **Add a Guardrail**
-   Read agent system situations aloud and have Geniuses move to the option that best matches what should happen next.
-   Example prompts:
    -   A Planner Agent makes good steps, but they are too generic
    -   A multi-agent workflow works, but the handoff between agents is messy
    -   A system gives useful output, but never asks for missing context
    -   A system handles low-risk requests well and should stay simple
    -   A wellness agent gives plans, but does not warn users that it is not medical advice
    -   A career workflow is strong, but the Checker Agent does almost nothing
    -   A system gives a result, but does not explain what the user should do next
    -   A productivity agent already works well for clear low-risk tasks
-   After each round, ask:
    -   Why keep it?
    -   Why fix it?
    -   Why does this need a guardrail?
    -   What would improve trust most?

#### **Icebreaker Option B: Rapid System Critique**

-   Put short workflow summaries on the board.
-   Ask Geniuses to quickly name:
    -   one strength
    -   one weak point
    -   one improvement type:
        -   role improvement
        -   context improvement
        -   policy improvement
        -   output improvement
-   Discuss which changes would matter most.

#### **Transition**

-   Say:
    -   "A first version proves the concept. A polished system proves the builder."
-   Ask:
    -   What still feels weakest in your system?
    -   What change would make the biggest difference for trust or usefulness?

### 2. **Direct Instruction (Time: 35 minutes)**

-   **Objective:** Help Geniuses identify meaningful ways to strengthen an agentic AI system and prepare for showcase thinking.
-   Use slides to guide the lesson and frame flex day choices.

#### **Suggested Slide Flow**

-   **Slide 1: Day 5 Focus --- Improve, Strengthen, Showcase**
    -   Today is about polishing your AI system and making smarter design decisions
-   **Slide 2: What Makes an Agentic System Feel Strong?**
    -   clear goal
    -   clear agent roles
    -   strong handoffs
    -   good context
    -   useful outputs
    -   clear policy behavior
    -   trust-aware boundaries
-   **Slide 3: Common Weak Spots in Agent Systems**
    -   vague agent roles
    -   repetitive or overlapping agents
    -   weak handoffs
    -   poor context gathering
    -   messy output formatting
    -   no clear guardrails
    -   weak escalation behavior
-   **Slide 4: Strong Upgrade Categories**
    -   **Role Design**
    -   **Workflow Handoffs**
    -   **Context Gathering**
    -   **Output Structure**
    -   **Policy and Guardrails**
    -   **Trust and Transparency**
-   **Slide 5: Role Design Improvements**
    -   make agent jobs clearer
    -   reduce overlap
    -   give each agent a real purpose
    -   strengthen specialization
-   **Slide 6: Trust and Policy Improvements**
    -   ask follow-up questions sooner
    -   add escalation logic
    -   add trust notes
    -   clarify low-risk vs higher-risk behavior
    -   avoid overconfident outputs
-   **Slide 7: Output and UX Improvements**
    -   cleaner structured formatting
    -   clearer stage labels
    -   final recommendation section
    -   better explanation of what the system did
    -   clearer next move for the user
-   **Slide 8: Showcase Thinking**
    -   Can you clearly explain:
        -   the goal of the system?
        -   what each agent does?
        -   what kind of data or context it needs?
        -   what guardrails it uses?
        -   why the system is stronger now?
-   **Slide 9: Build Priorities**
    -   improve the core workflow first
    -   fix weak trust points
    -   make the system easier to understand
    -   add features only if they improve the experience
-   **Slide 10: Finish Week 4 Strong**
    -   A strong AI system is not just smart
    -   It is structured, useful, and trustworthy

#### **Discussion Questions**

-   What makes an upgrade meaningful instead of random?
-   Which part of your system matters most for trust?
-   Why is output structure important in agent workflows?
-   What makes a handoff between agents strong?
-   How do policies change the quality of the whole system?

#### **Reflection Prompt**

-   Have Geniuses write for 4 minutes:
    -   "What are the two most important upgrades your system still needs before showcase?"

### 3. **Guided Practice (Time: 40 minutes)**

-   **Objective:** Help Geniuses apply a system review framework and improve an agentic workflow using targeted upgrades.
-   Explain that today's guided practice is about reviewing the whole system, not just one file.

#### **Guided Practice Build**

Use an existing Week 4 project and apply a system review framework before editing code.

#### **System Review Framework**

Ask the class to review a sample agentic workflow using these 5 prompts:

1.  Is the system goal clear?
2.  Does each agent have a distinct role?
3.  Does the system gather enough context before acting?
4.  Does the system know when to proceed, ask, or escalate?
5.  Is the final output useful and easy to understand?

#### **Project Goal**

Take a simple agent workflow and improve it by:

-   strengthening an agent role
-   improving handoff clarity
-   improving context gathering
-   improving policy behavior
-   improving final output formatting

#### **Sample Improvement Pattern**

The class will add:

-   a **Context Agent** before the Planner Agent
-   a clearer **Policy Agent** branch
-   a stronger final **Manager Agent** summary
-   clearer output labels for each stage

#### **Sample `agentStudioUpgrade.js`**
```
// agentStudioUpgrade.js
// Applied AI Week 4 Day 5
// This script shows a stronger agent workflow with context gathering,
// policy checking, planning, and final synthesis.

require("dotenv").config();
const OpenAI = require("openai");

const client = new OpenAI({
  apiKey: process.env.OPENAI_API_KEY,
});

// Helper function to run an agent prompt
async function runAgent(prompt) {
  const response = await client.responses.create({
    model: "gpt-4.1-mini",
    input: prompt,
  });

  return response.output_text;
}

async function main() {
  const userGoal = "Help me plan a school fundraiser for 60 people next month.";
  const userContext = `
- We already have a school gym reserved
- We still need food, volunteers, and promotion
- Our budget is limited
- We want the plan to feel realistic for students
`;

  try {
    const contextPrompt = `
You are a Context Agent.

User Goal:
"${userGoal}"

User Context:
${userContext}

Your job is to identify:
1. The most important facts
2. Missing information
3. Constraints that matter most

Return in this format:

Important Facts:
- ...

Missing Information:
- ...

Key Constraints:
- ...
`;

    const contextOutput = await runAgent(contextPrompt);

    const policyPrompt = `
You are a Policy Agent.

Review this request and context:

Goal:
"${userGoal}"

Context Analysis:
${contextOutput}

Decide:
- proceed
- ask_for_more_context
- escalate

This is a school event planning request, so treat it as low-risk unless something important is missing.

Return valid JSON in this format:
{
 "action": "proceed or ask_for_more_context or escalate",
 "reason": "short explanation"
}
`;

    const policyOutput = await runAgent(policyPrompt);
    const cleanedPolicyOutput = policyOutput.replace(/```json|```/g, "").trim();
    const policyDecision = JSON.parse(cleanedPolicyOutput);

    console.log("\n--- Context Agent Output ---");
    console.log(contextOutput);

    console.log("\n--- Policy Decision ---");
    console.log(policyDecision);

    if (policyDecision.action !== "proceed") {
      console.log("\n--- System Response ---");
      if (policyDecision.action === "ask_for_more_context") {
        console.log("The system needs more information before planning.");
      } else {
        console.log("This request should be escalated for human review.");
      }
      return;
    }

    const plannerPrompt = `
You are a Planner Agent.

Goal:
"${userGoal}"

Context Analysis:
${contextOutput}

Create:
1. A short goal summary
2. 4 practical planning step
3. A best first move

Keep it realistic and student-friendly.
`;

    const plannerOutput = await runAgent(plannerPrompt);

    const managerPrompt = `
You are a Manager Agent.

Combine the planner output below into a final polished response for a Genius.

Planner Output:
${plannerOutput}

Your job is to:
1. Present the plan clearly
2. Keep the tone supportive
3. End with one reminder about working within the budget and team capacity

Return in this format:

Final Plan:
- ...

Reminder:
- ...
`;

    const managerOutput = await runAgent(managerPrompt);

    console.log("\n--- Planner Agent Output ---");
    console.log(plannerOutput);

    console.log("\n--- Manager Agent Output ---");
    console.log(managerOutput);
  } catch (error) {
    console.log("Something went wrong while running the upgraded agent system.");
    console.error(error);
  }
}

main();
```
#### **Guided Practice Teaching Points**

-   Why a Context Agent can improve the whole workflow
-   Why a Policy Agent should often come before execution
-   Why a final Manager Agent can make outputs clearer
-   Why stronger stage labels improve understanding
-   Why polishing the system means improving coordination, not only adding more agents

#### **Guided Practice Discussion**

-   What part of this upgrade made the system feel stronger?
-   Why did the Context Agent help?
-   Why is the final Manager Agent useful?
-   What still might need improvement in a real product?

### 4. **Independent Practice (Time: 65 minutes)**

-   **Objective:** Give Geniuses time to strengthen, polish, and prepare their agentic AI system for showcase.
-   This completes the Week 4 mini-project.

#### **Mini-Project Title**

**Agentic AI System --- Day 5 Studio Polish and Showcase Prep**

#### **Independent Task**

Each Genius chooses **2--3 meaningful system upgrades** to apply to their project.

#### **Improvement Menu**

Geniuses can choose from the following:

-   improve an existing agent role
-   add a new specialized agent
-   improve handoff formatting between agents
-   add stronger context gathering
-   add a missing-info question
-   improve policy or escalation logic
-   add a caution or trust note
-   improve the final structured output
-   add a Manager Agent or Reviewer Agent
-   improve role labels in the terminal output
-   add deadline, budget, or user-type input
-   refactor repeated logic into helper functions
-   add simple JSON parsing for cleaner system decisions
-   improve error handling

#### **Required Deliverables**

-   A working updated `.js` file or files for the system
-   A working `.env` file configured locally
-   At least 2 meaningful system improvements
-   A short system summary that includes:
    -   system name
    -   user or use case
    -   list of agent roles
    -   one trust or policy feature
    -   two upgrades made today
    -   one reason the system is stronger now
-   A 1--2 minute showcase or demo plan

#### **Showcase Prep Prompt**

Ask Geniuses to prepare a short demo that answers:

-   What is your system called?
-   What goal or problem does it solve?
-   What does each agent do?
-   What kind of context does the system use?
-   What guardrails or policies does it include?
-   What did you improve today?
-   Why is the system stronger now?

#### **Facilitator Support Moves**

-   Help Geniuses choose upgrades that improve system quality, not just add complexity
-   Ask:
    -   What still feels weakest?
    -   Which handoff is the most important?
    -   Where could the system be more trustworthy?
    -   Does every agent have a real job?
    -   What will make your showcase strongest?
-   Encourage testing with multiple goals and clearer labels

### 5. **Closure (Time: 20 minutes)**

-   **Objective:** Celebrate system growth and reinforce that strong AI systems are designed through structure, trust, and iteration.
-   Bring the class together for a showcase.
-   Invite Geniuses to present individually or in small groups.
-   Each Genius should share:
    -   their system name
    -   the problem it solves
    -   their agent roles
    -   one context or data improvement
    -   one policy or guardrail improvement
    -   one reason the system is stronger now
-   After each share, invite quick audience feedback:
    -   What feels strongest?
    -   What feels most trustworthy?
    -   What role or guardrail was especially smart?
-   Lead a final reflection discussion:
    -   What did you learn this week about designing AI systems?
    -   What is the difference between an AI feature and an agentic AI system?
    -   Why do trust and policy matter in real AI products?
    -   What part of system design felt most exciting?

**Assessment:**
---------------

Student learning will be assessed through:

-   Participation in the icebreaker and discussion
-   Reflection responses during direct instruction
-   Completion of the guided system upgrade build
-   Completion of at least 2 meaningful improvements to the independent system
-   Final showcase and explanation of agent roles, context, and policy behavior
-   End-of-week reflection on trust-aware systems design

### **Exit Ticket**

1.  What is one improvement that made your system stronger today?
2.  What makes an agentic system trustworthy?
3.  What is one thing your system now does better than it did on Day 1?

**Extra Activities:**
---------------------

-   Geniuses who finish early can:
    -   add a web interface for their system
    -   add a second policy mode for stricter review
    -   add output history in the terminal or a file
    -   add a final score or confidence label
    -   add a route that shows agent stages separately
    -   split the system into multiple files for cleaner code organization
-   Add timestamps to each stage
-   Add a "why the system asked this question" message
-   Add a second use case mode
-   Add a final "system reflection" section that explains how the decision was made

**Reflection / Takeaways:**
---------------------------

This lesson works best when Geniuses see that building strong AI systems is not about making one large prompt and hoping for the best. It is about designing coordinated roles, stronger context, trust-aware behavior, and clear boundaries. Day 5 should feel like a studio day and a showcase day. By the end of Week 4, Geniuses should understand that agentic AI is really about system design: goals, roles, handoffs, data quality, guardrails, and responsibility all working together.

**Facilitator Notes**
---------------------

-   Keep using **Geniuses** consistently in prompts, examples, and discussion.
-   Let flex time feel open, but keep Geniuses focused on meaningful system improvements.
-   Encourage clarity, trust, and role quality over unnecessary complexity.
-   Help Geniuses explain not just what their system does, but why it is designed that way.
-   Reinforce that strong AI systems are built through iteration and judgment.

**Week 4 Wrap-Up**
------------------

By the end of Week 4, each Genius should have:

-   A defined agentic AI use case
-   A planner agent foundation
-   A multi-agent workflow with specialized roles
-   Better context or data gathering
-   At least one trust-aware design improvement
-   Policy or guardrail behavior
-   At least 2 meaningful flex day upgrades
-   A short system showcase or demo explanation
