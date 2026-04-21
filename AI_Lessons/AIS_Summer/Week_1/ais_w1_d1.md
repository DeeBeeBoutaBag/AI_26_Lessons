<img src="https://github.com/Hgp-GeniusLabs/Curriculum/blob/10734f2c827128dde773ea4f266d154d46977866/Org-Wide/Assets/hgp_logo_original.png" width="150"/>

Lesson Plan: AI Systems Week 1, Day 1 --- What Is an AI System? Ethics, Responsibility, and Real-World Impact
===========================================================================================================

**Duration:**
-------------

3 hours

**Lesson Overview:**
--------------------

This first AI Systems lesson introduces Geniuses to the technical and ethical foundations of modern AI systems. Geniuses begin by exploring what makes something an AI system instead of just a piece of software. They examine how AI systems take in data, process inputs, make predictions or generate outputs, and affect real people in the real world. The lesson also introduces key responsible AI concepts such as fairness, bias, privacy, safety, transparency, and accountability. Throughout the lesson, Geniuses begin thinking like technical builders who are not only interested in what AI can do, but also in how it works, what data it depends on, and what responsibilities come with building it.

During guided practice, the class builds a simple Python-based AI system analyzer in VS Code that takes an AI product idea and breaks it into technical parts such as input, model behavior, output, and possible risks. During independent practice, each Genius creates the first version of an AI system concept that they will continue refining across the week. By the end of the lesson, Geniuses should understand that AI systems are more than cool tools. They are technical systems with data, logic, tradeoffs, and consequences.

**Objectives:**
---------------

-   Define what an AI system is and explain how it differs from traditional software.
-   Identify the basic parts of an AI system, including input, processing, model behavior, and output.
-   Explain key responsible AI ideas including bias, fairness, privacy, transparency, safety, and accountability.
-   Analyze a real or imagined AI product as a technical system with ethical implications.
-   Build a simple Python program in VS Code that organizes the parts of an AI system.
-   Begin a mini-project by designing and documenting an AI system idea with technical and ethical awareness.

**Materials:**
--------------

-   Laptops for all Geniuses
-   VS Code installed
-   Python installed and working
-   Internet access
-   Projector or display
-   Whiteboard and markers
-   Slide deck for lecture and discussion
-   Reflection journal or digital notes
-   Terminal access in VS Code
-   Starter folder for Python files
-   Optional examples of modern AI products or systems

**Standards:**
--------------

-   Computational Thinking: Analyze systems through inputs, processes, outputs, and consequences.
-   Computer Science Practices: Explain how computing systems use data and models to produce results.
-   Digital Literacy: Evaluate ethical, responsible, and trustworthy uses of AI.
-   Career Readiness: Practice systems thinking, critical thinking, and technical communication.
-   Responsible Innovation: Identify risks, limitations, and social impacts of intelligent systems.
-   Technical Foundations: Distinguish between software logic and AI system behavior.

**Lesson Activity:**
--------------------

### 1. **Introduction (Time: 25 minutes)**

-   **Objective:** Energize Geniuses and introduce the idea that AI systems are all around them, but not every piece of software is actually an AI system.
-   Start with a fun icebreaker called **"AI System or Just Software?"**
-   This should be the first thing and the most fun thing to wake Geniuses up and get them ready for what they will learn today.

#### **Icebreaker Option A: Physical Movement**

-   Label one side of the room **"AI System"** and the other side **"Just Software."**
-   Read examples aloud and have Geniuses move to the side they think fits best.
-   Example prompts:
    -   A calculator
    -   A spam filter
    -   A playlist recommendation engine
    -   A stopwatch app
    -   A face unlock tool
    -   A simple website contact form
    -   A chatbot that answers questions
    -   A weather forecast app
    -   An object detection camera system
-   After each round, ask:
    -   Why does this count as an AI system or not?
    -   What data might it use?
    -   Is it making predictions, recognizing patterns, or generating something?
    -   What could go wrong if it makes mistakes?

#### **Icebreaker Option B: Live Poll**

-   Use Mentimeter, Slido, or another quick polling tool.
-   Show a list of digital tools and ask Geniuses to vote:
    -   AI system
    -   not an AI system
    -   not sure
-   Discuss surprising answers and introduce the idea that AI systems often involve data, pattern recognition, prediction, or generation.

#### **Transition**

-   Say:
    -   "This course is about understanding the systems underneath modern AI. Not just what they do, but how they work and why responsibility matters."
-   Ask:
    -   What makes something intelligent in a technical sense?
    -   What responsibilities come with building systems that influence people's decisions or experiences?

### 2. **Direct Instruction (Time: 55 minutes)**

-   **Objective:** Help Geniuses understand the basic structure of AI systems and why ethics and responsibility must be part of technical design.
-   Use slides to guide instruction and keep it interactive.

