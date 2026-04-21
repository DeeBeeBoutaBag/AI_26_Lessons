<img src="https://github.com/Hgp-GeniusLabs/Curriculum/blob/10734f2c827128dde773ea4f266d154d46977866/Org-Wide/Assets/hgp_logo_original.png" width="150"/>

Lesson Plan: Applied AI Week 2, Day 5 --- Flex Day, Product Polish, and AI SaaS Showcase
======================================================================================

**Duration:**
-------------

3 hours

**Lesson Overview:**
--------------------

Day 5 is a flex day focused on strengthening, extending, and showcasing the AI SaaS products Geniuses have been building all week. By this point, Geniuses have explored how businesses use AI, built a landing page, added front-end interactivity, connected their product to a Node backend, and integrated real OpenAI-powered output. Today, the goal is to make those products feel more complete, more useful, and more polished.

Geniuses will use this class to improve the most important parts of their projects. Some may strengthen the user interface, others may improve prompt quality, add new features, refine product flow, or make the experience more trustworthy. During guided practice, the class will build a reusable upgrade pattern for an AI SaaS product, including multiple AI actions, stronger UX, and cleaner organization. During independent practice, each Genius applies meaningful improvements to their own product and prepares a short showcase. The lesson ends with a product demo and reflection on how real AI SaaS products are built through iteration.

**Objectives:**
---------------

-   Reflect on how AI SaaS products improve through iteration and refinement.
-   Identify meaningful ways to strengthen an AI-powered web application.
-   Improve a full-stack AI SaaS project by adding functionality, polish, or trust-building features.
-   Practice presenting a product clearly in terms of user, value, workflow, and AI role.
-   Strengthen frontend, backend, and AI behavior in a real web product.
-   Showcase a more polished AI SaaS product to peers.

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
-   Browser for testing local web apps
-   Existing Week 2 Day 1--4 project files
-   Optional showcase rubric or peer feedback form

**Standards:**
--------------

-   Computational Thinking: Improve and extend a system based on testing and real use.
-   Computer Science Practices: Debug, refine, and enhance a full-stack AI application.
-   Web Development: Strengthen a full-stack product using HTML, CSS, JavaScript, Node, and API integration.
-   Digital Literacy: Evaluate whether a digital product is clear, useful, secure, and trustworthy.
-   Career Readiness: Practice iteration, presentation, and product communication.
-   Entrepreneurship and Innovation: Improve a product based on value, usability, and real user experience.

**Lesson Activity:**
--------------------

### 1. **Introduction (Time: 20 minutes)**

-   **Objective:** Energize Geniuses and frame the day around iteration, polish, and real product thinking.
-   Start with an icebreaker called **"Keep It, Fix It, Add It."**
-   This should be the first and most energetic part of the lesson.

#### **Icebreaker Option A: Physical Movement**

-   Label three areas of the room:
    -   **Keep It**
    -   **Fix It**
    -   **Add It**
-   Read different product features or situations aloud and have Geniuses move to the area that best matches what should happen.
-   Example prompts:
    -   A button works, but the label is confusing
    -   The AI gives good output, but the user has no loading feedback
    -   The product has one strong feature and no second action
    -   The site looks clean, but mobile layout breaks
    -   The app has good output, but no trust or caution note
    -   The user can paste text, but there is no reset button
    -   The AI output is strong, but the site still looks unfinished
-   After each round, ask:
    -   Why keep it?
    -   Why fix it?
    -   Why add something new?
    -   What matters more right now, polish or more features?

#### **Icebreaker Option B: Rapid Product Critique**

-   Show a few example product decisions on the board and have Geniuses vote:
    -   keep it
    -   fix it
    -   add to it
-   Discuss which changes improve the real user experience most.

#### **Transition**

-   Say:
    -   "A first version proves the idea. A polished version proves the builder."
-   Ask:
    -   What still feels weakest in your product?
    -   What would make your product feel more real today?

### 2. **Direct Instruction (Time: 35 minutes)**

-   **Objective:** Help Geniuses identify smart improvement strategies and prepare for showcase thinking.
-   Use slides to guide the lesson and frame flex day choices.

#### **Suggested Slide Flow**

-   **Slide 1: Day 5 Focus --- Improve, Extend, Showcase**
    -   Today is about meaningful upgrades and clear product presentation
-   **Slide 2: What Makes a Product Feel More Real?**
    -   clearer UX
    -   stronger output
    -   better structure
    -   more flexibility
    -   stronger trust signals
    -   smoother workflow
