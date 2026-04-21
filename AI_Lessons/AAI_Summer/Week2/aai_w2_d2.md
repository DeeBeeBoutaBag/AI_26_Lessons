<img src="https://github.com/Hgp-GeniusLabs/Curriculum/blob/10734f2c827128dde773ea4f266d154d46977866/Org-Wide/Assets/hgp_logo_original.png" width="150"/>

Lesson Plan: Applied AI Week 2, Day 2 --- From Landing Page to Interactive Product with JavaScript
================================================================================================

**Duration:**
-------------

3 hours

**Lesson Overview:**
--------------------

On Day 2, Geniuses move from a static AI SaaS landing page into a more interactive product experience. The focus of the lesson is understanding how modern AI businesses create user flow, collect input, and turn a website into something a user can actually engage with. Geniuses learn that a real SaaS product is not just a homepage. It has interaction, logic, and an experience that helps users move from curiosity into action.

During guided practice, the class uses HTML, CSS, and JavaScript to upgrade yesterday's landing page into a product page with a working form and dynamic output area. Geniuses build a simple front-end experience where a user can type information, click a button, and see a generated response on the page. This will act as the bridge to later connecting the project to Node and the OpenAI API. During independent practice, each Genius adds interactivity to their own AI SaaS website and strengthens the product flow for their specific business idea.

**Objectives:**
---------------

-   Explain how interactive user experiences make SaaS products more useful and believable.
-   Identify how modern AI businesses use forms, inputs, and product flow to guide users.
-   Use JavaScript to capture user input and update the page dynamically.
-   Build an interactive front-end product demo using HTML, CSS, and JavaScript.
-   Improve an AI SaaS website by adding a user-facing feature flow.
-   Prepare a web product for future backend and OpenAI API integration.

**Materials:**
--------------

-   Laptops for all Geniuses
-   VS Code installed
-   Internet access
-   Projector or display
-   Whiteboard and markers
-   Slide deck for lecture and discussion
-   Reflection journal or digital notes
-   Browser for viewing local HTML files
-   Live Server extension or another local preview method
-   Existing Week 2 Day 1 project files

**Standards:**
--------------

-   Computational Thinking: Model how user input moves through a digital system to produce output.
-   Computer Science Practices: Build and test interactive website features using JavaScript.
-   Web Development: Use HTML, CSS, and JavaScript together to create product experiences.
-   Digital Literacy: Evaluate how user experience influences trust and product value.
-   Career Readiness: Practice product thinking, iteration, and clear communication through digital tools.
-   Entrepreneurship and Innovation: Design interactive experiences that better communicate product value.

**Lesson Activity:**
--------------------

### 1. **Introduction (Time: 25 minutes)**

-   **Objective:** Energize Geniuses and help them understand that a real SaaS product needs interaction, not just good design.
-   Start with an icebreaker called **"Static or Interactive?"**
-   This should be the first and most energetic part of the lesson.

#### **Icebreaker Option A: Physical Movement**

-   Label one side of the room **"Static"** and the other side **"Interactive."**
-   Read product examples aloud and have Geniuses move to the side that best matches.
-   Example prompts:
    -   A homepage with only text and a button
    -   A study tool where you enter assignments and get a schedule
    -   A website with a pricing table and no other actions
    -   A career tool where users answer questions and get recommendations
    -   A productivity website with testimonials only
    -   A note summarizer where users paste text and see a result
-   After each round, ask:
    -   What makes this static?
    -   What makes this interactive?
    -   Which one feels more like a real product?
    -   What would a user expect to do on this page?

#### **Icebreaker Option B: Website Comparison**

-   Show two websites or two mockups:
    -   one that is just informational
    -   one that includes a form, buttons, and output
-   Ask Geniuses to vote:
    -   Which one feels more like a product?
    -   Which one would keep a user engaged longer?
    -   Which one would be easier to imagine paying for?

#### **Transition**

-   Say:
    -   "Yesterday, Geniuses built the front door. Today, we start building what happens when the user walks in."
-   Ask:
    -   What should a user be able to do on your product?
    -   What is the first useful action your product should support?

### 2. **Direct Instruction (Time: 50 minutes)**

-   **Objective:** Help Geniuses understand how JavaScript creates interactivity and why front-end logic matters in modern AI SaaS products.
-   Use slides to guide instruction and pause for discussion.

