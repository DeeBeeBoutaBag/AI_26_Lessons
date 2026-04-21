<img src="https://github.com/Hgp-GeniusLabs/Curriculum/blob/10734f2c827128dde773ea4f266d154d46977866/Org-Wide/Assets/hgp_logo_original.png" width="150"/>

Lesson Plan: AI Systems Week 3, Day 4 --- Video Vision Systems, Frame-by-Frame Analysis, and Real-Time AI Workflows
=================================================================================================================

**Duration:**
-------------

3 hours

**Lesson Overview:**
--------------------

On Day 4, Geniuses expand from still-image vision systems and sports tracking into **video vision systems**. After learning about computer vision, object detection, and sports analytics, Geniuses now focus on what changes when AI systems must interpret **many frames across time** instead of one image at a time. This lesson introduces the idea that video is not just a moving picture. For an AI system, video is a sequence of frames, events, and motion patterns that must be processed over time.

Geniuses explore how video AI systems support use cases like sports replay analysis, highlight generation, security review, training breakdowns, traffic systems, event detection, and real-time monitoring. They also examine why video vision is harder than image vision, including speed, motion blur, changing camera angles, longer sequences, and the difficulty of maintaining consistency across frames. During guided practice, the class builds a Python-based video vision workflow planner that organizes a system into frames, tracked targets, event logic, outputs, and trust concerns. During independent practice, each Genius creates a video-based AI software concept for a real use case. By the end of the lesson, Geniuses should understand that video vision systems are about detection plus time plus interpretation.

**Objectives:**
---------------

-   Explain how video vision systems differ from still-image vision systems.
-   Define frame-by-frame analysis and describe why time matters in video AI.
-   Identify common real-world use cases for video vision systems.
-   Explain how tracking, event detection, and sequence understanding work together in video AI.
-   Build a Python-based video vision workflow planner in VS Code.
-   Reflect on speed, accuracy, fairness, and trust in video AI systems.
-   Continue the Week 3 mini-project by designing a video vision AI software concept.

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
-   Optional short sports clips, security clips, or movement-based examples for discussion

**Standards:**
--------------

-   Computational Thinking: Analyze how systems process sequences of frames and events across time.
-   Computer Science Practices: Design and explain a video-based vision AI workflow.
-   Data Literacy: Interpret how motion, sequence, and time add complexity to visual data.
-   Digital Literacy: Evaluate the usefulness and risks of systems that analyze video over time.
-   Career Readiness: Practice technical explanation, critique, and system design thinking.
-   Technical Foundations: Explain video vision as a time-based extension of object detection and tracking.

**Lesson Activity:**
--------------------

### 1. **Introduction (Time: 25 minutes)**

-   **Objective:** Energize Geniuses and introduce the idea that video AI systems must understand not just what is in a scene, but what changes over time.
-   Start with a fun icebreaker called **"One Frame or Many Frames?"**
-   This should be the first thing and the most fun thing to wake Geniuses up and get them ready for the lesson.

#### **Icebreaker Option A: Physical Movement**

-   Label one side of the room **"One Frame Is Enough"** and the other side **"Need Video Over Time."**
-   Read scenarios aloud and have Geniuses move to the side they think fits best.
-   Example prompts:
    -   Detect whether a basketball is visible in an image
    -   Detect whether a shot attempt happened
    -   Identify whether a traffic light is red in one frame
    -   Detect whether a car ran a red light
    -   Identify that a runner is on the track
    -   Analyze sprint form over several seconds
    -   Detect a person in a doorway
    -   Detect whether unusual behavior happened in a hallway
-   After each round, ask:
    -   Why is one frame enough or not enough?
    -   What extra information comes from time?
    -   What event or motion is the system trying to understand?
    -   What could go wrong if the system only looked at one image?

#### **Icebreaker Option B: Event Breakdown**

-   Put events on the board:
    -   shot attempt
    -   fall detection
    -   pass completion
    -   sprint acceleration
    -   someone entering a room
-   Ask Geniuses:
    -   can this be understood from one frame?
    -   or does it need a sequence?
-   Discuss how events are often patterns across time, not single still moments.

#### **Transition**

-   Say:
    -   "A still image can tell a system what is there. A video can tell a system what happened."
-   Ask:
    -   Why does time matter so much in AI?
    -   What kinds of software products depend on events, motion, and sequences?

### 2. **Direct Instruction (Time: 55 minutes)**

-   **Objective:** Help Geniuses understand how video vision systems work and why frame sequences make AI more powerful and more difficult.
-   Use slides to guide instruction and keep it interactive.

#### **Suggested Slide Flow**

-   **Slide 1: What Is a Video Vision System?**
    -   A video vision system analyzes a sequence of frames over time
    -   It can detect objects, track movement, recognize events, and generate time-based insight
-   **Slide 2: Image Vision vs Video Vision**
    -   **Image vision:** one frame, one moment
    -   **Video vision:** many frames, motion, timing, sequence
    -   Video systems often combine:
        -   detection
        -   tracking
        -   event recognition
