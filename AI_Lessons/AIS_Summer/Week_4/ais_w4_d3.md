<img src="https://github.com/Hgp-GeniusLabs/Curriculum/blob/10734f2c827128dde773ea4f266d154d46977866/Org-Wide/Assets/hgp_logo_original.png" width="150"/>

Lesson Plan: AI Systems Week 4, Day 3 --- Adding Voice, TTS, and Spoken Agent Output
==================================================================================

**Duration:**
-------------

3 hours

**Lesson Overview:**
--------------------

On Day 3, Geniuses take their multimodal agents one step further by adding **voice and spoken output**. After learning what makes an agent different from a chatbot and building image-aware reasoning agents, Geniuses now focus on how AI systems can **speak back to the user** in a more embodied, interactive way. This lesson introduces **text-to-speech (TTS)** as part of agent design and explores how voice changes the product experience.

Geniuses examine how spoken output can make AI systems feel more immediate, more accessible, and more assistant-like. They also explore the risks that come with voice, especially that spoken AI can sound more confident and more believable than it really is. The lesson emphasizes that voice should not just be added because it sounds cool. It should improve accessibility, usability, and product value. During guided practice, the class builds a Python-based vision-and-voice agent workflow that returns structured text and saves a spoken response. During independent practice, each Genius creates a voice-enabled agent prototype for a real use case. By the end of the lesson, Geniuses should understand that TTS is not just output polish. It is a product and trust design choice.

**Objectives:**
---------------

-   Explain how TTS changes the user experience of an AI system.
-   Identify use cases where spoken output is genuinely helpful.
-   Distinguish between useful spoken responses and overly authoritative voice behavior.
-   Build a Python-based agent workflow that produces text output and spoken output.
-   Use the OpenAI API to create a simple TTS-enabled multimodal agent experience.
-   Reflect on trust, accessibility, tone, and review needs in speaking AI systems.
-   Continue the Week 4 mini-project by adding voice capability to an agent concept or prototype.

**Materials:**
--------------

-   Laptops for all Geniuses
-   VS Code installed
-   Python installed and working
-   OpenAI API key for each Genius or team
-   Internet access
-   Projector or display
-   Whiteboard and markers
-   Slide deck for lecture and discussion
-   Reflection journal or digital notes
-   Terminal access in VS Code
-   Speakers or headphones if available
-   Starter folder for Python files
-   `.env` setup instructions for API keys

**Standards:**
--------------

-   Computational Thinking: Analyze how output mode changes system behavior and user experience.
-   Computer Science Practices: Build and test an AI workflow that uses text generation and speech output together.
-   Programming: Use Python and the OpenAI API to generate text and spoken audio.
-   Digital Literacy: Evaluate how voice affects trust, accessibility, and perception in AI systems.
-   Career Readiness: Practice technical explanation, experimentation, and product design thinking.
-   Technical Foundations: Explain how TTS fits into a multimodal agent workflow.

**Lesson Activity:**
--------------------

### 1. **Introduction (Time: 25 minutes)**

-   **Objective:** Energize Geniuses and introduce the idea that voice changes how an AI system feels and how much users may trust it.
-   Start with a fun icebreaker called **"Text Only or Say It Out Loud?"**
-   This should be the first thing and the most fun thing to wake Geniuses up and get them ready for the lesson.

#### **Icebreaker Option A: Physical Movement**

-   Label one side of the room **"Text Is Enough"** and the other side **"Voice Helps More."**
-   Read scenarios aloud and have Geniuses move to the side that best matches.
-   Example prompts:
    -   A student wants a written summary of homework instructions
    -   A low-vision user wants help understanding a scene
    -   A coach wants quick spoken drill reminders during training
    -   A designer wants written critique of a flyer draft
    -   A user wants step-by-step directions while their hands are busy
    -   A Genius wants a study guide they can listen to while walking
    -   A user wants a high-stakes health explanation
-   After each round, ask:
    -   Why is text enough here or not enough?
    -   When does voice make the product more helpful?
    -   When might voice make the system feel too authoritative?
    -   What should users still verify even if the agent sounds confident?

#### **Icebreaker Option B: Voice Product Brainstorm**

