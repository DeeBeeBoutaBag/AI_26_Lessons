<img src="https://github.com/Hgp-GeniusLabs/Curriculum/blob/10734f2c827128dde773ea4f266d154d46977866/Org-Wide/Assets/hgp_logo_original.png" width="150"/>

Lesson Plan: AI Systems Week 1, Day 5 --- Ranking, Recommendation, Pattern Systems, and Week 1 AI Systems Showcase
================================================================================================================

**Duration:**
-------------

3 hours

**Lesson Overview:**
--------------------

Day 5 brings together everything Geniuses explored in Week 1: what AI systems are, how they learn from data, how classification works, and how rule-based systems compare to AI-powered systems. The new focus for today is **ranking, recommendation, and pattern systems**. Geniuses learn that many modern AI systems do not just classify something into one category. They score, rank, suggest, sort, prioritize, and recommend what should come next. This lesson helps Geniuses understand another major kind of AI system behavior that appears in playlists, shopping sites, feeds, task prioritization tools, and personalized support systems.

During guided practice, the class builds a simple Python-based recommendation and ranking simulator that takes user preferences and returns ordered suggestions. Geniuses examine how recommendation systems depend on data, patterns, scoring, and user context, and they discuss how these systems can be useful but also biased, repetitive, or manipulative. During independent practice, each Genius extends their Week 1 mini-project into a broader AI system concept that includes input, learning type, task type, responsible design, and either classification, recommendation, or ranking behavior. The lesson ends with a Week 1 showcase that prepares Geniuses for the next week of deeper technical system design.

**Objectives:**
---------------

-   Explain how ranking and recommendation systems differ from classification systems.
-   Identify real-world AI products that use scoring, prioritization, and recommendation behavior.
-   Build a simple Python recommendation and ranking simulator.
-   Analyze how recommendation systems depend on user data, patterns, and assumptions.
-   Identify trust and ethics issues in ranking and recommendation systems.
-   Combine Week 1 learning into a stronger AI system concept brief.
-   Reflect on how technical system design and responsible AI belong together.

**Materials:**
--------------

-   Laptops for all Geniuses
-   VS Code installed
-   Python installed and working
-   OpenAI API key access if needed for extension work
-   Internet access
-   Projector or display
-   Whiteboard and markers
-   Slide deck for lecture and discussion
-   Reflection journal or digital notes
-   Terminal access in VS Code
-   Starter folder for Python files
-   Existing Week 1 project files

**Standards:**
--------------

-   Computational Thinking: Analyze how systems sort, score, and prioritize information for users.
-   Computer Science Practices: Build and test pattern-based systems using structured logic.
-   Data Literacy: Explain how user preferences and data signals shape ranked outputs.
-   Digital Literacy: Evaluate the fairness, usefulness, and risks of recommendation systems.
-   Career Readiness: Practice technical explanation, critique, and system reasoning.
-   Technical Foundations: Distinguish between classification, recommendation, and ranking as different AI system behaviors.

**Lesson Activity:**
--------------------

### 1. **Introduction (Time: 25 minutes)**

-   **Objective:** Energize Geniuses and introduce the idea that many AI systems are designed to decide what should be shown, suggested, or prioritized first.
-   Start with a fun icebreaker called **"Why Did It Recommend That?"**
-   This should be the first thing and the most fun thing to wake Geniuses up and get them ready for the lesson.

#### **Icebreaker Option A: Physical Movement**

-   Label different parts of the room:
    -   **Recommendation**
    -   **Ranking**
    -   **Classification**
-   Read product behaviors aloud and have Geniuses move to the category they think fits best.
-   Example prompts:
    -   A music app suggests songs you may like
    -   A spam filter labels a message as junk
    -   A shopping site puts some products at the top of the page
    -   A video app suggests what to watch next
    -   A moderation system marks a comment as unsafe
    -   A study tool suggests which assignment should be done first
    -   A search engine decides which results appear at the top
