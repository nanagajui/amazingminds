# amazingminds
Educational tool for neurodiverse learners

The overall objective of this project is to create a Web App for Students who benefit from educational interventions to assist with their learning needs.

Teachers are under increasing pressure to assist their students by providing a wide range of learning delivery methods that are increasingly beyond their capcity to deliver. 

Learning requirements change dynamically throughout each session and apporaches that might be effective at times may not always be applicable to the same child. 

AI technology is able to assist teachers and their students by helping to provide learning assistance in a way that is better suited to each individual even as the situation changes each moment. 

This plan outlines a highlevel plan for this project outlining steps needed in creating a web application that leverages LLMs and MMLLMs to provide personalised support to teachers and their students with learning difficulties, this approach takes into account various learning needs and mental health considerations.

# Define User Personas & Needs:

At this stage the app will focus on dyslexia, ADHD, auditory processing disorder, autism spectrum disorder and will also consider comobidities often associated with these disorders.

Work required  - Create detailed user personas representing target student profiles, outlining their needs, challenges, and preferences in learning support.


# Design the Front-End Interface:

The front end of the app will prioritise accessibility and ease of use for both teachers and students with diverse learning needs:
Design requirements: 
  Large fonts (adjustable)
  Clear visual hierarchy
  Color contrast options
  Assistive technologies integration (e.g., screen readers, text-to-speech)
  Implement a user-friendly chat interface for interacting with the LLM.
  Implement a MMLLM interface to allow understanding of classroom learning materials and student awareness. 
Based on the initial profile that is created further taioloring of the interface is expected, for example, the interface will reflect the requirements similar to how the LLM will be instructed to interact with the student. 


# Develop Backend Infrastructure:
Choose a suitable backend framework (e.g., Node.js, Django) and database (e.g., PostgreSQL, MongoDB) to store user data and learning task details securely.
Design APIs to handle communication between the front-end and LLM server.
Design APIs to allow the vision model to understand the student and their work
# Implement User Authentication:

Allow users to create accounts and log in, enabling personalized settings and progress tracking.
Ensure secure storage and handling of user credentials.
Integrate LLM Functionality:

Set up a local server to host the chosen LLM (e.g., OpenAI's GPT).
Develop mechanisms for sending student prompts to the LLM and receiving responses.

# LLM Response Processing & Delivery:

Crate logic to analyze LLM responses and tailor them to individual student needs based on their user profile:
Pre-Prompt Engineering: Craft specific pre-prompts to guide the LLM towards generating suitable responses. This is essential for tailoring tone, complexity, and format.
  
  Example for Dyslexia: 
  User Input: "What is photosynthesis?" Pre-Prompt: "[Explain in simple terms, using short sentences] Photosynthesis is..."

  Example for ADHD:
  User Input: "Can you help me understand the water cycle?" Pre-Prompt: "[Break down the explanation into steps]: Here's how the water cycle works. Step 1: ..."

Use these pre-prompts in addition to other tailoring methods below

Response Tailoring Methods:
Sentence Simplification (Dyslexia): Break down long sentences into shorter ones. Use simpler vocabulary.
Text-to- speech (Dyslexia, ADHD): Offer text-to-speech options for students to listen rather than read.
Visual Aids (Dyslexia, Auditory Processing Disorder (APD), ASD): Use images, diagrams, mind maps to illustrate concepts alongside text.
Written Summaries (APD): Provide written summaries of audio content. * Direct Language (ASD): Use clear and literal language, avoiding idioms or sarcasm.
Structured Responses (ASD): Present information in a highly organized way using bullet points, numbered lists.

# Addressing Mental Health Needs:

There are a range of comorbitity factors that will need to be considered dynamically during learning sessions, meaning although there may be a set profile of diagnosis, there will be an intelligent response to behaviours demonstrated.
## **Dynamic Intervention Approach** -  the need for flexible and adaptable interventions based on the fluctuating nature of behaviors and their interaction with diagnoses. 

Anxiety/Overwhelm:
Keep responses concise and reassuring.
Offer positive reinforcement and encouragement.
Prompt Example: "[Encourage the user] That's a great question! Let's work through it together..."

# Testing and Refinement:
Conduct thorough testing with students representing different learning profiles.
Gather feedback and iterate on the design, interface, and LLM responses to optimize user experience.

# Output Format
The output should be a functional web application accessible through a web browser. The application will have a graphical user interface (GUI) for student interaction and a backend system handling data storage and communication with the LLM.

# Examples

Student Input: "I need help writing a book review for 'To Kill a Mockingbird'."
App Interaction: [The app asks questions about the student's learning needs, such as preferred learning style, any assistive technologies used.]
LLM Response (Processed):
[Text-to-speech option enabled] "Let's break down this book review. What are some key themes you noticed in 'To Kill a Mockingbird'? Maybe start by thinking about the characters and their relationships."
(Real examples would involve more complex interactions, incorporating personalized support based on student responses and identified learning needs)

# Notes

Prioritize user privacy and data security throughout development.
Adhere to accessibility guidelines (WCAG) for inclusive design.
Ethical Considerations:
Ensure responsible use of LLMs, addressing potential biases in outputs and mitigating risks of inappropriate or harmful content generation.
Obtain informed consent from users (or their guardians) regarding data collection and usage.