-   Ask Geniuses to name products where voice would improve the experience.
-   Then ask them to name products where voice might not help or might create risk.
-   Discuss why voice is a design choice, not just a feature.

#### **Transition**

-   Say:
    -   "When an AI system speaks, it can feel more natural and more accessible. But it can also feel more believable than it deserves."
-   Ask:
    -   What kinds of tasks benefit from spoken output?
    -   What kinds of tasks need extra caution if the AI is speaking?

### 2. **Direct Instruction (Time: 55 minutes)**

-   **Objective:** Help Geniuses understand TTS as part of multimodal agent design and why spoken AI changes trust and product experience.
-   Use slides to guide instruction and keep it interactive.

#### **Suggested Slide Flow**

-   **Slide 1: What Is TTS?**
    -   TTS means text-to-speech
    -   A system generates text and then turns that text into audio
    -   This creates a spoken output experience
-   **Slide 2: Why Voice Matters**
    -   accessibility
    -   hands-free support
    -   faster feedback
    -   more natural interaction
    -   stronger sense of an assistant or guide
-   **Slide 3: Where Voice Helps**
    -   accessibility tools
    -   coaching assistants
    -   language practice
    -   study support
    -   scene explanation
    -   real-time instructions
    -   navigation and task guidance
-   **Slide 4: Text Output vs Spoken Output**
    -   Text can be reviewed more carefully
    -   Spoken output feels faster and more immediate
    -   Spoken output can also hide uncertainty more easily
-   **Slide 5: Voice as Product Design**
    -   What should the agent say?
    -   How long should it speak?
    -   Should it summarize or explain?
    -   Should it use caution language?
    -   Should it sound formal, supportive, calm, or instructional?
-   **Slide 6: Risks in Voice AI**
    -   sounding too confident
    -   users overtrusting the system
    -   weak outputs sounding polished
    -   poor tone for the situation
    -   privacy concerns in public spaces
    -   using speech where silence or text would be safer
-   **Slide 7: Responsible Voice Design**
    -   keep spoken output focused
    -   communicate uncertainty when needed
    -   avoid sounding like final authority in high-stakes use
    -   support review and follow-up
    -   use voice where it adds real value
-   **Slide 8: TTS in Multimodal Agents**
    -   user goal
    -   image or scene input
    -   agent reasoning
    -   text response
    -   spoken response
    -   trust reminder if needed
-   **Slide 9: Real Product Examples**
    -   visual accessibility assistant
    -   spoken worksheet explainer
    -   training coach
    -   event setup guide
    -   design review assistant
    -   voice-first study support tool
-   **Slide 10: Week 4 Direction**
    -   Geniuses will soon connect speaking agents to image generation so the full agent can see, talk, and create

#### **Discussion Questions**

-   Why does voice make an AI system feel different from text?
-   When is spoken output clearly useful?
-   Why can voice increase trust risk?
-   What kinds of voice outputs should be shorter and more cautious?
-   How can a builder make a speaking agent more responsible?

#### **Reflection Prompt**

-   Have Geniuses write for 4 minutes:
    -   "Describe one AI agent that would be improved by spoken output. What should it say, and what should it avoid sounding too certain about?"

### 3. **Guided Practice (Time: 50 minutes)**

-   **Objective:** Help Geniuses build a Python-based vision-and-voice agent workflow that returns text and saves a spoken response.
-   Explain that today's code-along is about turning a text-based agent response into a more embodied output experience.
-   The class will create `vision_voice_agent.py`.

#### **Guided Practice Build**

Create a folder called `vision-voice-agent`.

#### **Project Goal**

Build a Python program that:

-   asks the user for a goal
-   asks for image or scene context
-   generates a structured text response
-   converts part of that response into speech
-   saves the spoken audio to a file

#### **Setup Steps**

1.  Open VS Code.
2.  Create a folder called `vision-voice-agent`.
3.  Open the terminal in VS Code.
4.  Install dependencies:
```
pip install openai python-dotenv
```
1.  Create a `.env` file:
```
OPENAI_API_KEY=your_key_here
```
1.  Create a file called `vision_voice_agent.py`

