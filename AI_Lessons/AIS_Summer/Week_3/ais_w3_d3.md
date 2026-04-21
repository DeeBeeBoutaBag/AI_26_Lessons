<img src="https://github.com/Hgp-GeniusLabs/Curriculum/blob/10734f2c827128dde773ea4f266d154d46977866/Org-Wide/Assets/hgp_logo_original.png" width="150"/>

Lesson Plan: AI Systems Week 3, Day 3 --- Sports Analytics, Tracking Systems, and Visual Performance Intelligence
===============================================================================================================

**Duration:**
-------------

3 hours

**Lesson Overview:**
--------------------

On Day 3, Geniuses focus on one of the most exciting real-world uses of computer vision: **sports analytics**. After learning about computer vision foundations and object detection, Geniuses now explore how AI systems can detect, track, and analyze motion across sports footage. The lesson introduces the idea that sports analytics systems do more than find objects in a single image. They often follow players, track the ball, measure movement, identify patterns, and generate insights that can support coaches, athletes, media teams, and fans.

This lesson helps Geniuses understand that sports analytics is a strong AI software domain because it combines visual input, tracking, data interpretation, and real decision-making. Geniuses explore use cases such as player tracking, ball tracking, shot chart systems, movement zone analysis, highlight detection, and training support. During guided practice, the class builds a Python-based sports analytics workflow planner that breaks a system into visual input, tracked objects, tracked events, outputs, and trust concerns. During independent practice, each Genius designs a sports analytics AI system concept for a real use case. By the end of the lesson, Geniuses should understand that sports analytics is a vision AI field where detection becomes movement intelligence.

**Objectives:**
---------------

-   Explain how sports analytics systems build on object detection and tracking.
-   Identify common AI tasks in sports analytics such as player tracking, ball tracking, event detection, and performance analysis.
-   Distinguish between single-frame detection and multi-frame tracking across time.
-   Analyze how sports analytics systems can support athletes, coaches, trainers, and media workflows.
-   Build a Python-based sports analytics workflow planner in VS Code.
-   Reflect on trust, bias, fairness, and overreliance concerns in sports AI systems.
-   Continue the Week 3 mini-project by designing a sports analytics AI software concept.

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
-   Existing Week 3 files
-   Starter folder for Python files
-   Optional sports images, screenshots, or game clips for discussion

**Standards:**
--------------

-   Computational Thinking: Analyze how AI systems track objects and events across time.
-   Computer Science Practices: Design and explain a sports analytics workflow using computer vision concepts.
-   Data Literacy: Interpret how movement, position, and tracking data can turn into insight.
-   Digital Literacy: Evaluate the usefulness and risks of AI systems used in sports decision-making.
-   Career Readiness: Practice technical explanation, critique, and modern product thinking.
-   Technical Foundations: Explain sports analytics as a computer vision system domain built on detection, tracking, and analysis.

**Lesson Activity:**
--------------------

### 1. **Introduction (Time: 25 minutes)**

-   **Objective:** Energize Geniuses and introduce the idea that AI can analyze sports visually by detecting and following movement over time.
-   Start with a fun icebreaker called **"What Would the AI Track?"**
-   This should be the first thing and the most fun thing to wake Geniuses up and get them ready for the lesson.

#### **Icebreaker Option A: Physical Movement**

-   Label different parts of the room:
    -   **Player**
    -   **Ball**
    -   **Event**
    -   **Zone**
-   Read sports situations aloud and have Geniuses move to what they think the AI system would most need to track.
-   Example prompts:
    -   A basketball coach wants to understand spacing on offense
    -   A soccer system wants to detect when a shot happens
    -   A trainer wants to study sprint patterns in practice
    -   A media team wants to auto-generate game highlights
    -   A baseball tool wants to follow the pitch path
    -   A football analyst wants to map player movement zones
