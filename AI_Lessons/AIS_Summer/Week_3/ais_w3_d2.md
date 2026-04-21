<img src="https://github.com/Hgp-GeniusLabs/Curriculum/blob/10734f2c827128dde773ea4f266d154d46977866/Org-Wide/Assets/hgp_logo_original.png" width="150"/>

Lesson Plan: AI Systems Week 3, Day 2 --- Object Detection, Bounding Boxes, and Scene Understanding
=================================================================================================

**Duration:**
-------------

3 hours

**Lesson Overview:**
--------------------

On Day 2, Geniuses go deeper into one of the most important and recognizable computer vision tasks: **object detection**. After being introduced to computer vision on Day 1, Geniuses now focus on how AI systems move beyond labeling an entire image and instead identify **multiple objects inside the same scene**. This lesson introduces the idea that a vision system can not only say what is in an image, but also point to where each object is and give a confidence-based prediction.

Geniuses learn about **bounding boxes**, scene complexity, multi-object environments, and how object detection systems are used in sports analytics, security tools, accessibility technology, retail systems, autonomous navigation, and training feedback software. They also examine where object detection systems fail, including low lighting, overlapping objects, motion blur, small objects, biased training data, and false confidence. During guided practice, the class builds a Python-based object detection planner that simulates how a system might describe detected objects and organize scene information. During independent practice, each Genius designs an object detection AI software concept for a real use case and explains its risks and responsible design needs. By the end of the lesson, Geniuses should understand that object detection is one of the key building blocks of modern vision AI.

**Objectives:**
---------------

-   Define object detection and explain how it differs from image classification.
-   Explain what bounding boxes are and why they matter in visual AI systems.
-   Identify real-world product use cases for object detection.
-   Analyze how object detection systems perform in complex scenes with multiple objects.
-   Build a Python-based object detection planner in VS Code.
-   Reflect on confidence, missed detections, false detections, and fairness in object detection systems.
-   Continue the Week 3 mini-project by designing an object detection-based AI software concept.

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
-   Existing Week 3 Day 1 files
-   Starter folder for Python files
-   Optional example images with multiple visible objects

**Standards:**
--------------

-   Computational Thinking: Analyze how AI systems identify and locate multiple objects in a scene.
-   Computer Science Practices: Design and explain a vision system that detects, labels, and describes objects.
-   Data Literacy: Interpret how scene complexity affects the quality of visual AI output.
-   Digital Literacy: Evaluate trust, fairness, and failure cases in object detection systems.
-   Career Readiness: Practice technical explanation, critique, and modern systems thinking.
-   Technical Foundations: Explain object detection as a major computer vision system behavior.

**Lesson Activity:**
--------------------

### 1. **Introduction (Time: 25 minutes)**

-   **Objective:** Energize Geniuses and introduce the idea that AI can find and label multiple things inside a single image or scene.
-   Start with a fun icebreaker called **"One Thing or Many Things?"**
-   This should be the first thing and the most fun thing to wake Geniuses up and get them ready for the lesson.

#### **Icebreaker Option A: Physical Movement**

-   Label one side of the room **"Classification"** and the other side **"Detection."**
-   Read image-based scenarios aloud and have Geniuses move to the side that best matches what the AI system needs to do.
-   Example prompts:
    -   Decide whether an image contains a basketball court
    -   Find every player and the ball in a game photo
    -   Decide whether a picture is mostly a dog or a cat
    -   Find all traffic signs in a street image
    -   Decide whether a photo is indoor or outdoor
    -   Find every product on a shelf
-   After each round, ask:
    -   Is the system labeling the whole image or finding multiple things?
    -   Why would detection be more useful here?
    -   What makes some scenes harder than others?
    -   What happens if the system misses an important object?

#### **Icebreaker Option B: Scene Breakdown**

-   Describe or show scenes with multiple objects:
    -   a basketball court
    -   a busy classroom
    -   a street crossing
    -   a store shelf
-   Ask Geniuses:
    -   what objects a system might need to detect
    -   which objects matter most
    -   which objects would be hardest to detect
-   Use this to introduce scene complexity and multi-object vision tasks.

#### **Transition**

-   Say:
    -   "Yesterday Geniuses learned that computer vision can interpret images. Today we go deeper into how systems detect many things in the same visual scene."
-   Ask:
    -   Why is finding many objects harder than labeling one whole image?
    -   Why would detection matter in sports, safety, accessibility, or retail?

### 2. **Direct Instruction (Time: 55 minutes)**

-   **Objective:** Help Geniuses understand object detection, bounding boxes, scene understanding, and failure cases in visual AI.
-   Use slides to guide instruction and keep it interactive.

#### **Suggested Slide Flow**

-   **Slide 1: What Is Object Detection?**
    -   Object detection means identifying what objects are present and where they are located in an image
    -   It answers:
        -   what is here?
        -   where is it?