#### **Sample Code**
```
# vision_voice_agent.py
# AI Systems Week 4 Day 3
# This program creates a vision + voice agent workflow
# with structured text output and spoken audio output.

import os
from dotenv import load_dotenv
from openai import OpenAI

load_dotenv()
client = OpenAI(api_key=os.getenv("OPENAI_API_KEY"))

print("Welcome to the Vision + Voice Agent\n")

user_goal = input("What does the user want help with? ")
image_context = input("Describe the image or scene the agent is using: ")

prompt = f"""
You are a vision-aware support agent.

The user's goal is:
"{user_goal}"

The image or scene is described as:
"{image_context}"

Return your answer in this format:

Key Finding:
- ...

Helpful Guidance:
- ...

Next Step:
- ...

Short Spoken Response:
- ...
"""

response = client.responses.create(
    model="gpt-4.1-mini",
    input=prompt
)

text_output = response.output_text
print("\n--- Agent Text Output ---")
print(text_output)

# Create a shorter spoken response from the generated output
spoken_prompt = f"""
Take the following agent output and create a short spoken response
that sounds helpful, clear, and not overly authoritative.

Agent output:
{text_output}

Keep the spoken response under 3 sentences.
"""

spoken_text_response = client.responses.create(
    model="gpt-4.1-mini",
    input=spoken_prompt
)

spoken_text = spoken_text_response.output_text.strip()

print("\n--- Spoken Response Text ---")
print(spoken_text)

# Generate audio and save it
audio_response = client.audio.speech.create(
    model="gpt-4o-mini-tts",
    voice="alloy",
    input=spoken_text
)

with open("agent_response.mp3", "wb") as f:
    f.write(audio_response.read())

print("\nSaved spoken response to agent_response.mp3")

print("\n--- Reflection ---")
print("Did the spoken version feel more natural?")
print("Did it sound too certain anywhere?")
print("What should still be reviewed by a human?")
```
#### **Guided Practice Teaching Points**

-   Why spoken output should be shorter than full text output
-   Why voice changes the feeling of the agent
-   Why caution language matters more in voice mode
-   Why TTS belongs inside a bigger workflow, not as a standalone trick
-   Why saving audio output makes the agent feel more like real software

#### **Guided Practice Discussion**

-   What made the spoken version more useful or less useful?
-   Did the spoken response sound too confident anywhere?
-   Why is short voice output often better than long speech?
-   What kinds of products would benefit most from this workflow?

### 4. **Independent Practice (Time: 30 minutes)**

-   **Objective:** Geniuses independently create a voice-enabled agent prototype for a real use case.
-   This continues the Week 4 mini-project.

#### **Mini-Project Title**

**Multimodal Agent System Concept --- Day 3 Voice + TTS Agent**

#### **Independent Task**

Each Genius creates a Python file that adds spoken output to their agent concept.

Examples:

-   worksheet explainer with spoken summary
-   design feedback agent with voice notes
-   accessibility helper with spoken scene guidance
-   sports coach agent with drill reminders
-   event setup assistant with spoken next steps

Their system must include:

-   agent name
-   user
-   user goal
-   image or scene input
-   text output
-   spoken output
-   one trust or ethics concern
-   one responsible design choice

#### **Required Deliverables**

-   A working Python file called `my_voice_agent.py`
-   A working `.env` file configured locally
-   A TTS-enabled agent concept with:
    -   agent name
    -   user
    -   user goal
    -   visual input
    -   text response
    -   spoken response
    -   one trust concern
    -   one responsible design choice
-   A short written reflection:
    -   Why does voice improve this product?
    -   What should the spoken response avoid doing?
    -   What should still be checked by a human?

