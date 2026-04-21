<img src="https://github.com/Hgp-GeniusLabs/Curriculum/blob/10734f2c827128dde773ea4f266d154d46977866/Org-Wide/Assets/hgp_logo_original.png" width="150"/>

Lesson Plan: AI Systems Week 1, Day 3 --- Classification Systems, Predictions, and How AI Decides Between Categories
==================================================================================================================

**Duration:**
-------------

3 hours

**Lesson Overview:**
--------------------

On Day 3, Geniuses go deeper into one of the most common types of AI systems: **classification systems**. After learning what AI systems are and how they learn from data, Geniuses now focus on how systems make category-based decisions such as spam or not spam, cat or dog, fraud or not fraud, positive or negative, safe or unsafe. The lesson introduces classification as a technical system behavior built on data, patterns, and probability.

Geniuses explore how classifiers work, why classification is different from generation, and what kinds of real-world products depend on category decisions. They also examine what happens when a classifier is wrong and why confidence, bias, and evaluation matter. During guided practice, the class builds a simple Python classification simulator in VS Code that sorts examples into categories using rules and structured logic. During independent practice, each Genius creates a classifier concept tied to a real AI system use case and explains the categories, risks, and trust challenges involved. By the end of the lesson, Geniuses should understand that classification is one of the core building blocks of modern AI systems.

**Objectives:**
---------------

-   Define classification and explain how it works in AI systems.
-   Distinguish between classification systems and generative systems.
-   Identify common real-world AI products that rely on classification.
-   Explain how AI systems make category-based predictions from learned patterns.
-   Build a simple Python program that simulates a classifier.
-   Analyze classification risks such as wrong labels, low confidence, and harmful mistakes.
-   Continue the Week 1 mini-project by designing a classification-based AI system.

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
-   Optional cards or printed examples for category sorting activity

**Standards:**
--------------

-   Computational Thinking: Analyze how systems sort inputs into categories and make decisions.
-   Computer Science Practices: Explain how data patterns connect to predictions and categories.
-   Data Literacy: Interpret examples, labels, and outputs in classification tasks.
-   Digital Literacy: Evaluate the strengths, weaknesses, and risks of automated category decisions.
-   Career Readiness: Practice technical reasoning, categorization, and responsible systems thinking.
-   Technical Foundations: Explain classification as a major type of AI system behavior.

**Lesson Activity:**
--------------------

### 1. **Introduction (Time: 25 minutes)**

-   **Objective:** Energize Geniuses and introduce the idea that many AI systems exist mainly to decide what category something belongs to.
-   Start with a fun icebreaker called **"What Category Does It Belong To?"**
-   This should be the first thing and the most fun thing to wake Geniuses up and get them ready for the lesson.

#### **Icebreaker Option A: Physical Movement**

-   Label different parts of the room with categories such as:
    -   **Spam**
    -   **Not Spam**
    -   **Safe**
    -   **Unsafe**
    -   **Positive**
    -   **Negative**
-   Read examples aloud and have Geniuses move to the category they think fits best.
-   Example prompts:
    -   "You won a free gift card, click now!"
    -   "Hey, checking in about our meeting tomorrow"
    -   "This movie was incredible"
    -   "This app is terrible and frustrating"
    -   "This post may contain harmful content"
    -   "This image likely contains a stop sign"
-   After each round, ask:
    -   What clues helped you decide?
    -   Was the answer obvious or uncertain?
    -   Could two people classify it differently?
    -   What happens if an AI classifier gets this wrong?

#### **Icebreaker Option B: Card Sort**

-   Give Geniuses text snippets, simple images, or product examples.
-   Have them sort the examples into categories and discuss edge cases.
-   Use the discussion to introduce the idea that classifiers often deal with uncertainty, not perfect truth.

#### **Transition**

-   Say:
    -   "Many AI systems are not trying to write or create. They are trying to decide what something is."
-   Ask:
    -   Where do we see category decisions in everyday technology?
    -   Why might classification be powerful but also risky?

### 2. **Direct Instruction (Time: 55 minutes)**

-   **Objective:** Help Geniuses understand how classification systems work and why category decisions matter in real AI products.
-   Use slides to guide instruction and keep it interactive.

#### **Suggested Slide Flow**

-   **Slide 1: What Is Classification?**
    -   Classification means assigning an input to one category out of possible categories
    -   Example:
        -   spam / not spam
        -   cat / dog
        -   positive / negative
        -   fraud / not fraud
-   **Slide 2: Classification Is Everywhere**
    -   email spam filters
    -   facial recognition categories
    -   sentiment analysis
    -   moderation systems
    -   medical screening tools
    -   recommendation triggers
    -   fraud detection