-   After each round, ask:
    -   Why is this recommendation, ranking, or classification?
    -   What data might the system be using?
    -   Is the system helping, influencing, or both?
    -   What could go wrong if the system keeps reinforcing the same patterns?

#### **Icebreaker Option B: Feed and Playlist Breakdown**

-   Ask Geniuses to think about apps they use that recommend, rank, or prioritize.
-   Have them list:
    -   what the system is probably using as input
    -   what it is optimizing for
    -   why the user sees what they see
-   Share out and discuss how invisible these systems can feel in everyday life.

#### **Transition**

-   Say:
    -   "Some AI systems decide what something is. Other AI systems decide what you should see next."
-   Ask:
    -   What is the difference between labeling something and recommending something?
    -   Why do ranking systems have so much power over attention and choices?

### 2. **Direct Instruction (Time: 50 minutes)**

-   **Objective:** Help Geniuses understand ranking, recommendation, and pattern systems as major AI system behaviors.
-   Use slides to guide instruction and keep it interactive.

#### **Suggested Slide Flow**

-   **Slide 1: What Comes Next?**
    -   Many AI systems do not only label inputs
    -   They also suggest, sort, rank, and prioritize outputs
-   **Slide 2: What Is a Recommendation System?**
    -   A recommendation system suggests items, actions, or next steps based on patterns
    -   Examples:
        -   music suggestions
        -   shopping suggestions
        -   movie recommendations
        -   learning next steps
        -   personalized support suggestions
-   **Slide 3: What Is a Ranking System?**
    -   A ranking system orders results based on a score or priority
    -   Examples:
        -   search results
        -   social media feeds
        -   product listings
        -   task prioritization
-   **Slide 4: Classification vs Recommendation vs Ranking**
    -   **Classification:** what category is this?
    -   **Recommendation:** what might this user want next?
    -   **Ranking:** what should appear first or higher?
-   **Slide 5: What Recommendation Systems Use**
    -   user history
    -   clicks
    -   likes
    -   preferences
    -   similar users
    -   item similarity
    -   timing or context
-   **Slide 6: What Ranking Systems Use**
    -   relevance
    -   confidence score
    -   popularity
    -   urgency
    -   match to user needs
    -   business priorities
-   **Slide 7: Pattern Systems Are Powerful**
    -   they influence attention
    -   they shape decisions
    -   they save time
    -   they can also create repetition, filter bubbles, or unfair visibility
-   **Slide 8: Risks in Recommendation and Ranking**
    -   bias in what gets shown
    -   repetition and lack of diversity
    -   pushing what is profitable instead of what is best
    -   hidden assumptions
    -   over-personalization
-   **Slide 9: Responsible Pattern Systems**
    -   explain why something is suggested
    -   allow user control
    -   include diversity in results
    -   avoid manipulative ranking
    -   use trust and fairness thinking
-   **Slide 10: Week 1 Wrap-Up**
    -   AI systems can classify, recommend, rank, detect, and generate
    -   strong builders understand both system behavior and system responsibility

#### **Discussion Questions**

-   What makes recommendation systems useful?
-   What makes them risky?
-   How is ranking different from recommendation?
-   Why might two users see different outputs from the same system?
-   What kinds of ranking systems should be designed with extra caution?

#### **Reflection Prompt**

-   Have Geniuses write for 4 minutes:
    -   "Think of one app that recommends or ranks content for you. What patterns do you think it is using?"

### 3. **Guided Practice (Time: 45 minutes)**

-   **Objective:** Help Geniuses build a simple Python recommendation and ranking simulator.
-   Explain that today's code-along is about modeling pattern-based system behavior.
-   The class will create `recommendation_ranker.py`.

#### **Guided Practice Build**

Create a folder called `recommendation-ranker`.

#### **Project Goal**

Build a Python program that:

-   asks the user for preferences
-   scores a list of items based on those preferences
-   ranks the items from strongest match to weakest
-   prints the ordered recommendation list

