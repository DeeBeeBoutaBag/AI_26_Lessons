<img src="https://github.com/Hgp-GeniusLabs/Curriculum/blob/10734f2c827128dde773ea4f266d154d46977866/Org-Wide/Assets/hgp_logo_original.png" width="150"/>

Lesson Plan: AI Systems Week 1, Day 2 --- How AI Systems Learn: Data, Labels, Supervised Learning, and Unsupervised Learning
==========================================================================================================================

**Duration:**
-------------

3 hours

**Lesson Overview:**
--------------------

On Day 2, Geniuses move from defining AI systems to understanding how many of those systems actually learn. The lesson introduces the role of data, labels, patterns, and training in modern AI systems. Geniuses explore the difference between **supervised learning** and **unsupervised learning** and begin to understand why some systems need labeled examples while others group, organize, or find patterns on their own.

The lesson emphasizes that models are only as strong as the data and learning setup behind them. Geniuses examine how labeled and unlabeled data shape system behavior and why data quality matters for fairness, trust, and performance. During guided practice, the class builds a Python-based data sorter that simulates simple supervised and unsupervised thinking. During independent practice, each Genius creates a small AI learning concept around a real use case and explains what kind of data and learning setup it would need. By the end of the lesson, Geniuses should understand that AI systems do not just "know" things. They learn from examples, patterns, and structure.

**Objectives:**
---------------

-   Explain how AI systems learn from data.
-   Define training data, labels, features, and patterns in student-friendly language.
-   Distinguish between supervised learning and unsupervised learning.
-   Identify when a system might need labeled data and when it might use unlabeled data.
-   Build a simple Python program that organizes examples into labeled and unlabeled groups.
-   Analyze how data quality affects the strength and responsibility of an AI system.
-   Continue the Week 1 mini-project by connecting an AI system idea to a learning setup.

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
-   Optional printed cards or sticky notes for labeled and unlabeled data activity

**Standards:**
--------------

-   Computational Thinking: Analyze how systems use examples, patterns, and structure to learn from data.
-   Computer Science Practices: Explain the relationship between data, labels, and model behavior.
-   Data Literacy: Distinguish between labeled and unlabeled data and explain why data quality matters.
-   Digital Literacy: Evaluate how weak or biased data can affect AI system performance and fairness.
-   Career Readiness: Practice technical reasoning, categorization, and systems analysis.
-   Technical Foundations: Explain supervised and unsupervised learning in modern AI systems.

**Lesson Activity:**
--------------------

### 1. **Introduction (Time: 25 minutes)**

-   **Objective:** Energize Geniuses and introduce the idea that AI systems learn in different ways depending on the kind of data they are given.
-   Start with a fun icebreaker called **"Labeled or Unlabeled?"**
-   This should be the first thing and the most fun thing to wake Geniuses up and get them ready for the lesson.

#### **Icebreaker Option A: Physical Movement**

-   Label one side of the room **"Labeled Data"** and the other side **"Unlabeled Data."**
-   Read examples aloud and have Geniuses move to the side they think fits best.
-   Example prompts:
    -   A folder of images where each one is tagged "cat" or "dog"
    -   A list of songs grouped only by listening patterns, with no names for the groups
    -   Emails marked "spam" and "not spam"
    -   Customer behavior data with no category labels yet
    -   Photos labeled "contains a stop sign" and "does not contain a stop sign"
    -   A dataset of shopping habits with no labels, used to find similar customer groups
-   After each round, ask:
    -   What made this labeled or unlabeled?
    -   What kind of system could use this?
    -   Why might labels help a model?
    -   Why might we still want unlabeled data?

#### **Icebreaker Option B: Card Sort**

-   Give Geniuses cards with examples of datasets.
-   Have them sort the cards into:
    -   supervised learning
    -   unsupervised learning
-   Discuss edge cases and why the distinction matters.

#### **Transition**

-   Say:
    -   "AI systems do not just appear fully formed. Many of them learn from examples, patterns, and structure."
-   Ask:
    -   What would a model need in order to learn the difference between two categories?
    -   What could a model still discover even if nobody labeled the data?

### 2. **Direct Instruction (Time: 55 minutes)**

-   **Objective:** Help Geniuses understand how learning works in AI systems and how supervised and unsupervised learning differ.
-   Use slides to guide instruction and keep it interactive.

#### **Suggested Slide Flow**

-   **Slide 1: How Do AI Systems Learn?**
    -   Many AI systems learn from data
    -   The system looks for patterns that connect inputs to outputs or groups
-   **Slide 2: Key Learning Vocabulary**
    -   **Data:** examples the system learns from
    -   **Label:** the correct answer or category attached to an example
    -   **Feature:** a part of the data that may help the model notice patterns
    -   **Training:** the process of learning from many examples
    -   **Prediction:** what the model says on new data