-   **Slide 3: How a Classifier Works**
    -   Input comes in
    -   System compares it to patterns learned from data
    -   System predicts the most likely category
    -   Output may include confidence or score
-   **Slide 4: Classification vs Generation**
    -   Classification:
        -   decides between categories
        -   predicts labels
    -   Generation:
        -   creates new text, images, audio, or video
    -   Both are AI, but they behave differently
-   **Slide 5: Binary vs Multi-Class Classification**
    -   **Binary:** two categories
        -   spam / not spam
        -   fraud / not fraud
    -   **Multi-class:** more than two categories
        -   dog / cat / bird
        -   sports / politics / entertainment
-   **Slide 6: Features and Signals**
    -   Classifiers look at signals in the data
    -   Example in text:
        -   words
        -   tone
        -   punctuation
    -   Example in images:
        -   shapes
        -   colors
        -   patterns
-   **Slide 7: Confidence and Uncertainty**
    -   A classifier may not be equally sure every time
    -   Confidence matters because low-confidence decisions may need caution or human review
-   **Slide 8: What Can Go Wrong?**
    -   weak training data
    -   biased labels
    -   unclear categories
    -   low confidence
    -   harmful false positives or false negatives
-   **Slide 9: Responsible Classification**
    -   ask who is affected by errors
    -   know when human review is needed
    -   understand the consequences of misclassification
    -   do not assume category systems are neutral
-   **Slide 10: This Week's Direction**
    -   Geniuses will continue learning how systems classify, detect, and generate so they can design stronger AI applications later

#### **Discussion Questions**

-   Why is classification different from generation?
-   What are examples of binary classification and multi-class classification?
-   Why is confidence important in classification systems?
-   What kinds of mistakes are most dangerous in real-world classifiers?
-   When should a classifier's decision be checked by a human?

#### **Reflection Prompt**

-   Have Geniuses write for 4 minutes:
    -   "Describe one real AI system that likely uses classification. What categories is it deciding between?"

### 3. **Guided Practice (Time: 45 minutes)**

-   **Objective:** Help Geniuses apply classification thinking by building a simple Python program that simulates a classifier.
-   Explain that today's code-along is not full machine learning training. It is about understanding classification behavior and logic.
-   The class will create `classification_simulator.py`.

#### **Guided Practice Build**

Create a folder called `classification-simulator`.

#### **Project Goal**

Build a Python program that:

-   asks for a short message
-   checks for certain signals or keywords
-   classifies the message into a category
-   prints the result and a basic confidence-style explanation

#### **Setup Steps**

1.  Open VS Code.
2.  Create a folder called `classification-simulator`.
3.  Create a file called `classification_simulator.py`.
4.  Run the file in the terminal.

#### **Sample Code**
```
# classification_simulator.py
# AI Systems Week 1 Day 3
# This program simulates a simple spam classifier using keyword rules.

print("Welcome to the Classification Simulator\n")

# Ask the user for a message
message = input("Enter a message to classify: ").lower()

# Define simple spam signal words
spam_keywords = ["free", "win", "gift card", "click now", "urgent", "prize"]

# Count how many spam keywords appear
spam_score = 0

for word in spam_keywords:
    if word in message:
        spam_score += 1

# Make a simple classification decision
if spam_score >= 2:
    classification = "spam"
    confidence = "high"
elif spam_score == 1:
    classification = "possibly spam"
    confidence = "medium"
else:
    classification = "not spam"
    confidence = "low"

# Print the result
print("\n--- Classification Result ---")
print(f"Category: {classification}")
print(f"Confidence: {confidence}")
print(f"Spam Score: {spam_score}")

# Reflection
print("\n--- Reflection ---")
print("This is a rule-based simulation of classification.")
print("Real AI classifiers learn patterns from data instead of using only fixed keywords.")
```
#### **Guided Practice Teaching Points**

-   Why classification systems often rely on patterns and signals
-   Why this example is a simulation, not a full trained model
-   Why confidence matters even in simple decision systems
-   Why category definitions affect the whole system
-   Why rule-based logic helps us understand classifier behavior

#### **Guided Practice Discussion**

-   What made the message seem like spam or not spam?
-   What are the limits of a keyword-only classifier?
-   What would a real model likely do better?
-   Could this system still make mistakes?

### 4. **Independent Practice (Time: 35 minutes)**

-   **Objective:** Geniuses independently create a classifier concept tied to a real use case and describe the categories, risks, and trust decisions involved.
-   This continues the Week 1 mini-project.

#### **Mini-Project Title**

**AI System Concept Brief --- Day 3 Classification Design**