#### **Setup Steps**

1.  Open VS Code.
2.  Create a folder called `recommendation-ranker`.
3.  Create a file called `recommendation_ranker.py`.
4.  Run the file in the terminal.

#### **Sample Code**
```
# recommendation_ranker.py
# AI Systems Week 1 Day 5
# This program simulates a simple recommendation and ranking system.

print("Welcome to the Recommendation Ranker\n")

# Ask the user for interests
interest_1 = input("Enter one interest: ").lower()
interest_2 = input("Enter another interest: ").lower()

# Example items the system could recommend
items = [
    {"name": "Intro to Python Workshop", "tags": ["technology", "coding", "problem solving"]},
    {"name": "Community Leadership Lab", "tags": ["leadership", "community", "service"]},
    {"name": "AI Design Sprint", "tags": ["technology", "design", "innovation"]},
    {"name": "Career Exploration Panel", "tags": ["career", "leadership", "future"]},
    {"name": "Media Arts Studio", "tags": ["design", "creativity", "art"]}
]

# Score items based on matching interests
for item in items:
    score = 0

    if interest_1 in item["tags"]:
        score += 1
    if interest_2 in item["tags"]:
        score += 1

    item["score"] = score

# Rank items from highest score to lowest
ranked_items = sorted(items, key=lambda item: item["score"], reverse=True)

# Print results
print("\n--- Ranked Recommendations ---")
for item in ranked_items:
    print(f"{item['name']} | Score: {item['score']} | Tags: {', '.join(item['tags'])}")

print("\n--- Reflection ---")
print("This is a simple recommendation system based on matching interests.")
print("Real recommendation systems may use more data, behavior patterns, and user history.")
```
#### **Guided Practice Teaching Points**

-   Why ranking needs some kind of scoring logic
-   Why recommendations depend on patterns and user context
-   Why the same system may give different outputs to different users
-   Why recommendation systems can feel helpful and influential at the same time
-   Why simple simulations help us understand bigger AI system behavior

#### **Guided Practice Discussion**

-   What made an item rank higher?
-   How could this system become smarter?
-   What data would a real system use beyond two typed interests?
-   How could this system become repetitive or unfair?

### 4. **Independent Practice (Time: 35 minutes)**

-   **Objective:** Geniuses independently extend their Week 1 AI system concept into a fuller technical and responsible design brief.
-   This completes the Week 1 mini-project.

#### **Mini-Project Title**

**Week 1 AI System Concept Brief --- System Behavior and Responsibility**

#### **Independent Task**

Each Genius updates their project into a stronger AI system concept that includes:

-   system name
-   input type
-   output type
-   task type
-   learning type
-   whether it classifies, recommends, ranks, detects, or generates
-   one major risk
-   one responsible design choice
-   one explanation of why the system matters

They may use Python to print the concept in a structured format.

#### **Required Deliverables**

-   A working Python file called `week1_ai_system_brief.py`
-   A complete concept brief with:
    -   system name
    -   input
    -   output
    -   task type
    -   learning type
    -   system behavior
    -   one major risk
    -   one responsible design choice
    -   one short mission statement
-   A short written reflection:
    -   What type of AI system is this?
    -   What kind of data would it depend on?
    -   What makes it important to build responsibly?