-   **Slide 2: Classification vs Detection**
    -   **Classification:** one label for the image
    -   **Detection:** multiple labels plus locations
    -   Example:
        -   classification: "basketball game"
        -   detection: "player here, ball here, hoop here"
-   **Slide 3: What Is a Bounding Box?**
    -   A bounding box is a rectangle around a detected object
    -   It helps the system mark where the object is located
    -   It is one of the simplest and most common ways to represent detected objects
-   **Slide 4: What Object Detection Systems Output**
    -   object label
    -   location
    -   sometimes confidence score
    -   sometimes multiple objects at once
-   **Slide 5: Real-World Object Detection Use Cases**
    -   sports analytics
    -   retail inventory systems
    -   autonomous navigation
    -   accessibility tools
    -   safety and security systems
    -   manufacturing and quality control
-   **Slide 6: Scene Complexity**
    -   crowded scenes
    -   overlapping objects
    -   motion blur
    -   small objects
    -   low light
    -   strange angles
    -   These all make detection harder
-   **Slide 7: Confidence and Errors**
    -   false positives:
        -   system thinks something is there when it is not
    -   false negatives:
        -   system misses something that is there
    -   confidence does not guarantee correctness
-   **Slide 8: Object Detection in Sports Analytics**
    -   detect players
    -   detect ball
    -   track movement zones
    -   identify events
    -   generate performance insights
-   **Slide 9: Responsible Object Detection**
    -   who is affected if the system misses something?
    -   what happens if a person or object is misidentified?
    -   how does bias in visual data affect results?
    -   when is human review necessary?
-   **Slide 10: Week 3 Direction**
    -   Geniuses will soon move into motion tracking, sports analytics, and video-based vision systems

#### **Discussion Questions**

-   Why is object detection different from image classification?
-   What does a bounding box actually help the system do?
-   What kinds of scenes are hardest for detection systems?
-   Why are false positives and false negatives both important?
-   What trust issues matter most in object detection systems?

#### **Reflection Prompt**

-   Have Geniuses write for 4 minutes:
    -   "Think of one object detection system that could be useful in the real world. What must it detect, and what happens if it misses something important?"

### 3. **Guided Practice (Time: 45 minutes)**

-   **Objective:** Help Geniuses build a Python-based object detection planner that organizes scene information, detected objects, and trust concerns.
-   Explain that today's code-along is about simulating how an object detection system might describe a scene and its detection goals.
-   The class will create `object_detection_planner.py`.

#### **Guided Practice Build**

Create a folder called `object-detection-planner`.

#### **Project Goal**

Build a Python program that:

-   asks the user for a scene
-   asks what objects need to be detected
-   asks why the detection matters
-   asks what could go wrong
-   prints a structured object detection system summary

#### **Setup Steps**

1.  Open VS Code.
2.  Create a folder called `object-detection-planner`.
3.  Create a file called `object_detection_planner.py`.
4.  Run the file in the terminal.

#### **Sample Code**
```
# object_detection_planner.py
# AI Systems Week 3 Day 2
# This program helps Geniuses plan an object detection system.

print("Welcome to the Object Detection Planner\n")

system_name = input("What is the name of your object detection system? ")
scene_type = input("What kind of scene does the system analyze? ")
objects_to_detect = input("What objects should the system detect? ")
why_detection_matters = input("Why does detection matter in this use case? ")
risk = input("What could go wrong if the system misses or mislabels an object? ")

print("\n--- Object Detection System Summary ---")
print(f"System Name: {system_name}")
print(f"Scene Type: {scene_type}")
print(f"Objects to Detect: {objects_to_detect}")
print(f"Why Detection Matters: {why_detection_matters}")
print(f"Risk: {risk}")

print("\n--- Reflection ---")
print("Would this scene have one object or many?")
print("Would objects overlap or move quickly?")
print("Would human review still be needed?")
```
#### **Optional Extension**

Add a simple detection list simulation:
```
# optional_detected_objects.py
# This shows how a system might structure detection outputs.

detected_objects = [
    {"label": "player", "location": "(120, 80, 200, 260)", "confidence": 0.93},
    {"label": "basketball", "location": "(310, 140, 340, 170)", "confidence": 0.81},
    {"label": "hoop", "location": "(500, 60, 560, 140)", "confidence": 0.88}
]

print("\n--- Example Detection Output ---")
for obj in detected_objects:
    print(f"Label: {obj['label']}")
    print(f"Bounding Box: {obj['location']}")
    print(f"Confidence: {obj['confidence']}\n")
```
#### **Guided Practice Teaching Points**

-   Why object detection needs both labels and locations
-   Why scene type affects system difficulty
-   Why detection goals should match the real user need
-   Why confidence should not be blindly trusted
-   Why planning helps before building more advanced vision systems

#### **Guided Practice Discussion**

-   What kinds of scenes seemed easiest to design for?
-   Which use cases felt highest-risk?
-   Why is location information important?
-   What would make a detection system more trustworthy?

