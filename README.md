# EX-02-Cross-Platform-Prompting-Evaluating-Diverse-Techniques-in-AI-Powered-Text-Summarization

## AIM
To evaluate and compare the effectiveness of prompting techniques (zero-shot, few-shot, chain-of-thought, role-based) across different AI platforms (e.g., ChatGPT, Gemini, Claude, Copilot) in a specific task: text summarization.

## Scenario:
You are part of a content curation team for an educational platform that delivers quick summaries of research papers to undergraduate students. Your task is to summarize a 500-word technical article on "The Basics of Blockchain Technology" using multiple AI platforms and prompting strategies.

<img width="685" height="273" alt="image" src="https://github.com/user-attachments/assets/5e76d064-dd30-499e-831e-aac5f4423da3" />


<img width="277" height="182" alt="image" src="https://github.com/user-attachments/assets/062b9773-a931-403f-b557-5c608b9ce680" />

Your goal is to determine which combination of prompting technique + platform provides the best summary in terms of:

## Accuracy

<img width="960" height="539" alt="Screenshot 2025-09-04 091813" src="https://github.com/user-attachments/assets/64733efc-67d0-447c-b43b-a91c906c3274" />

ChatGPT (GPT-4): A very strong all-rounder. It adapted well to the role-based prompt, producing summaries that were engaging and easy to understand. It consistently delivered high-quality results across all techniques.

Gemini: This platform excelled with the Chain-of-Thought prompt. Its ability to process and organize the logical steps led to some of the most accurate and well-reasoned summaries. Its output with the role-based prompt was also excellent and highly creative.

Claude 3: Claude's strength was in generating fluid and coherent prose. Its summaries, particularly from the role-based prompt, felt very natural, as if written by a human educator. It was especially good at simplifying complex ideas without losing important details.

Copilot: As an integrated tool, its main advantage was speed and convenience. The quality was similar to ChatGPT, as it is based on similar models. It was extremely fast for generating quick summaries but also handled more complex prompts effectively.

## Coherence

<img width="1400" height="452" alt="image" src="https://github.com/user-attachments/assets/8a094875-8be7-4aa3-842f-09c891e51530" />

Logical Flow and Progression of Ideas: A coherent summary presents information in a logical order. This doesn't have to be the same order as the source article. The ideas should be arranged to build on one another naturally.  
Example of poor flow: Starting with how blockchain is secure, then defining what a block is, then jumping to its use in cryptocurrency, and finally explaining what a ledger is. The information is there, but the reader has to piece it together like a puzzle.

Example of good flow: Starting with the basic concept (a digital ledger), then explaining how information is grouped into "blocks," how these blocks are linked into a "chain," and finally, how this structure creates security and trust. This follows a logical progression from the general to the specific.

Clarity of Connections (The "Glue"): This refers to how well sentences and paragraphs are connected. Coherent writing uses transitional words and phrases to show relationships between ideas, making the text flow smoothly instead of feeling like a list of disconnected facts.  
Lacks connection: "Blockchain is a distributed ledger. Every transaction is a block. Hashing makes it secure."

Shows connection: "Blockchain is fundamentally a distributed ledger. Information on this ledger is grouped into 'blocks,' which contain details of transactions. To ensure security, each block is connected to the previous one using a cryptographic principle called hashing, creating a permanent and unchangeable chain."

Unified Focus and Purpose: A coherent summary centers around a main theme or idea from the original text. It should not include irrelevant details or stray off topic. Every sentence should serve the main purpose of explaining the basics of the topic simply and clearly.  
Lacks focus: A summary that starts explaining blockchain basics but then gets sidetracked into a detailed discussion of the 2021 cryptocurrency market fluctuations.

Maintains focus: A summary that strictly defines the technology itself—ledger, blocks, chain, decentralization, and security—as these are the core concepts promised by the title "The Basics of Blockchain Technology."


## Simplicity

<img width="2932" height="1755" alt="image" src="https://github.com/user-attachments/assets/4948c87a-d04c-427c-8b64-408b5cfd8008" />

In our project, simplicity is the key process for making complex ideas easy for a non-expert audience, like undergraduate students. It's about translating important details into an easy-to-understand format, not about removing them. This is done by avoiding technical terms and using plain language, along with shorter, direct sentences and relatable analogies to clarify abstract concepts. For example, instead of calling blockchain a "distributed, immutable public ledger," a clearer summary might describe it as a "shared digital notebook" that everyone can see but no one can change. This method changes a dense, technical topic into a more intuitive idea. It ensures that the summary educates the reader rather than just providing facts.

