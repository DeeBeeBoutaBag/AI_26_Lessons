<img src="https://github.com/Hgp-GeniusLabs/Curriculum/blob/10734f2c827128dde773ea4f266d154d46977866/Org-Wide/Assets/hgp_logo_original.png" width="150"/>

Lesson Plan: Applied AI Week 2, Day 3 --- Connecting the Frontend to Node and the OpenAI API
==========================================================================================

**Duration:**
-------------

3 hours

**Lesson Overview:**
--------------------

On Day 3, Geniuses move from a front-end product demo into a real AI-powered web application. The focus of the lesson is helping Geniuses understand how modern AI SaaS products connect a user-facing website to backend logic and an API. Geniuses learn that most real AI products are built as systems where the frontend collects user input, the backend processes the request securely, and the AI model returns a response that is shown back to the user.

During guided practice, the class sets up a simple Node and Express server, connects it to the OpenAI API, and links it to the website Geniuses started earlier in the week. By the end of guided practice, the class will have a functioning AI SaaS demo where the frontend sends a prompt to the backend and receives a real AI-generated response. During independent practice, each Genius adapts this architecture to fit their own AI SaaS concept and begins turning their website into a real working product.

**Objectives:**
---------------

-   Explain how frontend and backend systems work together in modern AI SaaS products.
-   Describe why API keys should stay on the server and not in frontend code.
-   Use Node, NPM, and Express to create a basic backend server.
-   Connect a frontend website to a backend API endpoint using JavaScript `fetch`.
-   Use the OpenAI API in a Node server to generate real AI-powered output.
-   Upgrade an AI SaaS website into a working web app with real AI functionality.

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
-   Existing Week 2 Day 1 and Day 2 project files

**Standards:**
--------------

-   Computational Thinking: Model how information flows between user input, backend processing, and AI output.
-   Computer Science Practices: Build and test a full-stack web application with external API integration.
-   Web Development: Use HTML, CSS, JavaScript, and Node together in one project.
-   Digital Literacy: Evaluate secure and responsible ways to use AI services in web products.
-   Career Readiness: Practice systems thinking, debugging, and real-world product development.
-   Entrepreneurship and Innovation: Build an AI-powered web product that creates real value for users.

**Lesson Activity:**
--------------------

### 1. **Introduction (Time: 25 minutes)**

-   **Objective:** Energize Geniuses and help them understand that real AI products require more than frontend design.
-   Start with an icebreaker called **"Frontend or Backend?"**
-   This should be the first and most energetic part of the lesson.

#### **Icebreaker Option A: Physical Movement**

-   Label one side of the room **"Frontend"** and the other side **"Backend."**
-   Read different product actions aloud and have Geniuses move to the side they think matches best.
-   Example prompts:
    -   A user types into a text box
    -   A button sends data to a server
    -   A website displays the AI response
    -   A server stores the API key
    -   A page changes content after a user clicks
    -   The server sends a request to OpenAI
    -   The browser shows an error message
-   After each round, ask:
    -   Why is that frontend or backend?
    -   What would happen if that part were missing?
    -   Which side handles the user experience?
    -   Which side handles the secure logic?

#### **Icebreaker Option B: Matching Activity**

-   Put different system roles on the board:
    -   User
    -   Browser
    -   JavaScript
    -   Server
    -   API key
    -   OpenAI API
    -   Output
-   Have Geniuses match the order of how a request moves through the system.

#### **Transition**

-   Say:
    -   "Yesterday, the product looked interactive. Today, it becomes real."
-   Ask:
    -   Why can we not safely put API keys in frontend code?
    -   What needs to happen between the button click and the AI response?

### 2. **Direct Instruction (Time: 50 minutes)**

-   **Objective:** Help Geniuses understand the role of backend systems in AI SaaS products and how secure AI integrations work.
-   Use slides to guide instruction and stop often for questions.

#### **Suggested Slide Flow**

-   **Slide 1: Day 3 Focus --- Real AI-Powered Products**
    -   Websites become real AI products when they connect to secure backend logic.
-   **Slide 2: Frontend vs Backend**
    -   Frontend:
        -   user interface
        -   forms
        -   buttons
        -   visible output
    -   Backend:
        -   secure logic
        -   API calls
        -   key protection
        -   processing data
-   **Slide 3: Why API Keys Must Be Protected**
    -   API keys should not be placed in browser JavaScript
    -   Anyone can inspect frontend code
    -   Backend protects sensitive information
-   **Slide 4: What Is Node.js?**
    -   Node lets JavaScript run on the server
    -   It is commonly used to build web backends
-   **Slide 5: What Is Express?**
    -   Express is a Node framework for building routes and APIs quickly
