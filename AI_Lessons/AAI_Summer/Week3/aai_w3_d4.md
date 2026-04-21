<img src="https://github.com/Hgp-GeniusLabs/Curriculum/blob/10734f2c827128dde773ea4f266d154d46977866/Org-Wide/Assets/hgp_logo_original.png" width="150"/>

Lesson Plan: Applied AI Week 3, Day 4 --- Product Flows, Wireframing, and Intentional AI Interface Redesign
=========================================================================================================

**Duration:**
-------------

3 hours

**Lesson Overview:**
--------------------

On Day 4, Geniuses bring together everything they have learned so far in Week 3 by redesigning their AI product flow and interface more intentionally. After exploring UI/UX, culturally rooted design, and user insight, Geniuses now focus on structure: what the user sees first, what they do next, what the product returns, and how the overall experience should feel from beginning to end. The lesson emphasizes that strong AI products are not only visually clean or culturally aware. They also guide users through a thoughtful flow that reduces confusion and increases clarity, trust, and usefulness.

During guided practice, the class maps a product flow and then turns that flow into a clearer wireframe and coded interface using HTML, CSS, and JavaScript. Geniuses learn how to organize screens, sections, states, and user actions before adding more complexity. During independent practice, each Genius redesigns part of their own AI product by improving the sequence, layout, and logic of the experience based on everything they have learned this week.

**Objectives:**
---------------

-   Explain what a product flow is and why it matters in AI products.
-   Identify friction points in a user journey and redesign them more intentionally.
-   Create a simple wireframe or structured layout plan for an AI product.
-   Improve a product by redesigning the order, clarity, and flow of user actions and responses.
-   Use HTML, CSS, and JavaScript to implement a stronger product flow.
-   Reflect on how product flow affects trust, clarity, and user success.

**Materials:**
--------------

-   Laptops for all Geniuses
-   VS Code installed
-   Internet access
-   Projector or display
-   Whiteboard and markers
-   Slide deck for lecture and discussion
-   Reflection journal or digital notes
-   Browser for viewing local web apps
-   Existing Week 3 project files
-   Paper and pencil or sticky notes for quick wireframing
-   Optional sample wireframes or simple product flow examples

**Standards:**
--------------

-   Computational Thinking: Break down user journeys into clear steps, decisions, and outcomes.
-   Computer Science Practices: Plan, redesign, and improve a digital product through structured iteration.
-   Web Development: Use HTML, CSS, and JavaScript to support better product flow and layout.
-   Digital Literacy: Evaluate how design structure affects usability and trust.
-   Career Readiness: Practice planning, critique, communication, and user-centered problem-solving.
-   Entrepreneurship and Innovation: Improve a product by making its experience clearer, more intentional, and more user-friendly.

**Lesson Activity:**
--------------------

### 1. **Introduction (Time: 25 minutes)**

-   **Objective:** Energize Geniuses and introduce the idea that strong AI products guide the user clearly from step to step.
-   Start with an icebreaker called **"What Happens Next?"**
-   This should be the first thing and the most fun thing to wake Geniuses up and get them ready for the lesson.

#### **Icebreaker Option A: Physical Sequencing**

-   Choose a simple AI product scenario and give different Geniuses different "steps" in the flow.
-   Example roles:
    -   User sees homepage
    -   User reads instructions
    -   User types input
    -   User clicks button
    -   Product shows loading state
    -   Product displays result
    -   User decides what to do next
-   Mix up the order on purpose and ask the class to physically rearrange the steps into a stronger sequence.
-   After the sequence is corrected, ask:
    -   What step should come first?
    -   Where would a user get confused?
    -   What is missing?
    -   What should happen after the AI gives a result?

#### **Icebreaker Option B: Product Flow Sort**

-   Write product steps on the board or cards.
-   Ask small groups to put them in the best order for a strong AI experience.
-   Example steps:
    -   "See example input"
    -   "Type your notes"
    -   "Understand what the tool does"
    -   "Read result"
    -   "See trust note"
    -   "Click generate"
    -   "Get next step guidance"
-   Discuss how different sequences change the user experience.

#### **Transition**

-   Say:
    -   "A product is not just a page. It is a journey. If the journey is messy, the user feels it."
-   Ask:
    -   What should the user know first?
    -   What should happen after the result appears?
    -   What makes a product flow feel smooth?

### 2. **Direct Instruction (Time: 50 minutes)**

-   **Objective:** Help Geniuses understand product flow, wireframing, and how strong interface structure supports better user experiences.
-   Use slides to guide instruction and pause often for examples and discussion.

#### **Suggested Slide Flow**

-   **Slide 1: Day 4 Focus --- Design the Journey**
    -   Today is about product flow, layout planning, and intentional interface design
