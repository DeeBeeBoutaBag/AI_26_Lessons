<img src="https://github.com/Hgp-GeniusLabs/Curriculum/blob/10734f2c827128dde773ea4f266d154d46977866/Org-Wide/Assets/hgp_logo_original.png" width="150"/>

Lesson Plan: AI Systems Week 3, Day 1 --- What Is Computer Vision? Images as Data and How AI Systems See
======================================================================================================

**Duration:**
-------------

3 hours

**Lesson Overview:**
--------------------

Week 3 introduces Geniuses to **computer vision systems**. After learning about foundational AI systems in Week 1 and generative systems in Week 2, Geniuses now focus on how AI systems work with visual information such as images and video. Day 1 introduces the big idea that images are not just pictures for humans. For an AI system, images are data. Vision systems process patterns in that data to classify, detect, track, and interpret what is happening visually.

This lesson helps Geniuses understand the foundations of vision AI, including how computer vision differs from text-based AI, what makes images useful input for AI systems, and why vision systems matter in areas like sports analytics, security, accessibility, healthcare, media, transportation, and retail. Geniuses also begin learning the difference between **image classification** and **object detection**, which will be expanded later in the week. During guided practice, the class builds a Python-based computer vision system planner that breaks down a visual AI system into inputs, tasks, outputs, and trust concerns. During independent practice, each Genius creates the first version of a vision-based AI software concept. By the end of the lesson, Geniuses should understand that computer vision is about turning images into usable information.

**Objectives:**
---------------

-   Define computer vision and explain how it fits into modern AI systems.
-   Explain how images can be treated as data by AI systems.
-   Distinguish between image classification and object detection at a foundational level.
-   Identify real-world use cases for vision AI in products and industries.
-   Build a Python-based vision system planner in VS Code.
-   Analyze trust, bias, and risk concerns in visual AI systems.
-   Begin the Week 3 mini-project by designing a computer vision software concept.

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
-   Optional example images or screenshots for discussion

**Standards:**
--------------

-   Computational Thinking: Analyze visual AI systems through inputs, tasks, outputs, and constraints.
-   Computer Science Practices: Explain how image-based systems process information differently from text-based systems.
-   Data Literacy: Recognize that images can function as structured input for AI systems.
-   Digital Literacy: Evaluate the opportunities and risks of AI systems that interpret the visual world.
-   Career Readiness: Practice technical reasoning, critique, and modern systems thinking.
-   Technical Foundations: Explain computer vision as a key branch of AI systems.

**Lesson Activity:**
--------------------

### 1. **Introduction (Time: 25 minutes)**

-   **Objective:** Energize Geniuses and introduce the idea that AI systems can learn from visual inputs like images and scenes.
-   Start with a fun icebreaker called **"What Can AI See?"**
-   This should be the first thing and the most fun thing to wake Geniuses up and get them ready for the lesson.

#### **Icebreaker Option A: Physical Movement**

-   Label different parts of the room:
    -   **Can Classify**
    -   **Can Detect**
    -   **Can Track**
    -   **Can Be Risky**
-   Read visual AI scenarios aloud and have Geniuses move to the category that best matches what the system is mainly doing.
-   Example prompts:
    -   A phone identifies whether a photo contains a dog
    -   A sports system finds every player on the field
    -   A camera follows a basketball through the air
    -   A face recognition system decides who someone is
    -   A smart app describes what is in front of a user
    -   A security camera flags unusual movement
-   After each round, ask:
    -   What is the system actually doing?
    -   Is it classifying one thing or detecting many things?
    -   Is it following motion over time?
    -   What could go wrong if it makes a mistake?

#### **Icebreaker Option B: Visual Product Breakdown**

-   Show or describe familiar products that use vision AI:
    -   face unlock
    -   sports highlight tools
    -   lane detection in vehicles
    -   object recognition in phones
    -   accessibility tools that describe scenes
-   Ask Geniuses:
    -   What is the input?
    -   What is the system trying to understand?
    -   What is the output?
-   Use this to introduce the idea that images are input data for AI systems.

#### **Transition**

-   Say:
    -   "Humans look at images and instantly understand a lot. AI systems have to process that same world through data, patterns, and models."
-   Ask:
    -   What makes vision harder than text?
    -   Why would visual AI be so useful in the real world?

### 2. **Direct Instruction (Time: 55 minutes)**

-   **Objective:** Help Geniuses understand the foundations of computer vision and why visual AI systems matter.
-   Use slides to guide instruction and keep it interactive.

#### **Suggested Slide Flow**

-   **Slide 1: What Is Computer Vision?**
    -   Computer vision is the branch of AI that helps systems interpret and reason about images and video
    -   It allows systems to identify, detect, track, and analyze visual information