-   **Slide 3: What Is Supervised Learning?**
    -   The model learns from examples with labels
    -   It is shown the input and the correct answer
    -   Example:
        -   image → labeled as "dog"
        -   email → labeled as "spam"
-   **Slide 4: What Is Unsupervised Learning?**
    -   The model learns from data without labels
    -   It looks for patterns, groups, or structure on its own
    -   Example:
        -   grouping similar customer behavior
        -   clustering songs or articles by similarity
-   **Slide 5: Supervised Learning Examples**
    -   spam detection
    -   image classification
    -   sentiment analysis
    -   fraud detection
    -   recommendation signals with known outcomes
-   **Slide 6: Unsupervised Learning Examples**
    -   customer segmentation
    -   clustering similar products
    -   grouping users by behavior
    -   discovering hidden patterns in large datasets
-   **Slide 7: Labels Are Powerful**
    -   Labels tell the system what the correct pattern should lead to
    -   But labels can also be:
        -   expensive to create
        -   inconsistent
        -   biased
        -   incomplete
-   **Slide 8: Why Data Quality Matters**
    -   weak data leads to weak learning
    -   biased data leads to biased systems
    -   missing examples can hurt performance
    -   more data is not always better if it is messy or unfair
-   **Slide 9: Choosing the Right Learning Setup**
    -   supervised learning works well when you know the target category
    -   unsupervised learning works well when you want to discover patterns first
    -   builders need to ask what the system is trying to learn
-   **Slide 10: This Week's Direction**
    -   Geniuses will keep exploring how AI systems classify, detect, generate, and reason from data

#### **Discussion Questions**

-   Why are labels helpful in supervised learning?
-   What could go wrong if labels are wrong or biased?
-   When might unsupervised learning be more useful?
-   Why does data quality matter just as much as model quality?
-   What kind of learning setup would fit your AI system idea?

#### **Reflection Prompt**

-   Have Geniuses write for 4 minutes:
    -   "Think about an AI system idea. Would it need labeled data, unlabeled data, or both? Why?"

### 3. **Guided Practice (Time: 45 minutes)**

-   **Objective:** Help Geniuses apply learning concepts by building a simple Python program that organizes and explains labeled and unlabeled examples.
-   Explain that today's code-along is not full model training. It is about understanding data and learning setup.
-   The class will create `learning_data_sorter.py`.

#### **Guided Practice Build**

Create a folder called `learning-data-sorter`.

#### **Project Goal**

Build a Python program that:

-   stores examples of labeled and unlabeled data
-   prints them clearly
-   explains whether they fit supervised or unsupervised learning
-   helps Geniuses think like AI systems builders

#### **Setup Steps**

1.  Open VS Code.
2.  Create a folder called `learning-data-sorter`.
3.  Create a file called `learning_data_sorter.py`.
4.  Run the file in the terminal.

#### **Sample Code**
```
# learning_data_sorter.py
# AI Systems Week 1 Day 2
# This program helps a Genius understand labeled and unlabeled data
# and connect them to supervised and unsupervised learning.

print("Welcome to the Learning Data Sorter\n")

# Examples of labeled data
labeled_examples = [
    {"input": "Email: You won a free phone!", "label": "spam"},
    {"input": "Image of a golden retriever", "label": "dog"},
    {"input": "Review: This movie was amazing", "label": "positive"}
]

# Examples of unlabeled data
unlabeled_examples = [
    "Customer purchase history from 500 shoppers",
    "A folder of songs grouped only by listening patterns",
    "Website behavior data with no categories yet"
]

print("--- Supervised Learning Examples (Labeled Data) ---")
for example in labeled_examples:
    print(f"Input: {example['input']}")
    print(f"Label: {example['label']}\n")

print("--- Unsupervised Learning Examples (Unlabeled Data) ---")
for example in unlabeled_examples:
    print(f"Input: {example}\n")

print("--- Reflection ---")
print("Supervised learning uses labeled data to learn known categories or answers.")
print("Unsupervised learning uses unlabeled data to discover patterns or groups.")
```
#### **Guided Practice Teaching Points**

-   Why labeled examples are easier to use for known tasks
-   Why unlabeled data can still be valuable
-   Why categorizing datasets is part of technical design
-   Why builders need to know what the model is supposed to learn
-   Why data preparation is a real part of AI systems work

#### **Guided Practice Discussion**

-   Which examples clearly fit supervised learning?
-   Which ones fit unsupervised learning?
-   Could some systems use both?
-   What would happen if the labels were inconsistent?

### 4. **Independent Practice (Time: 35 minutes)**

-   **Objective:** Geniuses independently connect their AI system idea to a real learning setup and describe what kind of data it would need.
-   This continues the Week 1 mini-project.

