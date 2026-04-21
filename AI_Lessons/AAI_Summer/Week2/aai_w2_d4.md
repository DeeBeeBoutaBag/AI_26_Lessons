<img src="https://github.com/Hgp-GeniusLabs/Curriculum/blob/10734f2c827128dde773ea4f266d154d46977866/Org-Wide/Assets/hgp_logo_original.png" width="150"/>

Lesson Plan: Applied AI Week 2, Day 4 --- Improving AI Product UX, Prompt Quality, and Product Behavior
=====================================================================================================

**Duration:**
-------------

3 hours

**Lesson Overview:**
--------------------

On Day 4, Geniuses improve the quality of the AI SaaS products they began building earlier in the week. By this point, Geniuses have created a landing page, added front-end interactivity, and connected their product to a real Node backend with OpenAI-powered functionality. Now the focus shifts to making the product feel smarter, cleaner, more trustworthy, and more useful.

This lesson helps Geniuses understand that a working AI feature is only the beginning. Strong AI products also need better prompting, clearer output formatting, stronger user experience, and better product behavior. During guided practice, the class upgrades their web app by improving the server-side prompt, adding loading and error states, and structuring the AI output more clearly on the page. During independent practice, each Genius improves their own AI SaaS product so it feels more polished and more aligned to a real business use case.

**Objectives:**
---------------

-   Explain how prompt quality affects AI output quality in a web product.
-   Identify ways user experience design improves trust, clarity, and usefulness in AI SaaS products.
-   Improve a Node and OpenAI-powered product by refining prompts and output structure.
-   Add loading states, error handling, and cleaner result formatting to a web app.
-   Strengthen product behavior so the AI feels more intentional and more aligned with the target user.
-   Improve an AI SaaS product so it feels more like a real business tool and less like a raw demo.

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
-   Existing Week 2 Day 1, Day 2, and Day 3 project files

**Standards:**
--------------

-   Computational Thinking: Refine system behavior by improving inputs, outputs, and user flow.
-   Computer Science Practices: Test, revise, and improve a full-stack AI application.
-   Web Development: Improve a full-stack web product using HTML, CSS, JavaScript, Node, and API integration.
-   Digital Literacy: Evaluate whether a digital product is clear, trustworthy, and user-centered.
-   Career Readiness: Practice iteration, debugging, usability thinking, and product refinement.
-   Entrepreneurship and Innovation: Improve a product based on user needs, trust, and business value.

**Lesson Activity:**
--------------------

### 1. **Introduction (Time: 25 minutes)**

-   **Objective:** Energize Geniuses and help them recognize the difference between a product that merely works and a product that feels strong, polished, and trustworthy.
-   Start with an icebreaker called **"Good Output or Great Product?"**
-   This should be the first and most energetic part of the lesson.

#### **Icebreaker Option A: Physical Movement**

-   Label one side of the room **"Works"** and the other side **"Feels Real."**
-   Read product situations aloud and have Geniuses move to the side that best matches.
-   Example prompts:
    -   A button returns text, but the user has no idea what is happening while it loads
    -   The AI gives a response, but it is one huge paragraph
    -   The product gives a loading message, clear sections, and a helpful warning
    -   The AI answers well sometimes, but there is no error handling
    -   The output matches the product goal and has a clear next step
    -   The product works, but the tone feels random and inconsistent
-   After each round, ask:
    -   Why does this only "work" instead of "feel real"?
    -   What would make it more trustworthy?
    -   What would make the output more useful?
    -   What would make the product feel more complete?

#### **Icebreaker Option B: Product Critique**

-   Show two output examples for the same product:
    -   one vague and messy
    -   one structured and user-friendly
-   Ask Geniuses to vote:
    -   Which one feels more professional?
    -   Which one feels more useful?
    -   Which one would make a user come back?

#### **Transition**

-   Say:
    -   "A real product is not just about getting a response. It is about how that response feels, how it is delivered, and whether the user knows what to do next."
-   Ask:
    -   What makes an AI product feel polished?
    -   What makes users trust the result?

### 2. **Direct Instruction (Time: 50 minutes)**

