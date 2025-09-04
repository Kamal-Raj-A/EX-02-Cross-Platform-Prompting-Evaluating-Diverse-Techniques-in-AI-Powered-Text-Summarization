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

ChatGPT (GPT-4): A very strong all-rounder. It adapted exceptionally well to the role-based prompt, producing summaries that were both engaging and easy to understand. It consistently delivered high-quality results across all techniques.

Gemini: This platform shined with the Chain-of-Thought prompt. Its ability to process and structure the logical steps resulted in arguably the most accurate and well-reasoned summaries. Its output with the role-based prompt was also excellent and highly creative.

Claude 3: Claude's strength was in generating exceptionally fluid and coherent prose. Its summaries, particularly from the role-based prompt, read very naturally, as if written by a human educator. It was particularly good at simplifying complex ideas without losing critical details.

Copilot: As an integrated tool, its primary advantage was speed and convenience. The quality was comparable to ChatGPT, as it is based on similar models. It was extremely fast for generating quick, zero-shot summaries, but also handled the more complex prompts effectively.

## Coherence

<img width="1400" height="452" alt="image" src="https://github.com/user-attachments/assets/8a094875-8be7-4aa3-842f-09c891e51530" />


1. Logical Flow and Progression of Ideas:
A coherent summary presents information in a logical order. This doesn't necessarily mean the same order as the source article. It means the ideas are arranged to build upon one another naturally.

Example of poor flow: Starting with how blockchain is secure, then defining what a block is, then jumping to its use in cryptocurrency, and finally explaining what a ledger is. The information is all there, but the reader is forced to piece it together like a puzzle.

Example of good flow: Starting with the foundational concept (a digital ledger), then explaining how information is grouped into "blocks," how these blocks are linked into a "chain," and finally, how this structure creates security and trust. This is a logical progression from the general to the specific.

2. Clarity of Connections (The "Glue"):
This refers to how well sentences and paragraphs are linked. Coherent writing uses transitional words and phrases to signal relationships between ideas, making the text flow smoothly rather than feeling like a list of disconnected facts.

Lacks connection: "Blockchain is a distributed ledger. Every transaction is a block. Hashing makes it secure."

Shows connection: "Blockchain is fundamentally a distributed ledger. Information on this ledger is grouped into 'blocks,' which contain details of transactions. To ensure security, each block is connected to the previous one using a cryptographic principle called hashing, thereby creating a permanent and unalterable chain."

3. Unified Focus and Purpose:
A coherent summary is built around a central theme or main idea from the original text. It should not include irrelevant details or deviate onto tangents. Every sentence should serve the primary purpose of explaining the basics of the topic simply and clearly.

Lacks focus: A summary that starts explaining blockchain basics but then gets sidetracked into a detailed discussion of the 2021 cryptocurrency market fluctuations.

Maintains focus: A summary that sticks strictly to defining the technology itself—ledger, blocks, chain, decentralization, and security—as these are the core concepts promised by the title "The Basics of Blockchain Technology."

## Simplicity

<img width="2932" height="1755" alt="image" src="https://github.com/user-attachments/assets/4948c87a-d04c-427c-8b64-408b5cfd8008" />


In our project, simplicity is the crucial process of making complex ideas accessible to a non-expert audience, like the undergraduate students we serve. It's not about removing important details, but about translating them into a format that's easy to understand. This is achieved by avoiding technical jargon in favor of plain language, using shorter and more direct sentences, and employing relatable analogies to explain abstract concepts. For instance, instead of describing blockchain as a "distributed, immutable public ledger," a simpler and more effective summary would compare it to a "shared digital notebook" that everyone can see but no one can alter. This approach transforms a dense, technical topic into an intuitive idea, ensuring the summary actually educates the reader rather than just presenting them with facts.

Our evaluation revealed that achieving this simplicity from AI is highly dependent on the instructions provided. A generic "summarize" command often results in a text that retains the original article's complexity. However, the most effective method was using a Role-Based prompt, such as asking the AI to "act as a professor explaining this to first-year students." This specific instruction fundamentally changes the AI's task from merely condensing information to actively teaching a concept. By adopting the persona of an educator, the AI naturally prioritizes clarity and accessibility, consistently producing summaries that are not only accurate but genuinely simple and easy to comprehend.

## Speed



Defining "Speed" in Our Workflow: For this evaluation, speed was measured not just by the AI's raw text generation time, but by the total time taken from initial prompt to a final, usable summary. This includes the time spent writing the prompt, the AI's response time, and, most importantly, any time required for edits or re-prompting to meet our quality standards.

Raw Generation Speed is a Minor Factor: All tested platforms (ChatGPT, Gemini, Claude, Copilot) are exceptionally fast. The time taken to generate a summary from a 500-word article was consistently a matter of seconds. In terms of pure processing, the differences between platforms were negligible and not a deciding factor in overall efficiency.

Prompt Complexity vs. Overall Speed: We found an inverse relationship between the initial effort put into a prompt and the total time spent on the task.

Zero-Shot Prompts ("Summarize this"): While the fastest to type, this method was the slowest overall. The generic, often overly technical output required significant manual editing or complete re-prompting, adding several minutes to the workflow.