-   **Slide 2: Images as Data**
    -   To humans, an image feels like a scene
    -   To a computer, an image is data made of pixels
    -   Vision systems learn patterns across colors, shapes, edges, textures, and spatial relationships
-   **Slide 3: Why Vision AI Matters**
    -   accessibility tools
    -   sports analytics
    -   object recognition
    -   quality control
    -   security systems
    -   navigation and transportation
    -   retail and inventory
    -   media and content tools
-   **Slide 4: Common Vision System Behaviors**
    -   image classification
    -   object detection
    -   tracking
    -   scene understanding
    -   segmentation
    -   event recognition
-   **Slide 5: Image Classification**
    -   One main decision about the image
    -   Example:
        -   this image contains a basketball court
        -   this image is a cat
    -   Best when the goal is broad image-level labeling
-   **Slide 6: Object Detection**
    -   Finds and labels multiple objects in the image
    -   Example:
        -   player
        -   ball
        -   hoop
        -   cone
    -   Best when the goal is location plus identity
-   **Slide 7: Why Vision Systems Are Challenging**
    -   lighting changes
    -   angle changes
    -   blurry images
    -   crowding
    -   occlusion
    -   motion
    -   low-quality input
    -   biased or incomplete training data
-   **Slide 8: Confidence and Mistakes**
    -   Vision systems often operate with uncertainty
    -   They may miss objects, confuse objects, or over-detect
    -   Confidence does not always equal correctness
-   **Slide 9: Responsible Vision AI**
    -   ask who is affected by mistakes
    -   think about fairness in recognition
    -   think about privacy and surveillance concerns
    -   consider whether human review is needed
    -   be careful with public-facing claims
-   **Slide 10: Week 3 Direction**
    -   Geniuses will move deeper into object detection, sports analytics, video analysis, and vision-based software concepts

#### **Discussion Questions**

-   What makes computer vision different from text AI?
-   Why are images harder to interpret than they may seem?
-   What kinds of products benefit most from visual AI?
-   What mistakes in computer vision could be especially harmful?
-   Why should visual AI systems be built carefully and transparently?

#### **Reflection Prompt**

-   Have Geniuses write for 4 minutes:
    -   "Think of one real problem that could be helped by a vision AI system. What would the system need to see, and what would it need to output?"

### 3. **Guided Practice (Time: 45 minutes)**

-   **Objective:** Help Geniuses build a Python-based computer vision system planner that breaks a visual AI idea into clear technical parts.
-   Explain that today's code-along is about understanding the structure of a vision system before building more advanced versions later.
-   The class will create `vision_system_planner.py`.

#### **Guided Practice Build**

Create a folder called `vision-system-planner`.

#### **Project Goal**

Build a Python program that:

-   asks the user for a vision AI app idea
-   asks what visual input the system uses
-   asks what the system is trying to do
-   asks what output it should produce
-   asks what risk or trust concern exists
-   prints a structured vision system summary

#### **Setup Steps**

1.  Open VS Code.
2.  Create a folder called `vision-system-planner`.
3.  Create a file called `vision_system_planner.py`.
4.  Run the file in the terminal.

#### **Sample Code**
```
# vision_system_planner.py
# AI Systems Week 3 Day 1
# This program helps Geniuses design a computer vision system concept.

print("Welcome to the Vision System Planner\n")

app_name = input("What is the name of your vision AI app? ")
visual_input = input("What visual input does it use? ")
task_type = input("What task does the system perform? (classification, detection, tracking, scene understanding, etc.) ")
output_type = input("What output does the system produce? ")
trust_concern = input("What is one trust or ethics concern? ")

print("\n--- Vision AI System Summary ---")
print(f"App Name: {app_name}")
print(f"Visual Input: {visual_input}")
print(f"Task Type: {task_type}")
print(f"Output Type: {output_type}")
print(f"Trust Concern: {trust_concern}")

print("\n--- Reflection ---")
print("What makes this a vision system?")
print("Why is visual input important here?")
print("What should a user still verify before trusting the output?")
```
#### **Guided Practice Teaching Points**

-   Why visual input should be described clearly
-   Why task type matters in vision system design
-   Why output should match the real user need
-   Why trust concerns must be considered early
-   Why planning a vision system helps before building more advanced logic

#### **Guided Practice Discussion**

-   What kinds of visual inputs make the most sense for real products?
-   Which task types felt easiest to define?
-   Which trust concerns showed up most often?
-   What part of a vision AI system is still hardest to imagine?

### 4. **Independent Practice (Time: 35 minutes)**

-   **Objective:** Geniuses independently create the first version of a vision-based AI software concept.
-   This begins the Week 3 mini-project.

#### **Mini-Project Title**

**Vision AI Software Concept --- Day 1 Foundation**

#### **Independent Task**