-   **Slide 2: What Is a Product Flow?**
    -   A product flow is the path a user takes through the product
    -   It includes:
        -   what they see first
        -   what they do
        -   what the product does
        -   what happens next
-   **Slide 3: Why Flow Matters in AI Products**
    -   AI can already feel uncertain
    -   weak flow adds confusion
    -   strong flow gives the user confidence, clarity, and direction
-   **Slide 4: Common Product Flow Problems**
    -   unclear first step
    -   too many choices at once
    -   confusing buttons
    -   weak instructions
    -   output appears without context
    -   no next step after the result
-   **Slide 5: What Is a Wireframe?**
    -   A wireframe is a simple plan for layout and flow
    -   It helps builders think before over-designing
    -   It focuses on structure, not decoration
-   **Slide 6: What a Good Wireframe Clarifies**
    -   where the headline goes
    -   where the input goes
    -   where the output goes
    -   what the main action is
    -   what the user sees first
    -   what information supports trust
-   **Slide 7: Key Product Flow Questions**
    -   What is the user trying to do?
    -   What is the first useful action?
    -   What could confuse them?
    -   What should happen after the AI responds?
    -   What helps the user move forward?
-   **Slide 8: AI Product States**
    -   before input
    -   while loading
    -   after output
    -   if there is an error
    -   if the user needs help
    -   Products should be designed for all these states
-   **Slide 9: Strong AI Product Structure**
    -   onboarding or purpose
    -   user input
    -   main action
    -   result
    -   trust note
    -   next step or follow-up action
-   **Slide 10: Week 3 Mini-Project Growth**
    -   Day 1: better UX
    -   Day 2: cultural grounding
    -   Day 3: user insight
    -   Day 4: redesign the product flow and structure

#### **Discussion Questions**

-   Why do some products feel easy to use right away?
-   What makes a product flow confusing?
-   Why should a wireframe come before major redesign decisions?
-   What should happen after an AI result appears?
-   Why do AI tools need more than just input and output?

#### **Reflection Prompt**

-   Have Geniuses write for 4 minutes:
    -   "Where does your product still feel awkward, rushed, or confusing in the user journey?"

### 3. **Guided Practice (Time: 55 minutes)**

-   **Objective:** Help Geniuses map a product flow and implement a stronger interface structure using HTML, CSS, and JavaScript.
-   Explain that today's build is about improving the whole journey, not just one section.

#### **Guided Practice Build**

Use the existing Week 3 project or create a folder called `ai-product-flow-redesign`.

#### **Project Goal**

Take a simple AI product and redesign it so that it includes:

-   a stronger onboarding section
-   a clear input area
-   a loading state
-   a structured output area
-   a "what to do next" section
-   a trust note or guidance message

#### **Setup Steps**

1.  Open the project in VS Code.
2.  Use the existing files or create:
    -   `index.html`
    -   `style.css`
    -   `script.js`
3.  Sketch a quick wireframe before coding.
4.  Build the improved product structure.

#### **Sample `index.html`**
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Pathway AI</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>
  <main class="app-shell">
    <section class="hero-card">
      <p class="eyebrow">AI Planning Support</p>
      <h1>Get from scattered thoughts to a clear next move.</h1>
      <p class="hero-text">
        Pathway AI helps Geniuses organize ideas, identify priorities, and move forward with more clarity.
      </p>
    </section>

    <section class="flow-card">
      <div class="step-label">Step 1</div>
      <h2>Understand the tool</h2>
      <p class="helper-text">
        This tool works best when you paste a real list of tasks, ideas, or responsibilities you are trying to organize.
      </p>

      <div class="example-box">
        <strong>Example Input:</strong>
        <p>
          Need to finish my science assignment, check in with my coach, and plan out what I need for the weekend event.
        </p>
      </div>
    </section>

    <section class="flow-card">
      <div class="step-label">Step 2</div>
      <h2>Enter your notes</h2>
      <label for="userInput">Your notes</label>
      <textarea
        id="userInput"
        placeholder="Type what you are juggling right now..."
      ></textarea>

      <div class="button-row">
        <button id="generateButton">Help Me Sort It Out</button>
        <button id="clearButton" class="secondary-button">Clear</button>
      </div>

      <p id="statusMessage" class="status-message"></p>
    </section>

    <section id="resultSection" class="flow-card hidden">
      <div class="step-label">Step 3</div>
      <h2>Your organized result</h2>

      <div class="result-card">
        <h3>Main Focus</h3>
        <p id="summaryOutput"></p>
      </div>

      <div class="result-card">
        <h3>Suggested Steps</h3>
        <p id="actionsOutput"></p>
      </div>

      <div class="result-card">
        <h3>Best Next Move</h3>
        <p id="nextStepOutput"></p>
      </div>
    </section>

    <section id="nextSection" class="flow-card hidden">
      <div class="step-label">Step 4</div>
      <h2>What to do next</h2>
      <p id="followUpText">
        Review the result, choose one action to start with, and adjust the plan based on your real priorities.
      </p>

      <div class="trust-note">
        <strong>Product Note:</strong> AI can help bring structure, but you should always decide what matters most in your real life.
      </div>
    </section>
  </main>

  <script src="script.js"></script>