-   **Slide 6: AI SaaS Request Flow**
    -   User enters text
    -   Frontend sends data to backend
    -   Backend calls OpenAI
    -   Backend returns response
    -   Frontend displays result
-   **Slide 7: Why This Matters in Real Business**
    -   This is how many modern AI tools work
    -   The interface and AI are connected through product architecture
-   **Slide 8: Good Product Architecture Builds Trust**
    -   security
    -   clearer logic
    -   easier debugging
    -   easier scaling later
-   **Slide 9: Today's Build Goal**
    -   Connect the website to a Node backend and real OpenAI output
-   **Slide 10: Looking Ahead**
    -   Tomorrow Geniuses will improve prompting, UX, and product behavior even more

#### **Discussion Questions**

-   Why should API keys stay on the server?
-   What role does the backend play in user experience, even if the user does not see it?
-   What could go wrong if an AI product has weak architecture?
-   Why does secure backend logic matter for business trust?
-   How does full-stack thinking change the way you design products?

#### **Reflection Prompt**

-   Have Geniuses write for 4 minutes:
    -   "Why is it important for an AI product to be both useful and secure?"

### 3. **Guided Practice (Time: 60 minutes)**

-   **Objective:** Help Geniuses build a working Node and Express backend that connects their website to the OpenAI API.
-   Explain that today's code-along turns the website into a real AI app.

#### **Guided Practice Build**

Use the existing `ai-saas-starter` folder and add:

-   `package.json`
-   `server.js`
-   `.env`

#### **Project Goal**

Build a web app where:

-   the frontend collects text input
-   JavaScript sends the input to a Node backend
-   the backend calls OpenAI
-   the frontend displays the AI-generated result

#### **Setup Steps**

1.  Open the existing project folder in VS Code.
2.  Open the terminal.
3.  Run:
```
npm init -y
npm install express openai dotenv cors
```
1.  Create a `.env` file:
```
OPENAI_API_KEY=your_key_here
```
1.  Create `server.js`
2.  Update `script.js`
3.  Run the server with:
`
node server.js
`
#### **Sample `server.js`**
```
// server.js
// Applied AI Week 2 Day 3
// This file creates a backend server that receives user input,
// sends it to the OpenAI API, and returns the response.

const express = require("express");
const cors = require("cors");
const dotenv = require("dotenv");
const OpenAI = require("openai");

dotenv.config();

const app = express();
const PORT = 3000;

// Middleware
app.use(cors());
app.use(express.json());
app.use(express.static("."));

// Create the OpenAI client
const client = new OpenAI({
  apiKey: process.env.OPENAI_API_KEY,
});

// Basic test route
app.get("/", (req, res) => {
  res.sendFile(__dirname + "/index.html");
});

// AI route
app.post("/generate", async (req, res) => {
  const { userInput } = req.body;

  if (!userInput || userInput.trim() === "") {
    return res.status(400).json({\
      error: "User input is required.",\
    });
  }

  try {
    const prompt = `
You are a helpful AI SaaS assistant.

The user entered the following text:
"${userInput}"

Please organize the content into:
1. A short summary
2. Key action items
3. A helpful next step

Keep the response clear, practical, and easy to understand.
`;

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
      error: "Something went wrong while generating the AI response.",
    });
  }
});

// Start the server
app.listen(PORT, () => {\
  console.log(`Server is running on http://localhost:${PORT}`);
});
```
#### **Updated `script.js`**
```
// script.js
// Applied AI Week 2 Day 3
// This script sends user input to the backend and displays the AI response.

const userInput = document.getElementById("userInput");
const generateButton = document.getElementById("generateButton");
const outputCard = document.getElementById("outputCard");
const outputText = document.getElementById("outputText");