#### **Independent Task**

Each Genius creates a Python file for a classification-based AI system.

Their concept must include:

-   system name
-   what kind of input it classifies
-   what categories it predicts
-   whether it is binary or multi-class
-   one possible risk if it gets the classification wrong
-   one trust or review improvement

Examples:

-   study support mood classifier
-   email spam detector
-   sentiment analyzer
-   image category classifier
-   safety content classifier
-   task priority classifier

#### **Required Deliverables**

-   A working Python file called `my_classifier.py`
-   A classification system concept with:
    -   system name
    -   input type
    -   category options
    -   binary or multi-class explanation
    -   one major risk
    -   one trust improvement
-   A short written reflection:
    -   Why is this a classification system?
    -   What signals or features might it look at?
    -   What happens if it classifies something incorrectly?

#### **Independent Practice Starter Code**
```
# my_classifier.py
# Day 3 independent practice
# This program describes a Genius's classification system concept.

print("My Classification System\n")

system_name = "MoodCheck AI"
input_type = "Short text reflections written by students"
categories = "stressed, calm, excited, frustrated"
classification_type = "multi-class"
risk = "The system could misunderstand someone's feelings and suggest the wrong support"
trust_improvement = "The system should let the user confirm or reject the result instead of assuming it is always correct"

print(f"System Name: {system_name}")
print(f"Input Type: {input_type}")
print(f"Categories: {categories}")
print(f"Classification Type: {classification_type}")
print(f"Risk: {risk}")
print(f"Trust Improvement: {trust_improvement}")
```
#### **Facilitator Support Moves**

-   Help Geniuses choose a clear category-based task
-   Ask:
    -   What exactly is the system deciding between?
    -   Are the categories clear or messy?
    -   What kinds of clues would the model use?
    -   Who is harmed if the system guesses wrong?
-   Encourage realistic and thoughtful classification choices

### 5. **Closure (Time: 20 minutes)**

-   **Objective:** Reinforce that classification is a major AI systems behavior and that category decisions can have real consequences.
-   Bring the class together for a final share-out.
-   Ask 3--5 Geniuses to share:
    -   their system name
    -   what it classifies
    -   whether it is binary or multi-class
    -   one risk they identified
-   Lead a closing discussion:
    -   What makes classification different from generation?
    -   Why do classifiers need trust and caution?
    -   What surprised you about how many products rely on classification?
-   Preview the next lesson:
    -   Geniuses will move into recommendation, ranking, and pattern-based systems, and compare how systems go beyond simple categories into scoring and suggestion behavior.

**Assessment:**
---------------

Student learning will be assessed through:

-   Participation in the icebreaker and discussion
-   Reflection responses during direct instruction
-   Completion of the guided Python code-along
-   Completion of an independent classifier concept
-   Final share-out and explanation of classification choices

### **Exit Ticket**

1.  What is classification?
2.  What is the difference between binary and multi-class classification?
3.  Why does confidence or human review matter in classification systems?

**Extra Activities:**
---------------------

-   Geniuses who finish early can:
    -   add more categories to their classifier
    -   simulate a confidence score more explicitly
    -   build a sentiment classifier instead of spam
    -   compare rule-based classification and learned classification in writing
    -   create two test examples and see how their logic behaves
    -   rewrite their program using functions
-   Add a "human review needed" condition for uncertain results
-   Add a second type of classifier in the same file
-   Add example test cases
-   Add a section that explains false positives and false negatives

**Reflection / Takeaways:**
---------------------------

This lesson works best when Geniuses realize that classification is one of the most common and powerful behaviors inside AI systems. Day 3 helps make category-based prediction feel less abstract by connecting it to products they already know and by letting them simulate the logic themselves. By the end of the lesson, Geniuses should feel more confident explaining what a classifier does, how it differs from other AI systems, and why responsibility matters when a system makes decisions about what something is.

**Facilitator Notes**
---------------------

-   Keep using **Geniuses** consistently in examples and discussion.
-   Reinforce that classification systems often operate with uncertainty, not perfect truth.
-   Encourage discussion about harmful mistakes and trust, not just technical accuracy.
-   Keep classification examples current and grounded in real products.
-   Remind Geniuses that tomorrow they will explore recommendation, ranking, and pattern-finding systems that move beyond simple categories.

**Week 1 Day 3 Mini-Project Connection**
----------------------------------------

By the end of Day 3, each Genius should have:

-   A named classification-based AI system concept
-   A defined input type
-   Clear category outputs
-   A binary or multi-class classification explanation
-   At least one identified system risk
-   At least one trust or review improvement
-   A stronger understanding of classification as a core AI systems behavior