#### **Suggested Slide Flow**

-   **Slide 1: What Is an AI System?**
    -   An AI system takes in data, processes it using a model or learned pattern, and produces an output such as a prediction, classification, recommendation, or generated result.
    -   AI systems are not magic. They are technical systems with inputs, logic, outputs, and tradeoffs.
-   **Slide 2: Traditional Software vs AI Systems**
    -   Traditional software follows explicit rules written by humans.
    -   AI systems often learn patterns from data and make probabilistic outputs.
    -   Example:
        -   Traditional rule: "If password matches, log in."
        -   AI system: "Based on patterns, this image is probably a dog."
-   **Slide 3: Core Parts of an AI System**
    -   Input
    -   Data
    -   Model
    -   Processing
    -   Output
    -   Feedback or evaluation
    -   Human oversight
-   **Slide 4: Types of AI System Outputs**
    -   Classification
    -   Recommendation
    -   Detection
    -   Generation
    -   Ranking
    -   Prediction
-   **Slide 5: AI Systems Are Built on Data**
    -   Training data matters
    -   Input quality matters
    -   Missing or biased data affects results
    -   Garbage in, garbage out
-   **Slide 6: Responsible AI Core Ideas**
    -   Fairness
    -   Bias
    -   Privacy
    -   Safety
    -   Transparency
    -   Accountability
    -   Human oversight
-   **Slide 7: Why AI Ethics Belongs in AI Systems**
    -   Ethics is not separate from the system
    -   It affects:
        -   the data chosen
        -   the labels used
        -   the decisions automated
        -   the risks accepted
        -   the people impacted
-   **Slide 8: Real-World AI System Examples**
    -   Recommendation systems
    -   Object detection cameras
    -   AI writing tools
    -   Fraud detection systems
    -   Resume screening systems
    -   Image generators
    -   Route or scheduling tools
-   **Slide 9: Questions Technical Builders Should Ask**
    -   What data does this system need?
    -   What kind of output is it producing?
    -   Who is impacted if it is wrong?
    -   What kind of bias could appear?
    -   What guardrails or human review might be needed?
-   **Slide 10: This Week's Direction**
    -   Geniuses will explore what AI systems are, how they learn, and how responsibility changes technical design.

#### **Discussion Questions**

-   What makes an AI system different from basic software?
-   Why does data matter so much in AI systems?
-   Can an AI system be technically impressive and still irresponsible?
-   What kinds of users are most harmed when an AI system is wrong?
-   Why should a technical builder care about fairness and trust?

#### **Reflection Prompt**

-   Have Geniuses write for 4 minutes:
    -   "Describe one AI system you use or see in everyday life. What does it take in, and what does it give back?"

### 3. **Guided Practice (Time: 45 minutes)**

-   **Objective:** Help Geniuses apply technical systems thinking by building a simple Python program that breaks down an AI product into system parts and ethical considerations.
-   Explain that today's code-along is about thinking like an AI systems designer.
-   The class will create `ai_system_analyzer.py`.

#### **Guided Practice Build**

Create a folder called `ai-system-analyzer`.

#### **Project Goal**

Build a Python program that:

-   asks for the name of an AI system
-   asks what input it uses
-   asks what output it gives
-   asks what kind of task it performs
-   asks what risk could happen if it fails
-   prints a structured system summary

#### **Setup Steps**

1.  Open VS Code.
2.  Create a folder called `ai-system-analyzer`.
3.  Create a file called `ai_system_analyzer.py`.
4.  Run the file in the terminal.

#### **Sample Code**
```
# ai_system_analyzer.py
# AI Systems Week 1 Day 1
# This program helps a Genius describe the technical parts
# of an AI system and think about possible risks.

print("Welcome to the AI System Analyzer\n")

# Gather information about the AI system
system_name = input("What is the name of the AI system? ")
system_input = input("What kind of input does it use? ")
system_output = input("What kind of output does it produce? ")
system_task = input("What task does it perform (classification, generation, detection, recommendation, etc.)? ")
system_risk = input("What could go wrong if the system fails? ")

# Print a structured summary
print("\n--- AI System Summary ---")
print(f"System Name: {system_name}")
print(f"Input: {system_input}")
print(f"Output: {system_output}")
print(f"Task Type: {system_task}")
print(f"Possible Risk: {system_risk}")

# Add reflection questions
print("\n--- Responsible AI Reflection ---")
print("- What kind of data does this system depend on?")
print("- Who could be impacted if it makes mistakes?")
print("- What kind of human review or guardrail might be needed?")
```
#### **Guided Practice Teaching Points**

-   Why system inputs and outputs matter
-   Why naming the task type helps us understand the system
-   Why failure cases are part of technical design
-   Why even simple programs can help organize systems thinking
-   Why ethics questions belong next to technical questions

#### **Guided Practice Discussion**