#### **Mini-Project Title**

**AI System Concept Brief --- Day 2 Learning Setup**

#### **Independent Task**

Each Genius updates or creates a Python file that describes how their AI system would learn.

Their concept must include:

-   system name
-   whether it would use supervised learning, unsupervised learning, or both
-   one example of the data it would use
-   whether the data needs labels
-   one possible risk tied to the data
-   one improvement that would make the system more trustworthy

#### **Required Deliverables**

-   A working Python file called `my_learning_setup.py`
-   A learning setup with:
    -   system name
    -   learning type
    -   example data
    -   labeled or unlabeled explanation
    -   one risk
    -   one trust improvement
-   A short written reflection:
    -   Why does this learning setup fit your AI system?
    -   What kind of data would be hardest to collect well?
    -   What could go wrong if the training data is weak?

#### **Independent Practice Starter Code**
```
# my_learning_setup.py
# Day 2 independent practice
# This program describes how a Genius's AI system could learn from data.

print("My AI Learning Setup\n")

system_name = "VisionAssist AI"
learning_type = "supervised learning"
example_data = "Images labeled with objects such as backpack, chair, laptop, and stop sign"
needs_labels = "yes"
data_risk = "The labels could be wrong or the images might not represent all environments equally"
trust_improvement = "Use more diverse training images and review label quality carefully"

print(f"System Name: {system_name}")
print(f"Learning Type: {learning_type}")
print(f"Example Data: {example_data}")
print(f"Needs Labels: {needs_labels}")
print(f"Data Risk: {data_risk}")
print(f"Trust Improvement: {trust_improvement}")
```
#### **Facilitator Support Moves**

-   Help Geniuses choose a realistic learning type
-   Ask:
    -   Is the system trying to predict a known label or discover patterns?
    -   What would the data actually look like?
    -   Who decides the labels?
    -   What kind of bias might show up in the data?
-   Encourage clear and specific examples

### 5. **Closure (Time: 20 minutes)**

-   **Objective:** Reinforce that AI learning depends on data structure, labels, and quality, not magic.
-   Bring the class together for a final share-out.
-   Ask 3--5 Geniuses to share:
    -   their system name
    -   whether it uses supervised or unsupervised learning
    -   one kind of data it needs
    -   one risk they identified
-   Lead a closing discussion:
    -   What is the difference between supervised and unsupervised learning?
    -   Why does data quality matter so much?
    -   What surprised you when thinking about how systems learn?
-   Preview the next lesson:
    -   Geniuses will go deeper into classification and prediction systems and start building a simple classifier-style logic flow.

**Assessment:**
---------------

Student learning will be assessed through:

-   Participation in the icebreaker and discussion
-   Reflection responses during direct instruction
-   Completion of the guided Python code-along
-   Completion of an independent learning setup brief
-   Final share-out and explanation of data and learning choices

### **Exit Ticket**

1.  What is supervised learning?
2.  What is unsupervised learning?
3.  Why does data quality matter in AI systems?

**Extra Activities:**
---------------------

-   Geniuses who finish early can:
    -   add more labeled and unlabeled examples
    -   compare two learning setups in one file
    -   sort examples using a menu system
    -   create a "data quality checklist" section
    -   rewrite the program using dictionaries and loops
    -   add a "who labels the data?" prompt
-   Add a section on biased labels
-   Add a confidence field for how trustworthy the data is
-   Add a second AI system and compare which learning type fits better
-   Add a short explanation of when a system might need both supervised and unsupervised methods

**Reflection / Takeaways:**
---------------------------

This lesson works best when Geniuses realize that AI systems learn from structure, examples, and data choices. Day 2 makes it clear that supervised and unsupervised learning are not abstract buzzwords. They are different ways systems find patterns and make sense of information. By the end of the lesson, Geniuses should feel more confident describing how an AI system learns and more aware that the quality of the learning process depends heavily on the quality of the data behind it.

**Facilitator Notes**
---------------------

-   Keep using **Geniuses** consistently in examples and discussion.
-   Reinforce that labels are powerful but can also introduce mistakes and bias.
-   Keep the lesson grounded in real examples rather than only abstract definitions.
-   Encourage Geniuses to talk through what kind of data their own systems would need.
-   Remind Geniuses that tomorrow they will explore classification more directly and begin thinking about how systems make decisions between categories.

**Week 1 Day 2 Mini-Project Connection**
----------------------------------------

By the end of Day 2, each Genius should have:

-   A named AI system concept
-   A clearer sense of how that system would learn
-   A defined learning type such as supervised, unsupervised, or both
-   An example of the data it would need
-   An explanation of whether labels are required
-   At least one data-related risk
-   At least one trust improvement connected to the learning setup
