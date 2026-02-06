My AI Eval & Quality Journey (Building in Public)
This is my technical log where I’m documenting my 6-month deep dive into AI evaluation, RLHF, and RAG quality. I’m building this project bit by bit every day, so this repo is very much a "work in progress."

🎯 What I’m Chasing
I’m simulating what it’s like to manage AI quality in a real production environment. No be just to tell the AI "how far," I’m looking at three main things: Is the answer correct? Is it based on the facts I gave it? And is it safe for people to use?

🛠️ The Tools I’m Using (As I go)
Since I’m building this daily, my stack is still evolving, but here’s what I’m currently rocking:

Eval Method: Using Label Studio and proper RLHF guidelines to grade the models. It’s a lot of "Human-in-the-loop" work—eye-service is actually required here!

The Code Side: Python is my go-to for automating all the repetitive stuff. I’m still figuring out the best way to handle session persistence as the project grows.

The Models: Right now, I’m putting GPT-4o, Gemini 1.5 Pro, and Llama 3 through their paces.

📁 Repository Map (The Layout)
I’m populating these folders one-one as I move:

/instruction_following: Auditing if the AI can follow simple rules without "doing its own."

/groundedness_hallucination: Checking if the model is telling the truth or just vibes and stories.

/rag_evaluation: This is where I test how well the model reads the context I provide.

/safety_red_teaming: Trying my best to "break" the model to see if it’ll say what it’s not supposed to.

/scripts_and_automation: My Python scripts that make the whole evaluation loop run faster.