-   After each round, ask:
    -   What is the system actually following?
    -   Does it need one frame or many frames?
    -   Is it tracking an object, a player, an event, or a pattern?
    -   What could go wrong if the system misses something important?

#### **Icebreaker Option B: Sports AI Brainstorm**

-   Ask Geniuses to list sports they know well.
-   For each sport, ask:
    -   what objects matter
    -   what movement matters
    -   what a coach or athlete might want to know
-   Use this to connect sports knowledge to AI systems thinking.

#### **Transition**

-   Say:
    -   "Sports analytics is one of the best examples of vision AI because it turns motion and position into insight."
-   Ask:
    -   What is the difference between detecting a player once and tracking that player over time?
    -   Why would coaches, athletes, and teams want AI-generated visual insight?

### 2. **Direct Instruction (Time: 55 minutes)**

-   **Objective:** Help Geniuses understand how sports analytics systems work and why tracking and event detection matter.
-   Use slides to guide instruction and keep it interactive.

#### **Suggested Slide Flow**

-   **Slide 1: What Is Sports Analytics in AI?**
    -   Sports analytics uses data and AI to analyze performance, movement, events, and strategy
    -   Vision AI makes this possible directly from image and video input
-   **Slide 2: Sports Analytics as a Vision System**
    -   Input:
        -   game footage
        -   practice video
        -   camera feeds
    -   System behaviors:
        -   detect players
        -   detect ball
        -   track positions
        -   recognize events
        -   produce insights
-   **Slide 3: Detection vs Tracking**
    -   Detection:
        -   find the object now
    -   Tracking:
        -   follow the object across time
    -   Tracking matters when movement and sequence are important
-   **Slide 4: Common Sports Vision Tasks**
    -   player tracking
    -   ball tracking
    -   shot detection
    -   sprint tracking
    -   movement zone analysis
    -   formation analysis
    -   highlight detection
    -   event recognition
-   **Slide 5: What Outputs Can Sports AI Produce?**
    -   heat maps
    -   movement trails
    -   event counts
    -   shot charts
    -   highlight clips
    -   player positioning insights
    -   training feedback
-   **Slide 6: Real Product Use Cases**
    -   coaching support
    -   player development
    -   recruiting analysis
    -   broadcast enhancement
    -   fan engagement
    -   injury prevention support
    -   training review
-   **Slide 7: Why Sports Analytics Is Hard**
    -   fast movement
    -   camera shake
    -   overlapping players
    -   small ball size
    -   occlusion
    -   inconsistent video angles
    -   different sports environments
-   **Slide 8: Trust and Fairness in Sports AI**
    -   missed events
    -   inaccurate tracking
    -   weak camera coverage
    -   overreliance on system outputs
    -   unfair judgment from incomplete data
    -   using AI support as if it were final truth
-   **Slide 9: Responsible Sports AI Design**
    -   use AI as support, not absolute judgment
    -   show uncertainty when possible
    -   understand camera limitations
    -   avoid reducing athletes to only one metric
    -   keep human coaching context involved
-   **Slide 10: Week 3 Direction**
    -   Geniuses will next move into video vision, frame sequences, and real-time visual analysis systems

#### **Discussion Questions**

-   Why is sports analytics a strong use case for computer vision?
-   What is the difference between player tracking and event detection?
-   Why is a ball often harder to track than a player?
-   What risks come from overtrusting sports AI outputs?
-   What makes sports AI useful without letting it become unfair?

#### **Reflection Prompt**

-   Have Geniuses write for 4 minutes:
    -   "Choose a sport you know. What would a useful AI system track, and what insight would it give?"

### 3. **Guided Practice (Time: 45 minutes)**

-   **Objective:** Help Geniuses build a Python-based sports analytics workflow planner that organizes a sports vision system into inputs, tracked objects, events, outputs, and trust concerns.
-   Explain that today's code-along is about planning a sports AI system clearly.
-   The class will create `sports_analytics_planner.py`.

#### **Guided Practice Build**