Each Genius creates a Python file for a vision AI system concept.

Examples:

-   sports shot tracker
-   smart inventory scanner
-   object detection assistant
-   scene description helper
-   AI retail shelf monitor
-   training form analyzer
-   game film clip organizer

Their concept must include:

-   system name
-   visual input type
-   task type
-   output type
-   one product use case
-   one trust or ethics concern
-   one responsible design choice

#### **Required Deliverables**

-   A working Python file called `my_vision_system.py`
-   A system concept with:
    -   system name
    -   visual input type
    -   task type
    -   output type
    -   product use case
    -   one trust concern
    -   one responsible design choice
-   A short written reflection:
    -   Why is this a computer vision system?
    -   What kind of visual data would it depend on?
    -   What makes it important to use responsibly?

#### **Independent Practice Starter Code**
```
# my_vision_system.py
# Week 3 Day 1 independent practice
# This program creates a vision AI system concept.

print("My Vision AI System\n")

system_name = "CourtTrack AI"
visual_input = "Video from basketball training sessions"
task_type = "Object detection and player tracking"
output_type = "Player movement zones and ball movement insights"
use_case = "Help coaches and players review spacing and movement"
trust_concern = "The system could miss key actions or track players incorrectly"
responsible_design = "The system should be used as a coaching support tool, not as the only source of performance judgment"

print(f"System Name: {system_name}")
print(f"Visual Input: {visual_input}")
print(f"Task Type: {task_type}")
print(f"Output Type: {output_type}")
print(f"Use Case: {use_case}")
print(f"Trust Concern: {trust_concern}")
print(f"Responsible Design Choice: {responsible_design}")
```
#### **Facilitator Support Moves**

-   Help Geniuses choose a realistic visual use case
-   Ask:
    -   What is the system looking at?
    -   Is it classifying the whole image or finding things within it?
    -   What would the user want to know?
    -   What happens if the system misses something important?
-   Encourage concepts that are modern, useful, and clearly visual

### 5. **Closure (Time: 20 minutes)**

-   **Objective:** Reinforce that computer vision systems turn images and video into information, but they also need trust, care, and clear design.
-   Bring the class together for a final share-out.
-   Ask 3--5 Geniuses to share:
    -   their system name
    -   what it looks at
    -   what task it performs
    -   one trust or ethics concern
-   Lead a closing discussion:
    -   What makes a vision AI system different from other AI systems?
    -   Why are images powerful but challenging inputs?
    -   What kinds of vision tools seem most exciting or most risky?
-   Preview the next lesson:
    -   Geniuses will go deeper into object detection and scene understanding and begin focusing on how systems find multiple things inside an image.

**Assessment:**
---------------

Student learning will be assessed through:

-   Participation in the icebreaker and discussion
-   Reflection responses during direct instruction
-   Completion of the guided Python vision system planner
-   Completion of an independent vision AI system concept
-   Final share-out and explanation of technical and responsible design choices

### **Exit Ticket**

1.  What is computer vision?
2.  What is one difference between image classification and object detection?
3.  What is one trust risk in computer vision systems?

**Extra Activities:**
---------------------

-   Geniuses who finish early can:
    -   add a second vision use case
    -   compare image classification vs object detection in their concept
    -   add a "why this output matters" section
    -   add a "who uses this system" field
    -   create a second version focused on accessibility or sports
    -   add a simple confidence note section
-   Add a "human review needed?" field
-   Add a "what the system should not be used for" section
-   Add a "what visual conditions make this harder?" section
-   Add a "future features" section

**Reflection / Takeaways:**
---------------------------

This lesson works best when Geniuses realize that visual AI systems are not just about recognizing pictures. They are about transforming visual input into useful information for real decisions, products, and workflows. Day 1 sets the tone for Week 3 by helping Geniuses understand that images are data, vision is a technical system behavior, and trust matters just as much in visual AI as it does in text or generative systems. By the end of the lesson, Geniuses should feel more confident thinking about what AI can see and what it should do with what it sees.

**Facilitator Notes**
---------------------

-   Keep using **Geniuses** consistently in examples and discussion.
-   Reinforce that computer vision is broader than just "image recognition."
-   Encourage product and software thinking, not just abstract model thinking.
-   Keep trust, privacy, and fairness visible throughout the lesson.
-   Remind Geniuses that tomorrow they will move deeper into object detection and scene understanding.

**Week 3 Day 1 Mini-Project Connection**
----------------------------------------

By the end of Day 1, each Genius should have:

-   A named vision AI system concept
-   A defined visual input type
-   A clear task type such as classification, detection, or tracking
-   A defined output
-   A real product use case
-   At least one identified trust or ethics concern
-   At least one responsible design choice
-   A stronger understanding of how computer vision systems turn images into information