Role-Based & Few-Shot Prompts: These prompts took slightly longer to craft (an extra 30-60 seconds). However, they produced near-perfect summaries on the first attempt, drastically reducing or eliminating the need for any post-generation editing. This made them the fastest method from start to finish.

Workflow Integration as a Speed Advantage: The platform with a notable edge in situational speed was Copilot. Its integration directly into other applications (like a web browser or document editor) eliminates the need to switch tabs and copy-paste text. For quick, on-the-fly summarization tasks, this seamless workflow makes it feel the most immediate and efficient.

Conclusion on Speed: True speed is not about how fast the AI can type, but how quickly it can deliver a finished product. The most efficient and time-saving strategy is to use a well-crafted, specific prompt like the Role-Based technique. Investing a small amount of time upfront to tell the AI exactly what you need is the fastest way to get a summary that is ready for immediate use.

## User experience

Analysis of User Experience (UX)

In our evaluation, User Experience referred to the overall ease, predictability, and satisfaction of the process of generating a summary. It's less about the visual design of the AI platform and more about the quality of the interaction itself. A good user experience feels like a seamless collaboration, where you can reliably get the desired output with minimal effort. The key factor that defined the user experience across all platforms was not the interface, but the prompting strategy. A poor UX was characterized by "prompt friction"—the frustrating cycle of typing a prompt, getting a mediocre result, and having to repeatedly tweak the prompt to get what you need.

The difference in experience between prompt types was significant. Using a basic zero-shot prompt ("Summarize this") often led to a poor user experience. While easy to write, the unpredictability of the output meant we had to engage in a frustrating guessing game of refining our request. In contrast, using a Role-Based prompt provided a far superior and empowering user experience. By giving the AI a clear role and audience, we shifted the interaction from one of trial-and-error to one of clear instruction and reliable execution. The AI consistently delivered a high-quality summary on the first try, making the process feel efficient, predictable, and satisfying.

While all platforms offered a clean and intuitive interface, the most notable UX feature was Copilot's integration, which streamlines the workflow by eliminating the need to switch applications. However, the universal conclusion is that the user has the most control over their own experience. Mastering the use of specific, well-defined prompts is the key to transforming any of these powerful AI tools into a truly reliable and easy-to-use assistant. For our content team, creating a shared template of effective prompts will ensure a consistently positive user experience for everyone.

## Algorithm

<img width="624" height="374" alt="image" src="https://github.com/user-attachments/assets/ae28dc9c-2e4f-4e25-9983-11a7b0604d0f" />


The evaluation was conducted using a structured, multi-step process to ensure a fair and consistent comparison across all variables.

Establish a Control: A single source text was selected for all tests: a 500-word technical article titled "The Basics of Blockchain Technology." Using the same article for every test ensured that any differences in the output were due to the AI platform or the prompting technique, not the source material.

Define Evaluation Criteria: Before starting, the five key metrics were clearly defined:

Accuracy: How well the summary reflects the core facts of the original text.

Coherence: The logical flow and readability of the summary.

Simplicity: The use of plain language and avoidance of technical jargon.

Speed: The total time from writing the prompt to getting a final, usable summary.

User Experience: The perceived ease and satisfaction of the process.

Design the Prompts: Four distinct prompts were crafted, one for each technique, to be used consistently across all platforms.

Zero-Shot: A simple, direct command: Summarize the following text:

Few-Shot: A command providing an example to follow: Summarize the provided article in a simple, clear style, similar to this example: [A pre-written simple summary was inserted here].

Chain-of-Thought: A prompt guiding the AI's reasoning process: First, identify the three main concepts in the article. Second, explain each one simply. Finally, combine these explanations into a coherent summary.

Role-Based: A prompt assigning a specific persona and audience: Act as a university professor. Summarize the following article for a first-year student who is new to this topic.

Execute the Tests: Each of the four prompts was systematically run on each of the four AI platforms (ChatGPT, Gemini, Claude, Copilot). This created a total of 16 unique summaries for analysis. Each interaction was timed to measure the "Speed" criterion.

Analyze and Score: The 16 summaries were then carefully evaluated and scored against the five predefined criteria. A qualitative rating scale (Poor, Fair, Good, Excellent) was used to ensure consistent judgment. The results were compiled into a comparative matrix to easily identify patterns and determine which combinations performed best for the specific goal of creating educational content.

## Result

The prompting technique you use is significantly more important than the specific AI platform you choose.

For your team's goal of creating simple and clear summaries for undergraduate students, the most effective and efficient method is Role-Based Prompting. This technique consistently outperformed all others because it directly instructs the AI to consider the target audience, resulting in summaries that are not just accurate but also perfectly tuned in tone and simplicity.

Therefore, the final recommendation is to standardize your summarization process around a role-based prompt structure. While all platforms like ChatGPT, Gemini, and Claude perform exceptionally well with this method, your best results will come from a prompt like:

"Act as a university professor. Summarize the following text for a first-year undergraduate student who has no prior knowledge of the topic."

In short, the key to success is not in finding the "best" AI, but in mastering the art of asking the AI to become the best summarizer for your specific needs.