-   **Slide 3: What Is a Frame?**
    -   A video is made of many frames shown in sequence
    -   AI systems may analyze each frame and then connect patterns across frames
-   **Slide 4: What Video Vision Systems Can Do**
    -   track objects across time
    -   detect actions or events
    -   identify movement patterns
    -   summarize sequences
    -   trigger alerts
    -   support replay or performance review
-   **Slide 5: Real-World Video Vision Use Cases**
    -   sports analytics
    -   security and safety monitoring
    -   traffic analysis
    -   training and technique review
    -   warehouse or logistics monitoring
    -   content highlight generation
    -   accessibility tools
-   **Slide 6: Why Video Vision Is Hard**
    -   fast movement
    -   changing camera angles
    -   motion blur
    -   missing frames
    -   object overlap
    -   long sequences
    -   real-time speed requirements
-   **Slide 7: Event Detection**
    -   Some systems are not just tracking objects
    -   They are detecting events such as:
        -   shot made
        -   fall occurred
        -   car changed lanes
        -   player entered zone
        -   person crossed boundary
-   **Slide 8: Real-Time vs Delayed Analysis**
    -   **Real-time:** fast decisions while video is happening
    -   **Delayed analysis:** review later for deeper insight
    -   These have different tradeoffs in speed, quality, and use case
-   **Slide 9: Trust and Risk in Video Systems**
    -   missed events
    -   false alerts
    -   privacy concerns
    -   over-surveillance
    -   unfair interpretation
    -   overtrusting automated event detection
-   **Slide 10: Week 3 Direction**
    -   Geniuses will use tomorrow's studio day to refine and showcase a vision-based AI software concept using image, detection, tracking, or video workflows

#### **Discussion Questions**

-   Why is video AI harder than image AI?
-   What is the difference between tracking and event detection?
-   When is real-time analysis necessary?
-   What are the risks of false alerts in video systems?
-   Why should video AI systems be used carefully in public-facing or high-stakes settings?

#### **Reflection Prompt**

-   Have Geniuses write for 4 minutes:
    -   "Describe one real use case where a system would need to analyze motion or events over time, not just one image."

### 3. **Guided Practice (Time: 45 minutes)**

-   **Objective:** Help Geniuses build a Python-based video vision workflow planner that structures a time-based AI system.
-   Explain that today's code-along is about organizing a sequence-based vision workflow clearly.
-   The class will create `video_vision_planner.py`.

#### **Guided Practice Build**

Create a folder called `video-vision-planner`.

#### **Project Goal**

Build a Python program that:

-   asks the user for a video AI app idea
-   asks what the system tracks across frames
-   asks what event or sequence matters
-   asks what output the system should produce
-   asks what trust concern exists
-   prints a structured video vision system summary

#### **Setup Steps**

1.  Open VS Code.
2.  Create a folder called `video-vision-planner`.
3.  Create a file called `video_vision_planner.py`.
4.  Run the file in the terminal.

#### **Sample Code**
```
# video_vision_planner.py
# AI Systems Week 3 Day 4
# This program helps Geniuses design a video vision AI workflow.

print("Welcome to the Video Vision Planner\n")

system_name = input("What is the name of your video vision system? ")
video_input = input("What kind of video input does the system analyze? ")
tracked_targets = input("What does the system track across frames? ")
important_event = input("What event or sequence is the system trying to detect? ")
output_type = input("What output should the system produce? ")
trust_concern = input("What is one trust or ethics concern? ")

print("\n--- Video Vision System Summary ---")
print(f"System Name: {system_name}")
print(f"Video Input: {video_input}")
print(f"Tracked Targets: {tracked_targets}")
print(f"Important Event or Sequence: {important_event}")
print(f"Output Type: {output_type}")
print(f"Trust Concern: {trust_concern}")

print("\n--- Reflection ---")
print("Why does this system need video instead of only images?")
print("What happens across time that matters here?")
print("What should a human still review before acting on the output?")
```
#### **Optional Extension**

Add a simple frame workflow simulation:
```
# optional_frame_workflow.py
# This demonstrates a simple frame-by-frame video analysis plan.

workflow_steps = [
    "Frame 1: Detect all important objects",
    "Frame 2: Match detected objects to previous positions",
    "Frame 3: Update movement paths",
    "Frame 4: Check whether an event pattern is happening",
    "Frame 5: Save or report the event for review"
]

print("\n--- Example Video Analysis Workflow ---")
for step in workflow_steps:
    print(step)
```
#### **Guided Practice Teaching Points**

-   Why video systems need frame-by-frame logic
-   Why tracking and event recognition are linked
-   Why sequence understanding adds product value
-   Why real-time systems have stricter constraints
-   Why video workflows need caution and review

#### **Guided Practice Discussion**

-   What kinds of events truly require video?
-   Which parts of a video workflow feel hardest?
-   What would be most useful as an output?
-   What types of mistakes would be most harmful in these systems?

### 4. **Independent Practice (Time: 35 minutes)**

-   **Objective:** Geniuses independently create a video-based AI software concept for a real use case.
-   This continues the Week 3 mini-project.

