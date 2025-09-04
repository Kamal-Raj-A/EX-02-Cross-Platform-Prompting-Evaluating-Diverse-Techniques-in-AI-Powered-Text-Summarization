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

ChatGPT (GPT-4): This model is a powerhouse across the board. It adapted seamlessly to the role-based prompt, crafting summaries that were not only engaging but also easy to grasp. It consistently produced top-notch results across various techniques.

Gemini: This platform really shone with the Chain-of-Thought prompt. Its knack for processing and organizing logical steps resulted in some of the most precise and well-reasoned summaries. The output for the role-based prompt was equally impressive and bursting with creativity.

Claude 3: Claude truly excelled at generating smooth and coherent prose. Its summaries, especially those from the role-based prompt, felt incredibly natural, almost as if penned by a human educator. It had a remarkable talent for breaking down complex ideas while keeping all the essential details intact.

Copilot: As an integrated tool, its biggest perks were speed and convenience. The quality was on par with ChatGPT, given that it’s built on similar models. It was lightning-fast for whipping up quick summaries but also managed to tackle more intricate prompts with ease.

## Coherence

<img width="1400" height="452" alt="image" src="https://github.com/user-attachments/assets/8a094875-8be7-4aa3-842f-09c891e51530" />

Logical Flow and Progression of Ideas: A coherent summary lays out information in a way that makes sense. It doesn’t have to mirror the order of the original article. Instead, the ideas should connect and build on each other seamlessly. For instance, a poor flow might look like this: starting with the security of blockchain, then defining what a block is, jumping to its role in cryptocurrency, and finally explaining what a ledger is. While the information is present, the reader is left to piece it together like a jigsaw puzzle.

On the flip side, a good flow would start with the basic idea (a digital ledger), then move on to how information is organized into "blocks," how these blocks link together to form a "chain," and finally, how this structure ensures security and trust. This approach follows a logical path from the general to the specific.

Clarity of Connections (The "Glue"): This aspect focuses on how well sentences and paragraphs relate to each other. Coherent writing employs transitional words and phrases to illustrate the relationships between ideas, allowing the text to flow smoothly rather than reading like a disjointed list of facts. For example, a lack of connection might be: "Blockchain is a distributed ledger. Every transaction is a block. Hashing makes it secure."

In contrast, a connected version would be: "Blockchain is essentially a distributed ledger. The information on this ledger is organized into 'blocks,' which hold transaction details. To maintain security, each block is linked to the previous one through a cryptographic method known as hashing, forming a permanent and unalterable chain."

Unified Focus and Purpose: A coherent summary revolves around a central theme or idea from the original text. It should avoid including irrelevant details or veering off topic. Every sentence should contribute to the main goal of explaining the topic's basics in a straightforward and clear manner. A lack of focus might be a summary that starts with blockchain fundamentals but then gets sidetracked into a detailed analysis of the cryptocurrency market fluctuations in 2021.


## Simplicity

<img width="2932" height="1755" alt="image" src="https://github.com/user-attachments/assets/4948c87a-d04c-427c-8b64-408b5cfd8008" />

Logical Flow and Progression of Ideas: A coherent summary lays out information in a way that makes sense. It doesn’t have to mirror the order of the original article. Instead, the ideas should connect and build on each other seamlessly.

For instance, a poor flow might look like this: starting with the security of blockchain, then defining what a block is, jumping to its role in cryptocurrency, and finally explaining what a ledger is. While the information is present, the reader is left to piece it together like a jigsaw puzzle.

On the flip side, a good flow would start with the basic idea (a digital ledger), then move on to how information is organized into "blocks," how these blocks link together to form a "chain," and finally, how this structure ensures security and trust. This approach follows a logical path from the general to the specific.

Clarity of Connections (The "Glue"): This aspect focuses on how well sentences and paragraphs relate to each other. Coherent writing employs transitional words and phrases to illustrate the relationships between ideas, allowing the text to flow smoothly rather than reading like a disjointed list of facts. For example, a lack of connection might be: "Blockchain is a distributed ledger. Every transaction is a block. Hashing makes it secure."

In contrast, a connected version would be: "Blockchain is essentially a distributed ledger. The information on this ledger is organized into 'blocks,' which hold transaction details. To maintain security, each block is linked to the previous one through a cryptographic method known as hashing, forming a permanent and unalterable chain."

## Speed

Defining "Speed" in Our Workflow: When we talk about speed in this evaluation, we’re looking at more than just how fast the AI churns out text. We’re also considering the entire timeline—from the moment you hit send on your initial prompt to when you have a polished, usable summary in hand. This means factoring in the time spent crafting that prompt, how long the AI takes to respond, and any edits or re-prompts needed to ensure we meet our quality standards.

Raw Generation Speed is a Minor Factor: Across all the platforms we tested—ChatGPT, Gemini, Claude, and Copilot—speed was impressive. It took just seconds to generate a summary from a 500-word article. In terms of processing speed, the differences between these platforms were negligible and didn’t really impact overall efficiency.

Prompt Complexity vs. Overall Speed: We discovered that the effort you put into crafting a prompt and the total time spent on the task are actually inversely related.

Zero-Shot Prompts ("Summarize this"): While this approach was the quickest to type out, it turned out to be the slowest in practice. The generic and often overly technical responses required a lot of manual tweaking or even a complete re-prompt, which added several minutes to our workflow.