Our evaluation showed that achieving simplicity using AI depends heavily on the instructions given. A general "summarize" command often leads to text that keeps the original article's complexity. The most effective approach was using a Role-Based prompt, like telling the AI to "act as a professor explaining this to first-year students." This specific instruction changes the AI's role from merely condensing information to actively teaching a concept. By taking on the persona of an educator, the AI focuses on clarity and accessibility. It consistently produces summaries that are not only correct but also simple and easy to understand.


## Speed

Defining "Speed" in Our Workflow: In this evaluation, speed was measured not only by how quickly the AI generates text but also by the total time from the initial prompt to a final, usable summary. This includes the time spent crafting the prompt, the AI's response time, and any needed edits or re-prompts to meet our quality standards.

Raw Generation Speed is a Minor Factor: All platforms we tested (ChatGPT, Gemini, Claude, Copilot) are extremely fast. The time to generate a summary from a 500-word article was consistently just seconds. In terms of processing speed, the differences among platforms were minimal and did not significantly affect overall efficiency.

Prompt Complexity vs. Overall Speed: We found that the initial effort put into a prompt and the total time spent on the task were inversely related.

Zero-Shot Prompts ("Summarize this"): This method was the quickest to type but ended up being the slowest overall. The generic, often overly technical output required significant manual editing or complete re-prompting, adding several minutes to the workflow.

Role-Based & Few-Shot Prompts: These prompts took a little longer to create (an extra 30-60 seconds). However, they produced nearly perfect summaries on the first attempt, greatly reducing or eliminating the need for any post-generation editing. This made them the fastest method from start to finish.

Workflow Integration as a Speed Advantage: The platform that showed a clear advantage in situational speed was Copilot. Its integration into other applications, like a web browser or document editor, avoids the need to switch tabs and copy-paste text. For quick summarization tasks, this seamless workflow feels the most immediate and efficient.

Conclusion on Speed: True speed is about how quickly the AI can deliver a finished product, not just how fast it can type. The most efficient strategy uses a well-crafted, specific prompt like the Role-Based technique. Spending a small amount of time upfront to clearly state what you need is the best way to obtain an immediately usable summary.


## User experience



## Algorithm

<img width="624" height="374" alt="image" src="https://github.com/user-attachments/assets/ae28dc9c-2e4f-4e25-9983-11a7b0604d0f" />

The evaluation was conducted through a structured, multi-step process to guarantee a fair and consistent comparison across all variables.

Establish a Control: One source text was used for all tests: a 500-word technical article titled "The Basics of Blockchain Technology." Using the same article for every test ensured that any output differences stemmed from the AI platform or the prompting technique, not the source material.

Define Evaluation Criteria: Before we began, we clearly defined five key metrics:

- Accuracy: How well the summary reflects the core facts of the original text.
- Coherence: The logical flow and readability of the summary.
- Simplicity: The use of plain language and avoidance of technical jargon.
- Speed: The total time from writing the prompt to getting a final, usable summary.
- User Experience: The ease and satisfaction of the process.

Design the Prompts: Four distinct prompts were created, one for each technique, to be used consistently across all platforms.

Zero-Shot: A simple command: Summarize the following text:

Few-Shot: A command providing an example to follow: Summarize the provided article in a simple, clear style, similar to this example: [A pre-written simple summary was inserted here].

Chain-of-Thought: A prompt guiding the AI's reasoning process: First, identify the three main concepts in the article. Second, explain each one simply. Finally, combine these explanations into a coherent summary.

Role-Based: A prompt assigning a specific persona and audience: Act as a university professor. Summarize the following article for a first-year student who is new to this topic.

Execute the Tests: Each of the four prompts was systematically used on each of the four AI platforms (ChatGPT, Gemini, Claude, Copilot). This created a total of 16 unique summaries for analysis. Each interaction was timed to measure the "Speed" criterion.

Analyze and Score: The 16 summaries were scored against the five metrics we defined. We used a qualitative rating scale (Poor, Fair, Good, Excellent) to maintain consistent judgment. The results were compiled into a comparative matrix to easily identify patterns and find the best combinations for creating educational content.


## Result

The prompting technique you use is significantly more important than the specific AI platform you choose.

For your team's goal of creating simple and clear summaries for undergraduate students, the most effective and efficient method is Role-Based Prompting. This technique consistently outperformed all others because it directly instructs the AI to consider the target audience, resulting in summaries that are not just accurate but also perfectly tuned in tone and simplicity.

Therefore, the final recommendation is to standardize your summarization process around a role-based prompt structure. While all platforms like ChatGPT, Gemini, and Claude perform exceptionally well with this method, your best results will come from a prompt like:

"Act as a university professor. Summarize the following text for a first-year undergraduate student who has no prior knowledge of the topic."

In short, the key to success is not in finding the "best" AI, but in mastering the art of asking the AI to become the best summarizer for your specific needs.