-   **Slide 3: Common Weak Spots in AI SaaS Projects**
    -   unclear instructions
    -   weak prompt logic
    -   confusing output
    -   poor styling
    -   missing loading or error states
    -   only one narrow use case
-   **Slide 4: Strong Upgrade Categories**
    -   **Frontend UX**
    -   **Prompt Quality**
    -   **Backend Features**
    -   **Output Structure**
    -   **Trust and Safety**
    -   **Code Quality**
-   **Slide 5: Frontend Upgrade Ideas**
    -   better section spacing
    -   stronger headings
    -   improved buttons
    -   mobile responsiveness
    -   reset button
    -   tabbed or multiple action layout
-   **Slide 6: Backend and AI Upgrade Ideas**
    -   multiple AI routes
    -   multiple output modes
    -   stronger structured JSON
    -   better prompt instructions
    -   more specific product behavior
    -   better error handling
-   **Slide 7: Trust-Building Upgrade Ideas**
    -   caution note
    -   explanation of what AI is doing
    -   reminder to review important results
    -   user guidance for better input
-   **Slide 8: Showcase Thinking**
    -   Can you clearly explain:
        -   who the product is for?
        -   what problem it solves?
        -   how the user interacts with it?
        -   why AI is the right fit?
        -   what makes it trustworthy?
-   **Slide 9: Build Priorities**
    -   fix what is weak first
    -   improve what users see and feel most
    -   add features only if they support the main product goal
-   **Slide 10: Finish Strong**
    -   A polished product shows discipline, judgment, and product thinking

#### **Discussion Questions**

-   What part of your product still feels weakest?
-   What upgrade would add the most value for the user?
-   What makes an upgrade meaningful instead of random?
-   What makes a product demo feel polished?
-   What would make someone believe your product could be real?

#### **Reflection Prompt**

-   Have Geniuses write for 4 minutes:
    -   "What are the two most important upgrades your product still needs, and why?"

### 3. **Guided Practice (Time: 40 minutes)**

-   **Objective:** Help Geniuses learn a reusable AI SaaS improvement pattern they can apply to their own product.
-   Explain that today's code-along is about extending and polishing, not rebuilding from scratch.

#### **Guided Practice Build**

Use the existing project folder and add a second AI action plus a stronger UX flow.

#### **Project Goal**

Upgrade the product so it can:

-   support more than one AI action
-   give clearer user feedback
-   organize the UI more effectively
-   feel more like a real SaaS tool

#### **Example Upgrade Pattern**

The class will add:

-   a dropdown menu for output type
-   multiple backend prompt paths
-   better status messaging
-   a reset button

#### **Step 1: Update `index.html`**

Add a dropdown and reset button inside the demo section:
```
<section class="demo-section" id="demo">
  <h3>Try the Product Demo</h3>
  <p class="demo-description">
    Paste your notes below and choose what kind of AI help you want.
  </p>

  <label for="taskType">Choose an AI action:</label>
  <select id="taskType">
    <option value="organize">Organize Notes</option>
    <option value="summarize">Summarize Text</option>
    <option value="nextsteps">Generate Next Steps</option>
  </select>

  <textarea
    id="userInput"
    placeholder="Example: Team meeting on Friday. Finish logo update, send budget draft, and follow up with Marcus about website copy."
  ></textarea>

  <div class="button-row">
    <button id="generateButton" class="primary-button">Run AI</button>
    <button id="resetButton" class="secondary-button">Reset</button>
  </div>

  <p id="statusMessage" class="status-message"></p>

  <div id="outputCard" class="output-card hidden">
    <h4>AI Result</h4>
    <div class="result-block">
      <h5>Output</h5>
      <p id="mainOutput"></p>
    </div>
  </div>
</section>
```
#### **Step 2: Update `style.css`**

Add styling for the dropdown, secondary button, and button row:
```
select {
  width: 100%;
  padding: 12px;
  margin: 12px 0 16px;
  border: 1px solid #cbd5e1;
  border-radius: 10px;
  font-size: 1rem;
  background-color: white;
}

.button-row {
  display: flex;
  gap: 12px;
  flex-wrap: wrap;
}

.secondary-button {
  text-decoration: none;
  background-color: #e2e8f0;
  color: #1f2933;
  padding: 12px 20px;
  border-radius: 8px;
  display: inline-block;
  border: none;
  cursor: pointer;
}

.secondary-button:hover {
  background-color: #cbd5e1;
}
```
#### **Step 3: Update `server.js`**