#### **Suggested Slide Flow**

-   **Slide 1: Day 2 Focus --- From Website to Product Experience**
    -   A landing page explains the product
    -   An interactive page lets the user try the product
-   **Slide 2: What Makes a SaaS Product Feel Real?**
    -   Input
    -   Action
    -   Output
    -   Feedback
    -   Clear user flow
-   **Slide 3: The Front-End Role in AI Products**
    -   Collect user input
    -   Show buttons and controls
    -   Display responses
    -   Guide the experience
-   **Slide 4: JavaScript in the Browser**
    -   JavaScript helps pages respond to user actions
    -   It can:
        -   read user input
        -   listen for button clicks
        -   update content on the page
        -   show and hide sections
-   **Slide 5: User Flow in SaaS Products**
    -   User arrives
    -   User understands the value
    -   User tries a feature
    -   User gets a result
    -   User decides whether to continue
-   **Slide 6: AI Product Flow Without Real AI Yet**
    -   Even before connecting an API, we can build:
        -   form inputs
        -   action buttons
        -   placeholder output
        -   feedback messages
    -   This helps us design the product experience first
-   **Slide 7: Why Product Flow Matters**
    -   Better flow improves usability
    -   Better flow makes the product easier to trust
    -   Better flow helps the business communicate value quickly
-   **Slide 8: Common Front-End Product Elements**
    -   Text areas
    -   Input fields
    -   Buttons
    -   Output cards
    -   Status messages
    -   Error messages
-   **Slide 9: Today's Build Goal**
    -   Upgrade the Week 2 Day 1 landing page with a working product demo section
-   **Slide 10: Looking Ahead**
    -   Today: front-end interaction
    -   Next: backend connection and real OpenAI-powered output

#### **Discussion Questions**

-   Why does interactivity make a product feel more real?
-   What should happen after a user clicks a button?
-   Why should a product give clear feedback to the user?
-   What kind of user input would make sense for your product?
-   How does a better user flow improve business value?

#### **Reflection Prompt**

-   Have Geniuses write for 4 minutes:
    -   "What is the first action a user should take on your product, and what should happen next?"

### 3. **Guided Practice (Time: 55 minutes)**

-   **Objective:** Help Geniuses build an interactive product section using HTML, CSS, and JavaScript.
-   Explain that the class will keep yesterday's site and add a simple front-end product demo.

#### **Guided Practice Build**

Use the existing `ai-saas-starter` folder and add:

-   `script.js`

#### **Project Goal**

Upgrade the landing page so a user can:

-   type into a text area
-   click a button
-   see a dynamic response appear on the page

#### **Setup Steps**

1.  Open the existing project in VS Code.
2.  Confirm these files exist:
    -   `index.html`
    -   `style.css`
3.  Create:
    -   `script.js`
4.  Link `script.js` at the bottom of `index.html`

#### **Updated `index.html`**
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>ClarityAI</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>
  <div class="page">
    <header class="hero">
      <nav class="navbar">
        <h1 class="logo">ClarityAI</h1>
        <a href="#demo" class="nav-button">Try Demo</a>
      </nav>

      <div class="hero-content">
        <div class="hero-text">
          <p class="tag">AI SaaS for smarter work</p>
          <h2>Turn messy information into clear next steps.</h2>
          <p class="subtitle">
            ClarityAI helps teams summarize notes, organize action items, and move faster with confidence.
          </p>
          <a href="#demo" class="primary-button">Try the Demo</a>
        </div>
      </div>
    </header>

    <section class="features">
      <h3>Why teams use ClarityAI</h3>
      <div class="feature-grid">
        <div class="feature-card">
          <h4>Summarize Fast</h4>
          <p>Turn long notes, meetings, and documents into quick, useful summaries.</p>
        </div>
        <div class="feature-card">
          <h4>Organize Work</h4>
          <p>Extract action items and structure messy ideas into clear next steps.</p>
        </div>
        <div class="feature-card">
          <h4>Save Time</h4>
          <p>Reduce repetitive work so teams can focus on higher-value tasks.</p>
        </div>
      </div>
    </section>

    <section class="demo-section" id="demo">
      <h3>Try the Product Demo</h3>
      <p class="demo-description">
        Paste messy notes below and see how the product could help organize them.
      </p>

      <textarea
        id="userInput"
        placeholder="Example: Team meeting on Friday. Finish logo update, send budget draft, and follow up with Marcus about website copy."\
      ></textarea>

      <button id="generateButton" class="primary-button">Generate Demo Output</button>

      <div id="outputCard" class="output-card hidden">
        <h4>Organized Output</h4>
        <p id="outputText"></p>
      </div>
    </section>

    <section class="cta" id="cta">
      <h3>Build clarity into your workflow</h3>
      <p>Start using AI to simplify your team's day-to-day work.</p>
      <a href="#" class="primary-button">Start Free Trial</a>
    </section>
  </div>

  <script src="script.js"></script>