-   What parts of the analyzer feel most useful?
-   What information is still missing from this tool?
-   How would a real company benefit from mapping systems this way?
-   What kinds of systems need the most caution?

### 4. **Independent Practice (Time: 35 minutes)**

-   **Objective:** Geniuses independently create the first version of their own AI system concept and analyze it technically and ethically.
-   This begins the Week 1 mini-project.

#### **Mini-Project Title**

**AI System Concept Brief --- Day 1 Foundation**

#### **Independent Task**

Each Genius creates a Python file that describes an AI system idea and breaks it into technical parts.

Their system concept must include:

-   system name
-   what kind of data or input it uses
-   what kind of output it gives
-   what task it performs
-   one major risk or ethical concern
-   one possible guardrail or responsible design choice

#### **Required Deliverables**

-   A working Python file called `my_ai_system.py`
-   A system concept with:
    -   system name
    -   input
    -   output
    -   task type
    -   one major risk
    -   one responsible design choice
-   A short written reflection:
    -   Why is this an AI system?
    -   What makes it technically interesting?
    -   What makes it important to build responsibly?

#### **Independent Practice Starter Code**
```
# my_ai_system.py
# Day 1 independent practice
# This program describes a Genius's AI system concept.

print("My AI System Concept\n")

system_name = "VisionAssist AI"
system_input = "Images from a phone camera"
system_output = "Descriptions of objects detected in the image"
system_task = "Object detection"
system_risk = "The system could miss important objects or identify them incorrectly"
responsible_choice = "The system should show uncertainty and remind users to double-check important situations"

print(f"System Name: {system_name}")
print(f"Input: {system_input}")
print(f"Output: {system_output}")
print(f"Task Type: {system_task}")
print(f"Possible Risk: {system_risk}")
print(f"Responsible Design Choice: {responsible_choice}")
```
#### **Facilitator Support Moves**

-   Help Geniuses choose systems with a clear task type
-   Ask:
    -   What is the system actually trying to do?
    -   What data does it need?
    -   What happens if it gets the result wrong?
    -   What kind of user would depend on this system?
-   Push Geniuses to be specific, not generic

### 5. **Closure (Time: 20 minutes)**

-   **Objective:** Reinforce that AI systems are technical systems with real consequences and real responsibilities.
-   Bring the class together for a final share-out.
-   Ask 3--5 Geniuses to share:
    -   their system name
    -   the type of task it performs
    -   one risk they identified
    -   one responsible design choice they added
-   Lead a closing discussion:
    -   What makes something an AI system?
    -   Why is responsibility part of technical design?
    -   What surprised you when you started breaking systems into inputs, tasks, and outputs?
-   Preview the next lesson:
    -   Geniuses will go deeper into how AI systems learn from data, including training data, labels, and the difference between supervised and unsupervised learning.

**Assessment:**
---------------

Student learning will be assessed through:

-   Participation in the icebreaker and discussion
-   Reflection responses during direct instruction
-   Completion of the guided Python code-along
-   Completion of an independent AI system concept brief
-   Final share-out and explanation of technical and ethical choices

### **Exit Ticket**

1.  What is an AI system?
2.  Name one part of an AI system.
3.  Why should a technical builder think about ethics and responsibility?

**Extra Activities:**
---------------------

-   Geniuses who finish early can:
    -   add a confidence level field
    -   add a "human review needed" field
    -   create multiple system examples in one file
    -   classify their example as low-risk or high-risk
    -   rewrite the program using functions
    -   add a menu of task types to choose from
-   Add a "data source" field
-   Add a "who is impacted" field
-   Add a "failure example" section
-   Add a second AI system and compare the two

**Reflection / Takeaways:**
---------------------------

This lesson works best when Geniuses realize that AI systems are not mysterious black boxes. They are technical systems made of data, models, processing, outputs, and decisions. Day 1 sets the tone for the course by showing that technical understanding and responsible design belong together. By the end of the lesson, Geniuses should feel that AI Systems is not just about using AI tools. It is about understanding the machinery, the choices, and the responsibilities behind them.

**Facilitator Notes**
---------------------

-   Keep using **Geniuses** consistently in examples and discussion.
-   Reinforce that ethics is not separate from technical systems design.
-   Keep examples current and relevant to products Geniuses already know.
-   Encourage clear technical language without making the content feel dry.
-   Remind Geniuses that tomorrow they will explore how AI systems learn from data and what makes labeled and unlabeled data so important.

**Week 1 Day 1 Mini-Project Connection**
----------------------------------------

By the end of Day 1, each Genius should have:

-   A named AI system concept
-   A clearly defined input and output
-   A task type such as classification, generation, detection, or recommendation
-   At least one ethical risk
-   At least one responsible design choice
-   A stronger understanding of what makes AI systems technical, powerful, and important to build responsibly