-   **Objective:** Help Geniuses understand how prompt quality, UX, and product behavior shape the real value of an AI SaaS product.
-   Use slides to guide instruction and stop often for discussion.

#### **Suggested Slide Flow**

-   **Slide 1: Day 4 Focus --- Make the Product Smarter and Cleaner**
    -   A working AI product is only the starting point
    -   Today is about making it feel usable and trustworthy
-   **Slide 2: Why Prompt Quality Matters**
    -   The backend prompt shapes the response
    -   Better prompts lead to more relevant, structured, and consistent output
-   **Slide 3: Signs of a Weak AI Product Experience**
    -   vague output
    -   random tone
    -   no structure
    -   confusing next steps
    -   no loading state
    -   weak or missing error messages
-   **Slide 4: Signs of a Strong AI Product Experience**
    -   clear task-specific response
    -   useful formatting
    -   consistent tone
    -   visible feedback during loading
    -   helpful error handling
    -   a clear next step for the user
-   **Slide 5: Product Behavior Is a Design Choice**
    -   Should the product be encouraging?
    -   concise?
    -   step-by-step?
    -   cautious?
    -   professional?
    -   conversational?
-   **Slide 6: UX Improvements That Matter**
    -   loading indicators
    -   better button labels
    -   cleaner sections
    -   clearer instructions
    -   output headings
    -   warnings or notes when needed
-   **Slide 7: Prompt Engineering in SaaS Products**
    -   define the role
    -   define the user
    -   define the task
    -   define the output format
    -   define the tone
    -   define any limitations or boundaries
-   **Slide 8: Better Output Supports Business Value**
    -   stronger output can improve user trust
    -   stronger output can improve retention
    -   stronger output can make the product feel premium
-   **Slide 9: Day 4 Build Goal**
    -   make your AI web app more useful, clearer, and more trustworthy
-   **Slide 10: Looking Ahead**
    -   Day 5 will be a flex day to polish, extend, and showcase the product

#### **Discussion Questions**

-   Why can two products using the same model feel very different?
-   What kind of tone fits your product best?
-   What should happen while the AI is working?
-   Why is structured output often better than one long paragraph?
-   What makes a user more likely to trust the result?

#### **Reflection Prompt**

-   Have Geniuses write for 4 minutes:
    -   "What part of your product still feels unfinished, confusing, or weak?"

### 3. **Guided Practice (Time: 60 minutes)**

-   **Objective:** Help Geniuses improve the quality of their AI SaaS product by upgrading the backend prompt, adding better frontend UX, and improving output formatting.
-   Explain that today's code-along is about refinement, not starting over.

#### **Guided Practice Build**

Use the existing project folder and improve:

-   `server.js`
-   `script.js`
-   `index.html`
-   `style.css`

#### **Project Goal**

Improve the product so that:

-   the backend prompt is more specific
-   the frontend shows a loading state
-   the product shows clearer output sections
-   the product handles errors more gracefully
-   the user experience feels more professional

#### **Step 1: Update `index.html`**

Add a clearer output layout:
```
<section class="demo-section" id="demo">
  <h3>Try the Product Demo</h3>
  <p class="demo-description">
    Paste messy notes below and see how the product helps organize them.
  </p>

  <textarea
    id="userInput"
    placeholder="Example: Team meeting on Friday. Finish logo update, send budget draft, and follow up with Marcus about website copy."
  ></textarea>

  <button id="generateButton" class="primary-button">Organize My Notes</button>

  <p id="statusMessage" class="status-message"></p>

  <div id="outputCard" class="output-card hidden">
    <h4>AI Result</h4>

    <div class="result-block">
      <h5>Summary</h5>
      <p id="summaryOutput"></p>
    </div>

    <div class="result-block">
      <h5>Action Items</h5>
      <p id="actionsOutput"></p>
    </div>

    <div class="result-block">
      <h5>Next Step</h5>
      <p id="nextStepOutput"></p>
    </div>
  </div>
</section>
```
#### **Step 2: Update `style.css`**