</body>
</html>
```
#### **Updated `style.css`**
```
/* Reset browser defaults */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

/* Base page styles */
body {
  font-family: Arial, sans-serif;
  background-color: #f4f7fb;
  color: #1f2933;
  line-height: 1.6;
}

.page {
  width: 100%;
}

.hero {
  background: linear-gradient(135deg, #dbeafe, #eff6ff);
  padding: 32px 24px 80px;
}

.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 60px;
}

.logo {
  font-size: 1.8rem;
  font-weight: bold;
}

.nav-button,
.primary-button {
  text-decoration: none;
  background-color: #2563eb;
  color: white;
  padding: 12px 20px;
  border-radius: 8px;
  display: inline-block;
  border: none;
  cursor: pointer;
}

.primary-button:hover,
.nav-button:hover {
  background-color: #1d4ed8;
}

.hero-content,
.features,
.demo-section,
.cta {
  max-width: 1100px;
  margin: 0 auto;
}

.hero-text {
  max-width: 620px;
}

.tag {
  color: #2563eb;
  font-weight: bold;
  margin-bottom: 12px;
}

.hero-text h2 {
  font-size: 2.8rem;
  margin-bottom: 16px;
}

.subtitle {
  font-size: 1.1rem;
  margin-bottom: 24px;
  color: #52606d;
}

.features,
.demo-section,
.cta {
  padding: 70px 24px;
}

.features h3,
.demo-section h3,
.cta h3 {
  font-size: 2rem;
  margin-bottom: 24px;
}

.feature-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 20px;
}

.feature-card,
.output-card {
  background-color: white;
  padding: 24px;
  border-radius: 12px;
  box-shadow: 0 6px 16px rgba(0, 0, 0, 0.08);
}

.demo-description {
  margin-bottom: 16px;
  color: #52606d;
}

textarea {
  width: 100%;
  min-height: 140px;
  padding: 16px;
  border: 1px solid #cbd5e1;
  border-radius: 12px;
  font-size: 1rem;
  margin-bottom: 16px;
  resize: vertical;
}

.output-card {
  margin-top: 20px;
}

.hidden {
  display: none;
}

.cta {
  text-align: center;
}

@media (max-width: 768px) {
  .feature-grid {
    grid-template-columns: 1fr;
  }

  .hero-text h2 {
    font-size: 2rem;
  }

  .navbar {
    flex-direction: column;
    gap: 16px;
  }
}
```
#### **New `script.js`**
```
// script.js
// Applied AI Week 2 Day 2
// This script adds interactivity to the AI SaaS demo section.

// Select the elements we need from the page
const userInput = document.getElementById("userInput");
const generateButton = document.getElementById("generateButton");
const outputCard = document.getElementById("outputCard");
const outputText = document.getElementById("outputText");