generateButton.addEventListener("click", async () => {
  const text = userInput.value.trim();

  if (text === "") {
    outputText.textContent = "Please enter some notes or ideas first.";
    outputCard.classList.remove("hidden");
    return;
  }

  outputText.textContent = "Generating AI response...";
  outputCard.classList.remove("hidden");

  try {
    const response = await fetch("/generate", {
      method: "POST",
      headers: {
        "Content-Type": "application/json",
      },
      body: JSON.stringify({ userInput: text }),
    });

    const data = await response.json();

    if (data.error) {
      outputText.textContent = data.error;
      return;
    }

    outputText.textContent = data.result;
  } catch (error) {
    outputText.textContent = "There was a problem connecting to the server.";
    console.error(error);
  }
});
```
#### **Optional HTML Reminder**

Make sure `index.html` still includes:

-   a text area with `id="userInput"`
-   a button with `id="generateButton"`
-   an output card with `id="outputCard"`
-   a paragraph or element with `id="outputText"`

#### **Guided Practice Teaching Points**

-   How frontend and backend communicate
-   Why `fetch` is useful
-   Why Express routes matter
-   Why environment variables protect secrets
-   Why AI product architecture is part of product quality

#### **Guided Practice Discussion**

-   What part of this system felt most different from the frontend-only version?
-   Why is the backend necessary here?
-   What would need to change if the product had multiple AI features?
-   What makes this feel more like a real SaaS product?

### 4. **Independent Practice (Time: 30 minutes)**

-   **Objective:** Geniuses independently connect their own AI SaaS concept to a backend route and real OpenAI-powered output.
-   This is the main Day 3 upgrade to the Week 2 mini-project.

#### **Mini-Project Title**

**AI SaaS Product Website --- Day 3 Real AI Integration**

#### **Independent Task**

Each Genius updates their own project so that:

-   the frontend sends input to a backend route
-   the backend uses the OpenAI API
-   the result is shown on the page

Their AI behavior should match their product idea.

Examples:

-   Study tool: user enters assignments and gets an organized plan
-   Career tool: user enters interests and gets suggested careers
-   Productivity tool: user enters notes and gets a summary plus tasks
-   Wellness tool: user enters a goal and gets a simple action plan

#### **Required Deliverables**

-   A working `index.html`
-   A working `style.css`
-   A working `script.js`
-   A working `server.js`
-   A `.env` file configured locally
-   A product with:
    -   user input
    -   a frontend request
    -   a backend AI route
    -   real OpenAI output on the page
-   A short written reflection:
    -   What does the frontend do?
    -   What does the backend do?
    -   Why is the backend important for security?

#### **Facilitator Support Moves**

-   Help Geniuses keep the first backend route simple
-   Ask:
    -   What exact input is the user sending?
    -   What exact output should the AI return?
    -   Does the prompt match the product goal?
    -   What happens if the request fails?
-   Encourage testing with multiple user inputs

### 5. **Closure (Time: 15 minutes)**

-   **Objective:** Reinforce that full-stack architecture is what turns a product demo into a real AI application.
-   Bring the class together for a final share-out.
-   Ask 3--5 Geniuses to show:
    -   Their product name
    -   The user input they collect
    -   The AI output their backend returns
    -   One reason the backend matters
-   Lead a closing discussion:
    -   What changed when the AI became real?
    -   Why does security matter in AI products?
    -   What part of full-stack building felt most exciting?
    -   What would make your product even stronger tomorrow?
-   Preview the next lesson:
    -   Geniuses will improve prompt design, product UX, and the quality of the AI experience.

**Assessment:**
---------------

Student learning will be assessed through:

-   Participation in the icebreaker and discussion
-   Reflection responses during direct instruction
-   Completion of the guided backend and OpenAI integration build
-   Completion of an independent AI-powered web product route
-   Final share-out and explanation of system architecture

### **Exit Ticket**

1.  What does the frontend do in an AI SaaS product?
2.  What does the backend do?
3.  Why should API keys stay on the server?

**Extra Activities:**
---------------------

-   Geniuses who finish early can:
    -   add a loading state
    -   add better error handling
    -   add a second AI route
    -   add multiple buttons for different output types
    -   split the output into sections on the page
    -   improve the prompt inside `server.js`
-   Add a reset button
-   Add input validation on both frontend and backend
-   Add a simple route like `/health` to check whether the server is running

**Reflection / Takeaways:**
---------------------------

This lesson works best when Geniuses realize that real AI products are built through systems, not just screens. Day 3 is a major shift because it shows how the frontend, backend, and AI model work together as one product experience. It also introduces an important professional habit: secure architecture. By the end of the lesson, Geniuses should feel that they have crossed from a demo into a real application and that their AI SaaS idea now has a working technical foundation.

**Facilitator Notes**
---------------------

-   Keep using **Geniuses** consistently in all examples and discussion.
-   Reinforce that backend logic is part of product quality and user trust.
-   Encourage Geniuses to test often and debug patiently.
-   Keep the first AI route focused on one clear use case.
-   Remind Geniuses that tomorrow they can make the product smarter, cleaner, and more useful through better prompting and UX.

**Week 2 Day 3 Mini-Project Connection**
----------------------------------------

By the end of Day 3, each Genius should have:

-   A product landing page
-   A user input flow
-   A JavaScript-powered frontend interaction
-   A Node and Express backend
-   A secure `.env` setup for API keys
-   A working OpenAI-powered route
-   Real AI output displayed on the website
-   A stronger full-stack foundation for improving product quality next