#### **Mini-Project Title**

**Vision AI Software Concept --- Day 4 Video Vision Design**

#### **Independent Task**

Each Genius creates a Python file for a video vision AI system concept.

Examples:

-   highlight clip detector
-   fall detection system
-   sprint form analyzer
-   traffic event detector
-   practice drill tracker
-   unusual movement alert system
-   player movement sequence analyzer

Their concept must include:

-   system name
-   video input type
-   tracked targets
-   one important event or sequence
-   output type
-   one trust or ethics concern
-   one responsible design choice

#### **Required Deliverables**

-   A working Python file called `my_video_vision_system.py`
-   A system concept with:
    -   system name
    -   video input type
    -   tracked targets
    -   important event or sequence
    -   output type
    -   one trust or ethics concern
    -   one responsible design choice
-   A short written reflection:
    -   Why does this use case require video?
    -   What makes the event or sequence hard to detect?
    -   What should humans still interpret themselves?

#### **Independent Practice Starter Code**
```
# my_video_vision_system.py
# Week 3 Day 4 independent practice
# This program creates a video vision AI system concept.

print("My Video Vision AI System\n")

system_name = "SprintSense AI"
video_input = "Practice footage of athletes running sprint drills"
tracked_targets = "Athlete body position and movement across frames"
important_event = "Acceleration phase and form changes during the sprint"
output_type = "Technique flags and movement summary for coach review"
trust_concern = "The system could misread movement because of camera angle or video quality"
responsible_design = "The output should support coaching feedback, not replace expert instruction or athlete context"

print(f"System Name: {system_name}")
print(f"Video Input: {video_input}")
print(f"Tracked Targets: {tracked_targets}")
print(f"Important Event or Sequence: {important_event}")
print(f"Output Type: {output_type}")
print(f"Trust Concern: {trust_concern}")
print(f"Responsible Design Choice: {responsible_design}")
```
#### **Facilitator Support Moves**

-   Help Geniuses choose use cases where time actually matters
-   Ask:
    -   What happens across frames that one image cannot show?
    -   What event is the system trying to recognize?
    -   What would make detection harder in real video?
    -   What should still be reviewed by a coach, teacher, analyst, or human expert?
-   Encourage concepts that are specific, useful, and realistic

### 5. **Closure (Time: 20 minutes)**

-   **Objective:** Reinforce that video vision systems turn sequences and motion into usable insight, but they require strong design and careful trust thinking.
-   Bring the class together for a final share-out.
-   Ask 3--5 Geniuses to share:
    -   their system name
    -   what kind of video it analyzes
    -   what event or sequence it looks for
    -   one trust or ethics concern
-   Lead a closing discussion:
    -   Why does time matter in AI systems?
    -   What is the difference between object detection and event detection?
    -   What kinds of video vision systems feel most useful or most risky?
-   Preview the next lesson:
    -   Geniuses will use studio day to refine and showcase a vision AI software concept from the week.

**Assessment:**
---------------

Student learning will be assessed through:

-   Participation in the icebreaker and discussion
-   Reflection responses during direct instruction
-   Completion of the guided Python video vision planner
-   Completion of an independent video-based vision concept
-   Final share-out and explanation of sequence logic and trust choices

### **Exit Ticket**

1.  What is a video vision system?
2.  Why is video harder than still-image analysis?
3.  What is one trust risk in video AI systems?

**Extra Activities:**
---------------------

-   Geniuses who finish early can:
    -   add a real-time vs delayed-analysis choice
    -   create a second use case and compare it
    -   add a "hardest frame condition" section
    -   add an event confidence note
    -   build a simple frame sequence list for their system
    -   add a "why human review matters" section
-   Add a "camera angle limitation" field
-   Add a "what false alert would look like" section
-   Add a "what missed event would look like" section
-   Add a "future feature" section

**Reflection / Takeaways:**
---------------------------

This lesson works best when Geniuses realize that video AI systems are not simply image systems repeated many times. They are time-based systems that must interpret movement, sequence, and events. Day 4 helps Geniuses connect frame-by-frame processing to real software ideas and real-world use cases. By the end of the lesson, Geniuses should feel more confident explaining why video matters in AI and more aware that time-based systems bring both powerful possibilities and serious design challenges.

**Facilitator Notes**
---------------------

-   Keep using **Geniuses** consistently in examples and discussion.
-   Reinforce that video systems are sequence systems, not just image systems.
-   Encourage realistic use cases where time and events truly matter.
-   Keep trust, privacy, surveillance, and human review visible throughout the lesson.
-   Remind Geniuses that tomorrow they will refine and showcase the strongest vision AI software concepts from the week.

**Week 3 Day 4 Mini-Project Connection**
----------------------------------------

By the end of Day 4, each Genius should have:

-   A named video vision AI system concept
-   A defined video input type
-   Clear tracked targets
-   A meaningful event or sequence to detect
-   A useful output type
-   At least one trust or ethics concern
-   At least one responsible design choice
-   A stronger understanding of how video AI systems use time, motion, and sequence to create insight