// Add a click event listener to the button
generateButton.addEventListener("click", () => {
  // Get the text the user typed into the text area
  const text = userInput.value.trim();

  // Check whether the user entered anything
  if (text === "") {
    outputText.textContent = "Please enter some notes or ideas first.";
    outputCard.classList.remove("hidden");
    return;
  }

  // Create a simple front-end demo response
  // This is a placeholder experience before connecting real AI
  const demoResponse = `Here is a more organized version of your notes: ${text}

Suggested next step: Review the notes, identify the most urgent task, and assign ownership.`;

  // Put the generated response into the page
  outputText.textContent = demoResponse;

  // Show the output card
  outputCard.classList.remove("hidden");
});
```
#### **Guided Practice Teaching Points**

-   How JavaScript listens for user actions
-   How to grab values from input fields
-   How to update content on the page
-   Why even placeholder interactions help shape product design
-   Why clear feedback matters for users

#### **Guided Practice Discussion**

-   What makes this feel more like a real product?
-   What still feels fake or incomplete?
-   What would real AI improve here?
-   What should happen if the user enters poor input or no input?

### 4\. **Independent Practice (Time: 30 minutes)**

-   **Objective:** Geniuses independently add interactivity to their own AI SaaS website.
-   This builds the second layer of the Week 2 mini-project.

#### **Mini-Project Title**

**AI SaaS Product Website --- Day 2 Interactivity**

#### **Independent Task**

Each Genius updates their project to include:

-   at least one input field or text area
-   at least one button
-   a dynamic output area
-   JavaScript that responds to the user and updates the page

Their product interaction should match their business idea.

Examples:

-   Study tool: user enters assignments and gets an organized plan
-   Career tool: user enters interests and gets possible career suggestions
-   Productivity tool: user enters messy notes and gets a cleaner structure
-   Wellness tool: user enters a goal and gets a motivational plan

#### **Required Deliverables**

-   A working `index.html`
-   A working `style.css`
-   A working `script.js`
-   A site with:
    -   a clear product identity
    -   a user input area
    -   a button
    -   an output section
    -   a basic interactive flow
-   A short written reflection:
    -   What does the user type in?
    -   What should the product give back?
    -   What will real AI improve later?

#### **Facilitator Support Moves**

-   Help Geniuses keep the interaction simple and focused
-   Ask:
    -   What is the main action the user takes?
    -   What is the result they expect?
    -   Does the output feel useful?
    -   What would make this more believable?
-   Encourage good naming for ids, buttons, and sections

### 5. **Closure (Time: 20 minutes)**

-   **Objective:** Reinforce the idea that interactivity is what starts turning a website into a real product.
-   Bring the class together for a final share-out.
-   Ask 3--5 Geniuses to show:
    -   Their product name
    -   Their input area
    -   Their output area
    -   What the interaction is supposed to do
-   Lead a closing discussion:
    -   What changed when the page became interactive?
    -   What part of JavaScript felt most useful today?
    -   Why does user flow matter in SaaS products?
    -   What will real AI help improve next?

**Assessment:**
---------------

Student learning will be assessed through:

-   Participation in the icebreaker and discussion
-   Reflection responses during direct instruction
-   Completion of the guided interactive product demo
-   Completion of an independent JavaScript-powered product interaction
-   Final share-out and explanation of product flow

### **Exit Ticket**

1.  What makes a product interactive?
2.  What does JavaScript help websites do?
3.  What part of your product should be powered by real AI later?

**Extra Activities:**
---------------------

-   Geniuses who finish early can:
    -   add multiple buttons
    -   clear the form after submission
    -   add a character counter
    -   add multiple output sections
    -   show and hide loading text
    -   style the output card more clearly
-   Add a reset button
-   Add validation for very short input
-   Add multiple demo response types based on user input

**Reflection / Takeaways:**
---------------------------

This lesson works best when Geniuses realize that real digital products are more than visually appealing pages. They guide users through actions and responses. Day 2 helps Geniuses move from presenting an idea to simulating product behavior. Even before connecting a real AI model, this kind of interactivity helps clarify what the product should do, how the user experiences it, and what value it delivers. By the end of the lesson, Geniuses should feel that their AI SaaS idea is starting to become a usable product experience.

**Facilitator Notes**
---------------------

-   Keep using **Geniuses** consistently in all examples and discussion.
-   Reinforce that placeholder logic is still valuable because it helps design the user experience.
-   Encourage clarity and usability over complexity.
-   Help Geniuses keep their interaction focused on one strong use case.
-   Remind Geniuses that tomorrow they can begin connecting this flow to real backend and AI functionality.

**Week 2 Day 2 Mini-Project Connection**
----------------------------------------

By the end of Day 2, each Genius should have:

-   A product landing page
-   A clearer product flow
-   At least one user input area
-   At least one button
-   A dynamic output section
-   JavaScript that updates the page based on user action
-   A stronger foundation for connecting Node and the OpenAI API next
