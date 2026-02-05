Month 4: RAG Evaluation (Sticking to the Script)
What I’m looking for here: This month is all about boundary testing. When I give a model a specific set of documents, I want to see if it can stay strictly within those pages. I’m checking if it’s disciplined enough to say "the document doesn't say that" instead of pulling answers from its general training data.

My focus areas for this review:
Staying in its lane (Context Adherence): I’m testing if the model can answer only using what I provided. If I give it a manual for a Toyota and it starts talking about a Honda, it fails.

Spotting the "Outside" Info (Out-of-scope): I’ll be checking if the model is smart enough to detect when a question is outside the provided context. I’m looking for a clean "I don't have that information" rather than a guess.

Connecting dots that aren't there (Inference Errors): Sometimes a model takes a half-sentence and makes a huge, wrong assumption. I’m watching out for these "reaches" where the logic starts to break down.

The Truth vs. The Full Story (Faithfulness vs. Completeness): I’m looking for a balance. I'd rather have a model give a short, 100% faithful answer than a long, complete-sounding response that is 20% made up.

The Face-Off:
Control Model: Gemini 1.5 Flash (Fast and usually very grounded).

Challenger Model: Mistral Large (To see how a high-parameter open-weight model handles strict context boundaries).

My Perspective as an Evaluator:
In this phase, I’m being extra strict about grounding. I’ll be flagging even the smallest "hallucinated" details. If the model adds even one adjective that isn't in the source text, I’m calling it out. I want to see which model remains "faithful" to the source without getting over-confident and filling in the gaps with its own imagination.