Role-Based & Few-Shot Prompts: These prompts took a bit longer to set up—about an extra 30 to 60 seconds—but they delivered nearly flawless summaries on the first go. This significantly cut down or even eliminated the need for any post-generation edits, making them the fastest method from start to finish.

Workflow Integration as a Speed Advantage: The platform that really stood out for situational speed was Copilot. Its ability to integrate seamlessly with other applications, like web browsers or document editors, means you don’t have to waste time switching tabs or copying and pasting text. For quick summarization tasks, this smooth workflow feels the most immediate and efficient.

Conclusion on Speed: Ultimately, true speed is about how quickly the AI can provide a finished product, not just how fast it can type. The most effective strategy involves using a well-crafted, specific prompt, like the Role-Based technique. Investing a little time upfront to clearly articulate your needs is the best way to achieve the results you want.


## User experience

When it comes to the user experience (UX) for a system that utilizes Cross-Platform-Prompting-Evaluating-Diverse-Techniques-in-AI-Powered-Text-Summarization, the focus should be on making it user-friendly, clear, and trustworthy. The goal is to create a smooth interface where users can easily upload documents or audio, enter prompts, view summaries, and assess their quality across various devices and AI models. Essential features for a great UX include handling multiple input types, ensuring accessibility across platforms, providing clear evaluation metrics, and managing prompts effectively. This way, users can make the most of the AI for a variety of summarization tasks.

Key UX Considerations

Intuitive Input & Output:
Cross-Platform Input: Users should be able to upload documents (like PDFs or websites) or audio files from different sources and access the summarized content on any device.
Clear Summary Presentation: Summaries need to be displayed in a way that’s easy to read, concise, and well-organized, clearly differentiating between extractive and abstractive summaries.
Seamless Prompt Engineering:
Programmatic Prompt Management: Implement a toolkit like Promptimize that allows users to define, tweak, and manage prompts as code, making it easier to reuse and experiment across various AI engines.
Dynamic Prompt Variation: Help users create different prompt variations, allowing them to play around with contexts, constraints, and phrasing to enhance the summary output.
Transparent and Actionable Evaluation:
Objective Evaluation Metrics: Incorporate a range of metrics to evaluate the generated summaries and show these scores to users, enabling them to compare different prompt variations objectively.
Performance Reporting: Offer clear, data-driven reports on how prompts perform, helping users understand the quality of the summaries and refine their designs.
User Control and Trust:
Model Selection: If possible, let users choose from different AI models or engines for their summarization tasks, giving them more control over the process.
Feedback Mechanisms: Include ways for users to provide both explicit and implicit feedback, which can be used to further enhance the AI's performance.


## Algorithm

<img width="624" height="374" alt="image" src="https://github.com/user-attachments/assets/ae28dc9c-2e4f-4e25-9983-11a7b0604d0f" />

Establish a Control: We used a single source text for all tests: a 500-word technical article titled "The Basics of Blockchain Technology." Sticking to the same article for every test meant that any differences in output were due to the AI platform or the prompting method, rather than the source material itself.

Define Evaluation Criteria: Before diving in, we laid out five key metrics:

Accuracy: How closely the summary captures the essential facts of the original text.
Coherence: The logical flow and readability of the summary.
Simplicity: The use of straightforward language while steering clear of technical jargon.
Speed: The total time taken from writing the prompt to receiving a final, usable summary.
User Experience: The overall ease and satisfaction of the process.
Design the Prompts: We crafted four distinct prompts, one for each technique, to ensure consistency across all platforms.

Zero-Shot: A straightforward command: Summarize the following text:

Few-Shot: A command that includes an example to follow: Summarize the provided article in a simple, clear style, similar to this example: [A pre-written simple summary was inserted here].

Chain-of-Thought: A prompt that guides the AI's reasoning: First, identify the three main concepts in the article. Next, explain each one in simple terms. Finally, weave these explanations into a coherent summary.

Role-Based: A prompt that assigns a specific persona and audience: Act as a university professor. Summarize the following article for a first-year student who is just starting to learn about this topic.

Execute the Tests: We systematically applied each of the four prompts across the four AI platforms (ChatGPT, Gemini, Claude, Copilot). This resulted in a total of 16 unique summaries for analysis. We timed each interaction to measure the "Speed" criterion.

Analyze and Score: We evaluated the 16 summaries against the five metrics we established. A qualitative rating scale (Poor, Fair, Good, Excellent) was used to maintain consistency in our assessment.

## Result

For the	 team's aim of crafting straightforward and clear summaries for undergraduate students, the best approach is Role-Based Prompting. This method has consistently outshone the rest because it tells the AI to focus on the intended audience, leading to summaries that are not only accurate but also perfectly matched in tone and simplicity.

So, the final suggestion is to make your summarization process revolve around a role-based prompt structure. While platforms like ChatGPT, Gemini, and Claude all excel with this technique, you'll get the best results from a prompt like:

"Act as a university professor. Summarize the following text for a first-year undergraduate student who has no prior knowledge of the topic."

In a nutshell, the secret to success lies not in hunting for the "best" AI, but in mastering how to ask the AI to be the best summarizer for your unique needs.