Add multiple AI task types:
```
// server.js
// Applied AI Week 2 Day 5
// This server supports multiple AI actions for the product demo.

const express = require("express");
const cors = require("cors");
const dotenv = require("dotenv");
const OpenAI = require("openai");

dotenv.config();

const app = express();
const PORT = 3000;

app.use(cors());
app.use(express.json());
app.use(express.static("."));

const client = new OpenAI({
  apiKey: process.env.OPENAI_API_KEY,
});

app.post("/generate", async (req, res) => {
  const { userInput, taskType } = req.body;

  if (!userInput || userInput.trim() === "") {
    return res.status(400).json({
      error: "Please enter some notes or ideas first.",
    });
  }

  let prompt = "";

  if (taskType === "summarize") {
    prompt = `
You are a helpful AI assistant.
Summarize the following text clearly and briefly:

"${userInput}"

Return only the summary.
`;
  } else if (taskType === "nextsteps") {
    prompt = `
You are a helpful AI assistant.
Read the following text and generate clear next steps:

"${userInput}"

Return only practical next steps in a readable format.
`;
  } else {
    prompt = `
You are a helpful AI productivity assistant.
Organize the following notes into a clearer structure:

"${userInput}"

Return a clean, readable organized version.
`;
  }

  try {
    const response = await client.responses.create({
      model: "gpt-4.1-mini",
      input: prompt,
    });

    res.json({
      result: response.output_text,
    });
  } catch (error) {
    console.error("OpenAI API error:", error);
    res.status(500).json({
      error: "Something went wrong while generating the result.",
    });
  }
});

app.listen(PORT, () => {
  console.log(`Server is running on http://localhost:${PORT}`);
});
```
#### **Step 4: Update `script.js`**

Handle the dropdown and reset button:
```
// script.js
// Applied AI Week 2 Day 5
// This script supports multiple AI actions and a reset button.

const userInput = document.getElementById("userInput");
const taskType = document.getElementById("taskType");
const generateButton = document.getElementById("generateButton");
const resetButton = document.getElementById("resetButton");
const outputCard = document.getElementById("outputCard");
const statusMessage = document.getElementById("statusMessage");
const mainOutput = document.getElementById("mainOutput");

generateButton.addEventListener("click", async () => {
  const text = userInput.value.trim();
  const selectedTask = taskType.value;

  if (text === "") {
    statusMessage.textContent = "Please enter some text first.";
    outputCard.classList.add("hidden");
    return;
  }

  statusMessage.textContent = "Running AI...";
  outputCard.classList.add("hidden");

  try {
    const response = await fetch("/generate", {
      method: "POST",
      headers: {
        "Content-Type": "application/json",
      },
      body: JSON.stringify({
        userInput: text,
        taskType: selectedTask,
      }),
    });

    const data = await response.json();

    if (!response.ok || data.error) {
      statusMessage.textContent = data.error || "Something went wrong.";
      return;
    }

    mainOutput.textContent = data.result;
    statusMessage.textContent = "Done.";
    outputCard.classList.remove("hidden");
  } catch (error) {
    console.error(error);
    statusMessage.textContent = "There was a problem connecting to the server.";
  }
});