Create a folder called `sports-analytics-planner`.

#### **Project Goal**

Build a Python program that:

-   asks the user for a sport
-   asks what should be tracked
-   asks what event or pattern matters
-   asks what output should be produced
-   asks what trust concern exists
-   prints a structured sports analytics system summary

#### **Setup Steps**

1.  Open VS Code.
2.  Create a folder called `sports-analytics-planner`.
3.  Create a file called `sports_analytics_planner.py`.
4.  Run the file in the terminal.

#### **Sample Code**
```
# sports_analytics_planner.py
# AI Systems Week 3 Day 3
# This program helps Geniuses plan a sports analytics AI system.

print("Welcome to the Sports Analytics Planner\n")

system_name = input("What is the name of your sports analytics system? ")
sport = input("What sport does the system focus on? ")
tracked_items = input("What should the system track? ")
important_event = input("What event or pattern matters most? ")
output_type = input("What output should the system produce? ")
trust_concern = input("What is one trust or fairness concern? ")

print("\n--- Sports Analytics System Summary ---")
print(f"System Name: {system_name}")
print(f"Sport: {sport}")
print(f"Tracked Items: {tracked_items}")
print(f"Important Event or Pattern: {important_event}")
print(f"Output Type: {output_type}")
print(f"Trust Concern: {trust_concern}")

print("\n--- Reflection ---")
print("Does this system need detection, tracking, or both?")
print("What kind of video conditions could make this harder?")
print("How should humans still stay involved in interpreting the results?")
```
#### **Optional Extension**

Add a simple frame-sequence style planning output:
```
# optional_tracking_steps.py
# This demonstrates how a sports AI system might think across time.

tracking_steps = [
    "Frame 1: Detect players and ball",
    "Frame 2: Match player positions to previous frame",
    "Frame 3: Update movement paths",
    "Frame 4: Detect event pattern such as shot attempt or sprint burst",
    "Frame 5: Save insight for coach review"
]

print("\n--- Example Tracking Workflow ---")
for step in tracking_steps:
    print(step)
```
#### **Guided Practice Teaching Points**

-   Why sports analytics depends on both detection and tracking
-   Why event recognition often requires multiple frames
-   Why outputs should connect directly to a coach, athlete, or analyst need
-   Why trust concerns should be included in system planning
-   Why sports AI should support insight, not replace all human interpretation

#### **Guided Practice Discussion**

-   Which tracked items seem most important in different sports?
-   What kinds of outputs would be most useful to a coach?
-   What conditions would make the system weaker?
-   Why might a highlight system need different logic than a training system?

### 4. **Independent Practice (Time: 35 minutes)**

-   **Objective:** Geniuses independently design a sports analytics AI system concept for a real use case.
-   This continues the Week 3 mini-project.

#### **Mini-Project Title**

**Vision AI Software Concept --- Day 3 Sports Analytics Design**

#### **Independent Task**

Each Genius creates a Python file for a sports analytics AI software concept.

Examples:

-   basketball spacing tracker
-   soccer shot event detector
-   sprint training analyzer
-   football route tracker
-   tennis ball path analyzer
-   highlight clip generator
-   player movement heat map system

Their concept must include:

-   system name
-   sport
-   tracked items
-   important event or pattern
-   output type
-   one trust or fairness concern
-   one responsible design choice

#### **Required Deliverables**

-   A working Python file called `my_sports_ai_system.py`
-   A system concept with:
    -   system name
    -   sport
    -   tracked items
    -   important event or pattern
    -   output type
    -   one trust or fairness concern
    -   one responsible design choice
-   A short written reflection:
    -   Why is vision AI the right system type here?
    -   What makes this sport hard to analyze visually?
    -   What should humans still interpret instead of relying on the AI completely?