</body>
</html>
```
#### **Sample `style.css`**
```
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: Arial, sans-serif;
  background: #f4f8ff;
  color: #1f2933;
  line-height: 1.6;
  padding: 32px 16px;
}

.app-shell {
  max-width: 920px;
  margin: 0 auto;
}

.hero-card,
.flow-card {
  background: white;
  border-radius: 18px;
  padding: 28px;
  box-shadow: 0 10px 24px rgba(0, 0, 0, 0.08);
  margin-bottom: 24px;
}

.eyebrow,
.step-label {
  display: inline-block;
  color: #2563eb;
  font-weight: bold;
  margin-bottom: 10px;
}

.hero-card h1,
.flow-card h2 {
  margin-bottom: 12px;
}

.hero-card h1 {
  font-size: 2.2rem;
}

.hero-text,
.helper-text {
  color: #52606d;
}

.example-box {
  margin-top: 16px;
  background: #eff6ff;
  border-left: 4px solid #2563eb;
  border-radius: 12px;
  padding: 14px 16px;
}

.example-box p {
  margin-top: 6px;
}

label {
  display: block;
  font-weight: bold;
  margin-bottom: 8px;
}

textarea {
  width: 100%;
  min-height: 140px;
  border: 1px solid #cbd5e1;
  border-radius: 12px;
  padding: 16px;
  font-size: 1rem;
  margin: 12px 0 16px;
  resize: vertical;
}

.button-row {
  display: flex;
  gap: 12px;
  flex-wrap: wrap;
}

button {
  border: none;
  border-radius: 10px;
  padding: 12px 18px;
  background: #2563eb;
  color: white;
  font-size: 1rem;
  cursor: pointer;
}

button:hover {
  background: #1d4ed8;
}

.secondary-button {
  background: #e2e8f0;
  color: #1f2933;
}

.secondary-button:hover {
  background: #cbd5e1;
}

.status-message {
  margin-top: 14px;
  min-height: 24px;
  font-weight: bold;
  color: #2563eb;
}

.result-card {
  background: #f8fafc;
  border-radius: 14px;
  padding: 18px;
  border: 1px solid #e5e7eb;
  margin-top: 14px;
}

.result-card h3 {
  margin-bottom: 8px;
  color: #1d4ed8;
}

.trust-note {
  margin-top: 16px;
  padding: 14px 16px;
  background: #eefcf5;
  border-left: 4px solid #16a34a;
  border-radius: 10px;
  color: #334155;
}

.hidden {
  display: none;
}

@media (max-width: 640px) {
  .hero-card h1 {
    font-size: 1.8rem;
  }

  .hero-card,
  .flow-card {
    padding: 20px;
  }
}
```
#### **Sample `script.js`**
```
// script.js
// Applied AI Week 3 Day 4
// This script supports a clearer product flow with result and follow-up states.

const userInput = document.getElementById("userInput");
const generateButton = document.getElementById("generateButton");
const clearButton = document.getElementById("clearButton");
const statusMessage = document.getElementById("statusMessage");
const resultSection = document.getElementById("resultSection");
const nextSection = document.getElementById("nextSection");

const summaryOutput = document.getElementById("summaryOutput");
const actionsOutput = document.getElementById("actionsOutput");
const nextStepOutput = document.getElementById("nextStepOutput");

generateButton.addEventListener("click", () => {
  const text = userInput.value.trim();

  if (text === "") {
    statusMessage.textContent = "Please enter your notes first.";
    resultSection.classList.add("hidden");
    nextSection.classList.add("hidden");
    return;
  }

  statusMessage.textContent = "Building your plan...";
  resultSection.classList.add("hidden");
  nextSection.classList.add("hidden");

  setTimeout(() => {
    summaryOutput.textContent = "Your notes show that you need structure so you can focus on the most important responsibility first.";
    actionsOutput.textContent = "1. Identify the most urgent deadline. 2. Separate school, personal, and event-related tasks. 3. Start with one action that lowers pressure quickly.";
    nextStepOutput.textContent = "Take the task with the nearest deadline and commit to one small action on it today.";

    statusMessage.textContent = "Your plan is ready.";
    resultSection.classList.remove("hidden");
    nextSection.classList.remove("hidden");
  }, 900);
});