Add cleaner styles for status and output sections:
```
.status-message {
  margin: 14px 0;
  font-weight: bold;
  color: #2563eb;
}

.output-card {
  margin-top: 20px;
}

.result-block {
  margin-bottom: 20px;
  padding: 16px;
  background-color: #f8fafc;
  border-radius: 10px;
}

.result-block h5 {
  margin-bottom: 8px;
  font-size: 1rem;
  color: #1d4ed8;
}
```
#### **Step 3: Improve `server.js`**

Use a stronger prompt and request structured JSON output:
```
// server.js
// Applied AI Week 2 Day 4
// This server improves prompt quality and returns structured output.

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
  const { userInput } = req.body;

  if (!userInput || userInput.trim() === "") {
    return res.status(400).json({
      error: "Please enter some notes or ideas first.",
    });
  }

  try {
    const prompt = `
You are ClarityAI, a helpful AI productivity assistant for busy teams.

A user pasted the following notes:
"${userInput}"

Your job is to organize the notes into three parts:
1. summary
2. actionItems
3. nextStep

Rules:
- Keep the summary short and clear
- Make action items practical
- Make the next step specific
- Use language that feels professional and easy to understand
- Do not make up details that are not supported by the user's notes

Return your response as valid JSON in this exact shape:
{
 "summary": "string",
 "actionItems": "string",
 "nextStep": "string"
}
`;

    const response = await client.responses.create({
      model: "gpt-4.1-mini",
      input: prompt,
    });

    const rawText = response.output_text;
    const cleanedText = rawText.replace(/```json|```/g, "").trim();
    const parsedResult = JSON.parse(cleanedText);

    res.json(parsedResult);
  } catch (error) {
    console.error("OpenAI API error:", error);

    res.status(500).json({
      error: "Something went wrong while improving your notes. Please try again.",
    });
  }
});

app.listen(PORT, () => {
  console.log(`Server is running on http://localhost:${PORT}`);
});
```
#### **Step 4: Improve `script.js`**

Show loading state and display structured output:
```
// script.js
// Applied AI Week 2 Day 4
// This script shows loading feedback and displays structured AI output.

const userInput = document.getElementById("userInput");
const generateButton = document.getElementById("generateButton");
const outputCard = document.getElementById("outputCard");
const statusMessage = document.getElementById("statusMessage");

const summaryOutput = document.getElementById("summaryOutput");
const actionsOutput = document.getElementById("actionsOutput");
const nextStepOutput = document.getElementById("nextStepOutput");