#### **Independent Practice Starter Code**
```
# my_sports_ai_system.py
# Week 3 Day 3 independent practice
# This program creates a sports analytics AI system concept.

print("My Sports Analytics AI System\n")

system_name = "HoopFlow AI"
sport = "Basketball"
tracked_items = "Players, ball, and court position zones"
important_event = "Offensive spacing and shot creation sequences"
output_type = "Movement heat maps and coaching insight summaries"
trust_concern = "The system could overvalue visible movement patterns while missing game context and decision-making"
responsible_design = "The system should support coaching review and film study, not act as the final judgment on player value"

print(f"System Name: {system_name}")
print(f"Sport: {sport}")
print(f"Tracked Items: {tracked_items}")
print(f"Important Event or Pattern: {important_event}")
print(f"Output Type: {output_type}")
print(f"Trust Concern: {trust_concern}")
print(f"Responsible Design Choice: {responsible_design}")
```
#### **Facilitator Support Moves**

-   Help Geniuses pick a realistic sports use case
-   Ask:
    -   What does the user most want to learn?
    -   What objects or movement matter most?
    -   What would the AI struggle to see?
    -   What should remain a coach or athlete decision?
-   Encourage sports concepts that feel useful, specific, and fair

### 5. **Closure (Time: 20 minutes)**

-   **Objective:** Reinforce that sports analytics is a powerful vision AI domain built on movement, tracking, and insight.
-   Bring the class together for a final share-out.
-   Ask 3--5 Geniuses to share:
    -   their system name
    -   the sport they focused on
    -   what the system tracks
    -   one trust or fairness concern
-   Lead a closing discussion:
    -   Why is sports analytics more than just object detection?
    -   What makes tracking across time important?
    -   Why should sports AI support human judgment instead of replacing it?
-   Preview the next lesson:
    -   Geniuses will move into video vision systems, frame-by-frame analysis, and real-time visual workflows.

**Assessment:**
---------------

Student learning will be assessed through:

-   Participation in the icebreaker and discussion
-   Reflection responses during direct instruction
-   Completion of the guided Python sports analytics planner
-   Completion of an independent sports analytics AI system concept
-   Final share-out and explanation of tracking choices and trust concerns

### **Exit Ticket**

1.  What is one difference between detection and tracking?
2.  What is one useful output from a sports analytics AI system?
3.  What is one trust or fairness concern in sports AI?

**Extra Activities:**
---------------------

-   Geniuses who finish early can:
    -   add a frame-by-frame tracking plan
    -   create a second sports use case and compare it
    -   add a "what makes this hard to detect?" section
    -   add a "coach dashboard" idea
    -   add a "highlight generation" mode
    -   add a "what should not be automated?" note
-   Add a "camera angle limitation" field
-   Add a "best user for this tool" field
-   Add a "what metric could be misleading?" section
-   Add a "future feature" section for live analysis

**Reflection / Takeaways:**
---------------------------

This lesson works best when Geniuses realize that sports analytics is one of the clearest examples of AI systems turning vision into insight. Day 3 helps them connect object detection, tracking, movement, and user value in one real-world domain. By the end of the lesson, Geniuses should feel more confident explaining how sports AI systems work and more aware that performance data should be used carefully, fairly, and in support of human judgment.

**Facilitator Notes**
---------------------

-   Keep using **Geniuses** consistently in examples and discussion.
-   Reinforce that sports analytics systems often require both visual intelligence and contextual human interpretation.
-   Encourage product thinking by asking who the tool helps and what decision it supports.
-   Keep fairness and overreliance concerns visible.
-   Remind Geniuses that tomorrow they will move into video vision, real-time analysis, and frame-based system workflows.

**Week 3 Day 3 Mini-Project Connection**
----------------------------------------

By the end of Day 3, each Genius should have:

-   A named sports analytics AI system concept
-   A defined sport and use case
-   A clear list of tracked items
-   An important event or pattern to analyze
-   A useful output type
-   At least one trust or fairness concern
-   At least one responsible design choice
-   A stronger understanding of tracking and analytics as a vision AI workflow