clearButton.addEventListener("click", () => {
  userInput.value = "";
  summaryOutput.textContent = "";
  actionsOutput.textContent = "";
  nextStepOutput.textContent = "";
  statusMessage.textContent = "";
  resultSection.classList.add("hidden");
  nextSection.classList.add("hidden");
});
```
#### **Guided Practice Teaching Points**

-   Why the user journey should be intentional from first screen to next action
-   Why wireframes help simplify thinking before styling
-   Why strong products design for before, during, and after the AI response
-   Why "what happens next" matters for usefulness
-   Why follow-up guidance helps users act on the output

#### **Guided Practice Discussion**

-   How did this version improve the flow?
-   What did adding a Step 4 do for the user experience?
-   What still feels like it could be smoother?
-   How can wireframing help prevent messy design choices?

### 4. **Independent Practice (Time: 30 minutes)**

-   **Objective:** Geniuses independently redesign the flow of their own AI product and implement a clearer wireframe-based structure.
-   This continues the Week 3 mini-project.

#### **Mini-Project Title**

**AI Product Redesign --- Day 4 Product Flow and Wireframe Build**

#### **Independent Task**

Each Genius must:

-   sketch a basic wireframe of their product before coding
-   identify at least 2 weak points in their current flow
-   redesign the structure of the product so the experience feels clearer and more intentional

Their redesigned product should include:

-   a clearer beginning state
-   a stronger action step
-   a more structured result state
-   a better "what next" section or follow-up action
-   at least one flow improvement based on user insight from Day 3

#### **Required Deliverables**

-   A working `index.html`
-   A working `style.css`
-   A working `script.js`
-   A simple wireframe or layout sketch
-   A redesigned interface with:
    -   improved flow
    -   improved section sequence
    -   clearer result state
    -   follow-up or next action guidance
-   A short written reflection:
    -   What part of your flow changed most?
    -   What user problem did this redesign solve?
    -   How does the new structure help users better?

#### **Facilitator Support Moves**

-   Ask:
    -   What does the user need to understand first?
    -   Where do they take action?
    -   What happens when the AI finishes?
    -   What should the user do next?
    -   What did user feedback suggest needed to change?
-   Encourage Geniuses to simplify cluttered flows and design fewer, clearer steps

### 5. **Closure (Time: 20 minutes)**

-   **Objective:** Reinforce that product structure and flow are major parts of AI product quality.
-   Bring the class together for a final share-out.
-   Ask 3--5 Geniuses to show:
    -   one part of their wireframe
    -   one flow problem they fixed
    -   one improvement to what the user sees after the result
    -   one reason the product feels smoother now
-   Lead a closing discussion:
    -   What makes a product flow feel clear?
    -   Why is "what happens next" important in AI products?
    -   How did wireframing help your design thinking?
-   Preview the next lesson:
    -   Day 5 will be a flex day for redesign polish, critique, final improvements, and showcase.

**Assessment:**
---------------

Student learning will be assessed through:

-   Participation in the icebreaker and discussion
-   Reflection responses during direct instruction
-   Completion of the guided wireframe and flow redesign build
-   Completion of an independent product flow redesign
-   Final share-out and explanation of flow improvements

### **Exit Ticket**

1.  What is a product flow?
2.  Why does "what happens next" matter in AI products?
3.  What part of your product flow improved most today?

**Extra Activities:**
---------------------

-   Geniuses who finish early can:
    -   add a progress indicator
    -   add multiple result states
    -   improve mobile flow
    -   add a restart or "try again" section
    -   build a second flow for a different type of user input
    -   turn their wireframe into a second page mockup
-   Add anchor navigation between steps
-   Add a "tips for better results" section
-   Add empty-state guidance before users enter input
-   Add conditional messaging based on user input length

**Reflection / Takeaways:**
---------------------------

This lesson works best when Geniuses realize that product design is not only about how something looks. It is also about the path the user takes through it. AI products especially need strong structure because users need clarity before, during, and after the AI response. By the end of Day 4, Geniuses should understand that wireframing and flow design help products feel smoother, more useful, and more trustworthy. A stronger journey leads to a stronger product.

**Facilitator Notes**
---------------------

-   Keep using **Geniuses** consistently in examples and discussion.
-   Reinforce that wireframes are for structure, not perfection.
-   Encourage Geniuses to design with fewer, clearer steps.
-   Help Geniuses connect Day 3 user insights to Day 4 flow changes.
-   Remind Geniuses that Day 5 will be the redesign flex day and showcase.

**Week 3 Day 4 Mini-Project Connection**
----------------------------------------

By the end of Day 4, each Genius should have:

-   A simple wireframe or layout sketch
-   A clearer product flow
-   A better beginning state for the user
-   A stronger result state
-   A clearer follow-up or next action section
-   At least one flow improvement based on user insight
-   A more intentional and user-centered AI product redesign