resetButton.addEventListener("click", () => {
  userInput.value = "";
  taskType.value = "organize";
  mainOutput.textContent = "";
  statusMessage.textContent = "";
  outputCard.classList.add("hidden");
});
```
#### **Guided Practice Teaching Points**

-   Why multiple AI actions make a product feel more capable
-   Why reset and control features improve usability
-   Why flexible UX can increase product value
-   Why backend logic should stay organized as the product grows
-   Why a polished demo should show choice, control, and clarity

#### **Guided Practice Discussion**

-   What made this version feel more advanced?
-   Why are multiple actions useful for a SaaS tool?
-   What other action types could fit this product?
-   How do these changes improve the user experience?

### 4\. **Independent Practice (Time: 65 minutes)**

-   **Objective:** Give Geniuses time to make meaningful improvements to their own AI SaaS product and prepare for a short showcase.
-   Geniuses continue and strengthen their Week 2 project.

#### **Mini-Project Title**

**AI SaaS Product Website --- Day 5 Flex Build and Showcase Prep**

#### **Independent Task**

Each Genius chooses **2--3 meaningful upgrades** to apply to their product.

#### **Improvement Menu**

Geniuses can choose from the following:

-   Add a second AI action or route
-   Add a dropdown or multiple buttons for task types
-   Add a reset button
-   Improve the backend prompt
-   Improve result formatting
-   Add better instructions for the user
-   Add loading and disabled button states
-   Add a pricing section to the landing page
-   Add testimonials or trust signals
-   Add a navbar with better links
-   Improve mobile responsiveness
-   Add a footer
-   Add stronger error handling
-   Add a product note explaining limitations
-   Refactor backend or frontend code to be cleaner

#### **Required Deliverables**

-   A working full-stack AI SaaS product
-   At least 2 meaningful improvements
-   A short product summary with:
    -   Product name
    -   Target user
    -   Problem solved
    -   Main user flow
    -   Main AI feature
    -   One trust or UX feature
    -   Two upgrades made today
-   A 1--2 minute showcase or demo plan

#### **Showcase Prep Prompt**

Ask Geniuses to prepare a short demo that answers:

-   What is your product called?
-   Who is it for?
-   What problem does it solve?
-   How does the user interact with it?
-   What role does AI play?
-   What did you improve today?
-   What makes your product useful or trustworthy?

#### **Facilitator Support Moves**

-   Help Geniuses choose upgrades that matter most
-   Push them to strengthen the main product experience before adding random extras
-   Ask:
    -   What still feels weakest?
    -   What would help the user most?
    -   What would make the product feel more complete?
    -   What will make your demo stronger?
-   Encourage repeated testing and debugging

### 5\. **Closure (Time: 20 minutes)**

-   **Objective:** Celebrate the week's work, reinforce growth, and help Geniuses practice showcasing an AI SaaS product clearly.
-   Bring the class together for a showcase.
-   Invite Geniuses to present individually or in small groups.
-   Each Genius should share:
    -   Their product name
    -   Their target user
    -   The problem solved
    -   The main user interaction
    -   The AI-powered result
    -   Two improvements they made today
-   After each share, invite quick audience feedback:
    -   What feels strongest?
    -   What feels most useful?
    -   What would be exciting to add next?
-   Lead a final reflection discussion:
    -   What did you learn this week about how businesses build AI products?
    -   What part of the full-stack process was hardest?
    -   What part felt most exciting?
    -   What makes an AI SaaS product feel real instead of just being a demo?

**Assessment:**
---------------

Student learning will be assessed through:

-   Participation in the icebreaker and discussion
-   Reflection responses during direct instruction
-   Completion of the guided AI SaaS upgrade build
-   Completion of at least 2 meaningful improvements to the independent project
-   Final product showcase and explanation
-   End-of-week reflection on business value, UX, and AI integration

### **Exit Ticket**

1.  What is one improvement that made your product stronger today?
2.  What makes your product feel more real now than it did on Day 1?
3.  What is one thing you would still improve next?

**Extra Activities:**
---------------------

-   Geniuses who finish early can:
    -   add a second page like `pricing.html` or `about.html`
    -   add tabbed result sections
    -   add copy-to-clipboard for output
    -   add a download or save feature
    -   add a theme toggle
    -   add more polished animations or transitions
-   Add input examples beneath the text area
-   Add output history on the page
-   Add a second backend route for a different product behavior
-   Split backend logic into reusable functions

**Reflection / Takeaways:**
---------------------------

This lesson works best when Geniuses see that real AI SaaS products are not built in one pass. They are shaped through iteration, product judgment, and constant improvement. Day 5 should feel like a builder studio and a showcase day. The goal is not perfect products, but stronger ones. By the end of the lesson, Geniuses should feel that they have built something that connects business thinking, web development, backend logic, and real AI functionality into one product experience.

**Facilitator Notes**
---------------------

-   Keep using **Geniuses** consistently in prompts, examples, and discussion.
-   Let the flex time feel open, but keep Geniuses focused on meaningful upgrades.
-   Encourage quality over quantity.
-   Help Geniuses prepare to explain both the technical side and the business side of their product.
-   Reinforce that product polish is a real part of professional software development.

**Week 2 Wrap-Up**
------------------

By the end of Week 2, each Genius should have:

-   An AI SaaS business idea
-   A landing page built with HTML and CSS
-   Front-end interactivity with JavaScript
-   A Node and Express backend
-   Real OpenAI-powered product functionality
-   A stronger prompt and cleaner UX
-   At least 2 meaningful flex day upgrades
-   A product demo and short showcase explanation