#### **Independent Practice Starter Code**
```
# week1_ai_system_brief.py
# Week 1 independent practice
# This program prints a structured AI system concept brief.

print("Week 1 AI System Brief\n")

system_name = "PathSuggest AI"
input_type = "Student interests and goals"
output_type = "Ranked learning and career suggestions"
task_type = "Recommendation and ranking"
learning_type = "Could use supervised learning, pattern data, or recommendation logic"
system_behavior = "Suggests and ranks next-step opportunities"
major_risk = "The system could keep recommending narrow options and miss broader possibilities"
responsible_design = "The system should include diverse suggestions and explain why items are recommended"
mission_statement = "Help Geniuses discover meaningful next steps with clearer and more supportive guidance"

print(f"System Name: {system_name}")
print(f"Input Type: {input_type}")
print(f"Output Type: {output_type}")
print(f"Task Type: {task_type}")
print(f"Learning Type: {learning_type}")
print(f"System Behavior: {system_behavior}")
print(f"Major Risk: {major_risk}")
print(f"Responsible Design Choice: {responsible_design}")
print(f"Mission Statement: {mission_statement}")

#### **Facilitator Support Moves**

-   Help Geniuses decide what type of system behavior best fits their idea
-   Ask:
    -   Is the system deciding a category, suggesting a next step, or creating something?
    -   What kind of user data would shape the output?
    -   What is the most important risk?
    -   What would make the system more trustworthy?
-   Encourage Geniuses to make the brief clear and realistic

### 5. **Closure (Time: 25 minutes)**

-   **Objective:** Reinforce the technical ideas from Week 1 and help Geniuses see how different AI system behaviors connect.
-   Bring the class together for a Week 1 showcase.
-   Ask 3--5 Geniuses to share:
    -   their system name
    -   what type of system it is
    -   what behavior it uses
    -   one major risk
    -   one responsible design choice
-   Lead a closing discussion:
    -   What are the main types of AI system behavior we explored this week?
    -   How is recommendation different from classification?
    -   Why does technical understanding matter for responsible AI?
    -   What are you most curious about next?
-   Preview the next lesson:
    -   Week 2 will move into deeper technical AI system types such as vision systems, object detection, and how computers interpret images and visual data.

**Assessment:**
---------------

Student learning will be assessed through:

-   Participation in the icebreaker and discussion
-   Reflection responses during direct instruction
-   Completion of the guided Python recommendation/ranking simulator
-   Completion of a full Week 1 AI system concept brief
-   Final showcase and explanation of technical and responsible design choices

### **Exit Ticket**

1.  What is the difference between classification and recommendation?
2.  What is a ranking system?
3.  What is one risk in recommendation or ranking systems?

**Extra Activities:**
---------------------

-   Geniuses who finish early can:
    -   add more interests and item tags to the recommender
    -   add weighted scoring
    -   sort by multiple factors
    -   add a "why this was recommended" explanation
    -   compare a recommendation system and a classifier in the same file
    -   use the OpenAI API to explain ranked results in plain language
-   Add a diversity rule so repeated tag types do not dominate the results
-   Add a trust note after recommendations
-   Add a "needs human review" idea for sensitive use cases
-   Add a second system concept and compare the two

**Reflection / Takeaways:**
---------------------------

This lesson works best when Geniuses realize that AI systems do many different technical jobs. Some classify, some recommend, some rank, some generate, and some combine several behaviors at once. Day 5 helps tie Week 1 together by showing that understanding AI means understanding system behavior, data, risk, and responsibility together. By the end of the week, Geniuses should feel more confident identifying what kind of AI system they are looking at or imagining, and more prepared to explore deeper technical systems in the weeks ahead.

**Facilitator Notes**
---------------------

-   Keep using **Geniuses** consistently in examples and discussion.
-   Reinforce that recommendation and ranking systems are powerful because they shape user attention and choices.
-   Help Geniuses connect technical system behavior to real product experiences.
-   Use the Week 1 showcase to check whether Geniuses can now name and explain different AI system types.
-   Remind Geniuses that Week 2 will move into vision systems and how computers interpret images and scenes.

**Week 1 Wrap-Up**
------------------

By the end of Week 1, each Genius should have:

-   A named AI system concept
-   A clearly defined input and output
-   A learning setup such as supervised, unsupervised, or both
-   A system behavior such as classification, recommendation, ranking, detection, or generation
-   At least one identified risk
-   At least one responsible design choice
-   A first OpenAI-powered mini-tool
-   A stronger technical understanding of what makes AI systems work and why they must be built responsibly