#### **Independent Practice Starter Code**
```
# my_voice_agent.py
# Week 4 Day 3 independent practice
# This program creates a voice-enabled multimodal agent.

import os
from dotenv import load_dotenv
from openai import OpenAI

load_dotenv()
client = OpenAI(api_key=os.getenv("OPENAI_API_KEY"))

agent_name = "CoachVoice AI"
user = "Athletes in training"
user_goal = input("What does the athlete want help with? ")
image_context = input("Describe the training image or scene: ")

prompt = f"""
You are a supportive training feedback agent.

The user is:
"{user}"

The goal is:
"{user_goal}"

The scene is:
"{image_context}"

Return your answer in this format:

Main Observation:
- ...

Coaching Tip:
- ...

Short Spoken Response:
- ...
"""

response = client.responses.create(
    model="gpt-4.1-mini",
    input=prompt
)

text_output = response.output_text
print(f"\nAgent Name: {agent_name}")
print("\n--- Text Output ---")
print(text_output)

speech_text = "Keep working with good form. Focus on one improvement at a time and review this with your coach."

audio_response = client.audio.speech.create(
    model="gpt-4o-mini-tts",
    voice="alloy",
    input=speech_text
)

with open("coach_voice.mp3", "wb") as f:
    f.write(audio_response.read())

print("\nSaved spoken response to coach_voice.mp3")
print("\nTrust Note: Voice guidance should support training reflection, not replace coaching judgment or real-time safety decisions.")
```
#### **Facilitator Support Moves**

-   Help Geniuses choose a use case where voice genuinely improves usability
-   Ask:
    -   Why is voice better than text alone here?
    -   What should the spoken response be short enough to say well?
    -   What kind of tone should the system use?
    -   What should users never trust blindly just because it sounds polished?
-   Encourage systems that are accessible, useful, and carefully framed

### 5. **Closure (Time: 20 minutes)**

-   **Objective:** Reinforce that voice output can make AI agents more useful and accessible, but also increases trust design responsibilities.
-   Bring the class together for a final share-out.
-   Ask 3--5 Geniuses to share:
    -   their agent name
    -   what kind of help it speaks out loud
    -   why voice improves the experience
    -   one trust or ethics concern
-   Lead a closing discussion:
    -   What makes voice helpful in an AI agent?
    -   Why can spoken AI feel more believable than text?
    -   What should builders do to keep speaking agents responsible?
-   Preview the next lesson:
    -   Geniuses will add image generation so their agent can not only see and speak, but also create visual output as part of solving a task.

**Assessment:**
---------------

Student learning will be assessed through:

-   Participation in the icebreaker and discussion
-   Reflection responses during direct instruction
-   Completion of the guided Python vision + voice agent build
-   Completion of an independent TTS-enabled agent prototype
-   Final share-out and explanation of usability and trust choices

### **Exit Ticket**

1.  What is TTS?
2.  Why can spoken AI feel more believable than text AI?
3.  What is one trust risk in a voice-enabled AI agent?

**Extra Activities:**
---------------------

-   Geniuses who finish early can:
    -   try different voice styles
    -   shorten or lengthen the spoken output and compare it
    -   add a caution sentence to the voice response
    -   create a second mode for text-only vs voice-enabled
    -   add a "when not to use voice" note
    -   build a second TTS use case
-   Add a "best tone" section
-   Add a "voice should not be used for..." section
-   Add a "human review needed" reminder
-   Add a "future image generation step" section

**Reflection / Takeaways:**
---------------------------

This lesson works best when Geniuses realize that spoken output changes an AI system from something that feels like a tool into something that feels more like an assistant. Day 3 helps them understand that TTS is not only a technical feature. It is a product decision that affects accessibility, trust, tone, and user experience. By the end of the lesson, Geniuses should feel more confident building agents that speak while also recognizing that voice makes responsible design even more important.

**Facilitator Notes**
---------------------

-   Keep using **Geniuses** consistently in examples and discussion.
-   Reinforce that voice should add usability, not just novelty.
-   Encourage short, focused spoken responses instead of long speeches.
-   Keep trust, authority, and overconfidence visible throughout the lesson.
-   Remind Geniuses that tomorrow they will add image generation so their agents can create as well as see and speak.

**Week 4 Day 3 Mini-Project Connection**
----------------------------------------

By the end of Day 3, each Genius should have:

-   A named voice-enabled agent concept or prototype
-   A defined user and user goal
-   A clear visual input type
-   A text output and spoken output pathway
-   Experience using TTS with the OpenAI API
-   At least one trust or ethics concern
-   At least one responsible design choice
-   A stronger understanding of how voice changes the design and responsibility of multimodal AI agents