generateButton.addEventListener("click", async () => {
  const text = userInput.value.trim();

  if (text === "") {
    statusMessage.textContent = "Please enter some notes or ideas first.";
    outputCard.classList.add("hidden");
    return;
  }

  statusMessage.textContent = "Generating AI response...";
  outputCard.classList.add("hidden");

  try {
    const response = await fetch("/generate", {
      method: "POST",
      headers: {
        "Content-Type": "application/json",
      },
      body: JSON.stringify({ userInput: text }),
    });

    const data = await response.json();

    if (!response.ok || data.error) {
      statusMessage.textContent = data.error || "Something went wrong.";
      outputCard.classList.add("hidden");
      return;
    }

    summaryOutput.textContent = data.summary;
    actionsOutput.textContent = data.actionItems;
    nextStepOutput.textContent = data.nextStep;

    statusMessage.textContent = "Done.";
    outputCard.classList.remove("hidden");
  } catch (error) {
    console.error(error);
    statusMessage.textContent = "There was a problem connecting to the server.";
    outputCard.classList.add("hidden");
  }
});
```
#### **Guided Practice Teaching Points**

-   Why stronger prompts produce better results
-   Why structured output is easier to display in a product
-   Why loading and error states matter
-   Why clearer UX improves trust
-   Why product refinement is part of real-world development

#### **Guided Practice Discussion**

-   What made this version feel stronger than yesterday's?
-   Why is structured JSON useful here?
-   What would a user appreciate most about these upgrades?
-   What other UX improvement would help even more?

### 4. **Independent Practice (Time: 30 minutes)**

-   **Objective:** Geniuses independently improve their own AI SaaS app by refining prompts, output structure, and UX.
-   This is the main Day 4 upgrade to the Week 2 mini-project.

#### **Mini-Project Title**

**AI SaaS Product Website --- Day 4 UX and Prompt Upgrade**

#### **Independent Task**

Each Genius improves their product by making at least **3 meaningful upgrades** in one or more of these categories:

-   **Prompt Quality**
    -   make the AI role clearer
    -   define output structure
    -   improve tone
    -   add helpful rules or boundaries
-   **Frontend UX**
    -   add loading text
    -   improve button labels
    -   add better instructions
    -   create clearer sections for the result
-   **Output Structure**
    -   split the result into sections
    -   label the response more clearly
    -   show next steps
    -   improve readability
-   **Error Handling**
    -   better empty input handling
    -   better server error messaging
    -   safer JSON parsing support

#### **Required Deliverables**

-   Updated `index.html`
-   Updated `style.css`
-   Updated `script.js`
-   Updated `server.js`
-   A product with:
    -   stronger prompt logic
    -   better frontend feedback
    -   clearer result display
    -   improved usability
-   A short written reflection:
    -   What 3 upgrades did you make?
    -   Which upgrade improved your product the most?
    -   What still needs improvement?

#### **Facilitator Support Moves**

-   Push Geniuses to improve what matters most for the user
-   Ask:
    -   Is your AI output clear?
    -   Does your product explain what it is doing?
    -   Does the result feel helpful and specific?
    -   What happens if the AI gives an unexpected response?
-   Encourage testing multiple inputs

### 5. **Closure (Time: 15 minutes)**

-   **Objective:** Reinforce that strong AI products are built through iteration and thoughtful refinement.
-   Bring the class together for a final share-out.
-   Ask 3--5 Geniuses to show:
    -   Their product name
    -   One prompt improvement
    -   One UX improvement
    -   One reason their app feels stronger now
-   Lead a closing discussion:
    -   What changed when you focused on polish instead of just functionality?
    -   Why does output structure matter?
    -   Why does UX matter even when the AI is strong?
    -   What should you focus on during the flex day tomorrow?

**Assessment:**
---------------

Student learning will be assessed through:

-   Participation in the icebreaker and discussion
-   Reflection responses during direct instruction
-   Completion of the guided product refinement build
-   Completion of at least 3 meaningful improvements to the independent product
-   Final share-out and explanation of why the product improved

### **Exit Ticket**

1.  What is one way prompt quality affects product quality?
2.  Why do loading and error states matter?
3.  What upgrade made your product stronger today?

**Extra Activities:**
---------------------

-   Geniuses who finish early can:
    -   add a reset button
    -   add multiple AI modes or output types
    -   improve JSON validation
    -   add a confidence or caution note
    -   improve styling for mobile screens
    -   create separate cards for each output section
-   Add a character counter
-   Disable the button while loading
-   Add helper text under the input box
-   Add a second AI route with a different product behavior

**Reflection / Takeaways:**
---------------------------

This lesson works best when Geniuses realize that quality is not just about having a response from the AI. It is about making that response understandable, useful, structured, and trustworthy. Day 4 teaches an important product lesson: users judge the full experience, not just the model behind it. By the end of the lesson, Geniuses should feel that their AI SaaS project is no longer just functioning, but improving into something more real, polished, and business-ready.

**Facilitator Notes**
---------------------

-   Keep using **Geniuses** consistently in all examples and discussion.
-   Reinforce that prompt design is product design.
-   Encourage clarity, structure, and user trust over unnecessary complexity.
-   Help Geniuses focus on improvements that matter most for the user experience.
-   Remind Geniuses that tomorrow is flex day for polish, feature additions, and showcase preparation.

**Week 2 Day 4 Mini-Project Connection**
----------------------------------------

By the end of Day 4, each Genius should have:

-   A landing page
-   Front-end interactivity
-   A Node and Express backend
-   Real OpenAI-powered output
-   A stronger backend prompt
-   Better frontend feedback
-   A more structured result display
-   At least 3 meaningful upgrades to UX or prompt quality
-   A more polished and trustworthy AI SaaS product