### 4. **Independent Practice (Time: 35 minutes)**

-   **Objective:** Geniuses independently design an object detection AI software concept for a real use case.
-   This continues the Week 3 mini-project.

#### **Mini-Project Title**

**Vision AI Software Concept --- Day 2 Object Detection Design**

#### **Independent Task**

Each Genius creates a Python file for an object detection-based software concept.

Examples:

-   sports play detector
-   retail shelf monitor
-   classroom object finder
-   training cone and ball tracker
-   smart accessibility scene detector
-   package sorting assistant
-   equipment detection system

Their concept must include:

-   system name
-   scene type
-   objects to detect
-   why detection matters
-   one trust or ethics concern
-   one responsible design choice

#### **Required Deliverables**

-   A working Python file called `my_object_detector.py`
-   A system concept with:
    -   system name
    -   scene type
    -   objects to detect
    -   why detection matters
    -   one trust concern
    -   one responsible design choice
-   A short written reflection:
    -   Why is object detection the right system behavior here?
    -   What makes the scene difficult?
    -   What must a user still verify before trusting the output?

#### **Independent Practice Starter Code**
```
# my_object_detector.py
# Week 3 Day 2 independent practice
# This program creates an object detection AI system concept.

print("My Object Detection System\n")

system_name = "PlayVision AI"
scene_type = "Basketball game footage"
objects_to_detect = "Players, ball, hoop, and court zones"
why_detection_matters = "The system helps coaches understand movement, spacing, and play flow"
trust_concern = "The system could lose track of the ball or confuse overlapping players"
responsible_design = "The output should support coaching analysis, not replace human judgment about performance"

print(f"System Name: {system_name}")
print(f"Scene Type: {scene_type}")
print(f"Objects to Detect: {objects_to_detect}")
print(f"Why Detection Matters: {why_detection_matters}")
print(f"Trust Concern: {trust_concern}")
print(f"Responsible Design Choice: {responsible_design}")
```
#### **Facilitator Support Moves**

-   Help Geniuses choose realistic scenes and object goals
-   Ask:
    -   What objects matter most in the scene?
    -   Would the system need to find one object or many?
    -   What makes this scene messy or difficult?
    -   What happens if a critical object is missed?
-   Encourage clear, visual, real-world product ideas

### 5. **Closure (Time: 20 minutes)**

-   **Objective:** Reinforce that object detection helps AI systems move from broad image understanding to scene-level awareness.
-   Bring the class together for a final share-out.
-   Ask 3--5 Geniuses to share:
    -   their system name
    -   what scene it analyzes
    -   what objects it detects
    -   one trust concern
-   Lead a closing discussion:
    -   What makes object detection more powerful than image classification?
    -   Why are bounding boxes and location information so important?
    -   What kinds of detection mistakes are most dangerous?
-   Preview the next lesson:
    -   Geniuses will move into sports analytics, player and ball tracking, and motion-based visual systems.

**Assessment:**
---------------

Student learning will be assessed through:

-   Participation in the icebreaker and discussion
-   Reflection responses during direct instruction
-   Completion of the guided Python object detection planner
-   Completion of an independent object detection concept
-   Final share-out and explanation of detection choices and risks

### **Exit Ticket**

1.  What is object detection?
2.  What is a bounding box?
3.  What is one trust risk in object detection systems?

**Extra Activities:**
---------------------

-   Geniuses who finish early can:
    -   add example detected objects with confidence scores
    -   compare a classification system and a detection system for the same scene
    -   add a "hardest object to detect" field
    -   add a "what conditions make this harder?" section
    -   create two different scene types and compare them
    -   add a "needs human review?" note
-   Add a "false positive example" section
-   Add a "false negative example" section
-   Add a "public safety use?" section
-   Add a "future feature" section for motion tracking

**Reflection / Takeaways:**
---------------------------

This lesson works best when Geniuses realize that object detection is one of the core ways AI systems turn images into useful structured information. Day 2 helps them see that visual AI is not only about saying what kind of image something is. It is about identifying multiple things, locating them, and making those detections useful in real workflows. By the end of the lesson, Geniuses should feel more confident explaining what object detection does, where it is useful, and why it must be designed with care.

**Facilitator Notes**
---------------------

-   Keep using **Geniuses** consistently in examples and discussion.
-   Reinforce that object detection is more complex than broad image classification.
-   Keep sports, accessibility, and product use cases visible to make the lesson feel current and real.
-   Encourage Geniuses to think carefully about false confidence and missed detections.
-   Remind Geniuses that tomorrow they will move into motion and sports analytics systems built on top of visual detection.

**Week 3 Day 2 Mini-Project Connection**
----------------------------------------

By the end of Day 2, each Genius should have:

-   A named object detection AI system concept
-   A defined scene type
-   A clear list of objects to detect
-   A real reason detection matters
-   At least one trust or ethics concern
-   At least one responsible design choice
-   A stronger understanding of how object detection systems turn scenes into structured information
