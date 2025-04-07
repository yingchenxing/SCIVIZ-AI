# SCIVIZ AI

## Inspiration
This project was inspired by our own experience. When we took the database course, we struggled to understand the concept of the B+ tree. It was difficult to grasp how it works and how elements are inserted into it. We searched for videos on YouTube, but often couldn’t find explanations that covered the edge cases.

Another challenge came from our materials science course. The lecture slides were outdated and completely static. But in a subject where understanding how atoms behave under different environments is crucial, static content just isn’t enough. As students, we wanted to see how atoms respond to changes, not just read about it.

These experiences made us wonder: what if students or instructors could easily create videos to explain complex concepts, using just simple instructions?

## What it does
Our website converts user instructions into AI-generated, dynamic, animated videos. For example, a user might ask, "What is the blackhole?" The system starts by generating a clear and concise script and inputs it into the video generator. In just a few minutes, the user receives a short video complete with narration and simple animations explaining the blackhole. The result is a personalized explainer video on demand, designed to make learning accessible, engaging, and fun. Whether users are curious about science or math, the website delivers videos in a fast and visually appealing format.

## How we built it

### Front-end:
We developed a scientific visualization platform by leveraging **Next.js** as our React framework foundation with **TypeScript**. For styling, we've implemented **Tailwind CSS**. For UI component architecture, we built upon Shadcn UI's component system. Our development workflow is optimized with tools like **ESLint** for code quality.

### Back-end
We built a dynamic educational platform by combining Node.js with AI technologies, using Claude 3 Sonnet to generate Manim animation code, incorporating OpenAI's voiceover capabilities for narration, and leveraging Google's Gemini AI to create comprehensive explanations, all working together to transform complex concepts into engaging, visually appealing animations with synchronized audio and captions for both students and instructors.


## Challenges we ran into
Throughout our development journey, we encountered several significant challenges that required solutions. Fine-tuning the prompt engineering for LLM was crucial to generate accurate Manim code that consistently produced high-quality animations with proper voiceovers and captions. 

We implemented streaming capabilities for both video delivery and AI-generated explanations to ensure a smooth user experience, while also developing a robust file management system for seamless video processing and transfer. 

One of our biggest challenges was handling animation errors, which we solved by creating a retry mechanism that automatically detects failures, uses Claude to revise the code, and attempts execution up to three times, significantly improving the success rate of our animation generation process.

## Accomplishments that we're proud of

We are proud of several key accomplishments. 

First, we successfully built an end-to-end system that takes user questions and generates AI-powered explainer videos, combining language generation, video synthesis, and narration into a seamless pipeline. We significantly improved performance by reducing video generation times from over 10 minutes to just a few minutes, making the user experience much smoother. We also tackled challenges such as aligning narration with visuals, simplifying AI-generated scripts for clearer explanations, and managing costs effectively by exploring open-source alternatives. Most importantly, we created an engaging and functional prototype that demonstrates the potential of AI-generated educational videos, and we have already received positive feedback from early testers.

## What we learned
This journey was a crash course in AI and teamwork. We mastered prompting LLMs to keep answers short and sweet, a skill that’s harder than it sounds. We learned the ins and outs of video AI, like how to tweak pacing, visuals, and voiceovers for clarity. 

## What's next for SciViz AI
We are just getting started. Our next focus is reducing video render times to under 30 seconds. We also plan to introduce more customization, allowing users to choose narrator voices, adjust visual styles, and personalize their learning experience. 
