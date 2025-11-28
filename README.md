# EX-02-Cross-Platform-Prompting-Evaluating-Diverse-Techniques-in-AI-Powered-Text-Summarization
# EXPERIMENT – 2:
# Evaluation of Prompting Tools Across Diverse AI Platforms: ChatGPT, Claude, Bard, Cohere Command, and Meta

## AIM
To evaluate and compare the effectiveness of prompting techniques (zero-shot, few-shot, chain-of-thought, role-based) across different AI platforms (e.g., ChatGPT, Gemini, Claude, Copilot) in a specific task: text summarization.
# Aim:
To systematically evaluate and compare the performance, user experience, and response quality of multiple AI platforms (ChatGPT, Claude, Perplexity) across different prompting strategies — namely Zero-Shot, Few-Shot, Chain-of-Thought, Role-Based, and ReAct prompting — within a focused mechanical engineering use case (Soft Robotics). The goal is to analyze how each AI tool interprets and summarizes a given technical paragraph (150 words) under various prompting techniques. Each AI's response will be individually assessed for quality, accuracy, and depth using a grading system, with separate notes for each model. The experiment also aims to capture actual model outputs to provide context for the evaluations, ensuring that comparisons are traceable, detailed, and meaningful.

## Scenario:
You are part of a content curation team for an educational platform that delivers quick summaries of research papers to undergraduate students. Your task is to summarize a 500-word technical article on "The Basics of Blockchain Technology" using multiple AI platforms and prompting strategies.
# 📊 Grading Key:
•	A = Excellent
•	B+ = Very Good
•	B = Good
•	C = Adequate
•	D = Poor
•	F = Inadequate

Your goal is to determine which combination of prompting technique + platform provides the best summary in terms of:
# Use Case: Text Summarization
“Soft robotics is an emerging field in mechanical engineering that focuses on creating robots constructed from highly flexible and compliant materials, such as silicones, polymers, and smart textiles. Unlike traditional rigid robots, soft robots are designed to safely interact with humans and adapt to unpredictable environments. They often mimic biological organisms, offering advantages like enhanced dexterity, safe physical interaction, and the ability to squeeze through confined spaces. Recent advancements include artificial muscles powered by pneumatics, hydraulics, or electroactive polymers, enabling more lifelike and versatile movement. Soft robotic grippers are now widely used in delicate object handling, such as food processing and medical surgery. Researchers are also exploring untethered soft robots that can crawl, swim, or even heal themselves after damage. The combination of material innovation, bioinspired design, and intelligent control systems positions soft robotics as a transformative force across healthcare, wearable technology, aerospace, and beyond.”

Accuracy
# 1.	Prompt Type: Zero-Shot Prompt
Question: "Summarize the paragraph about soft robotics."
🔹 ChatGPT: "Soft robotics focuses on building flexible, adaptable robots from materials like silicones and smart textiles. These robots mimic biological organisms, enhancing safety, dexterity, and adaptability. Innovations include artificial muscles, soft grippers for delicate tasks, and self-healing robots. Applications span healthcare, aerospace, and wearable technology."

Coherence
🔹Claude: "Soft robotics is a new mechanical engineering field creating flexible robots from materials like polymers and textiles. These robots are safe for human interaction, inspired by biological systems, and useful in confined spaces. Innovations include artificial muscles and self-healing designs, with applications in healthcare, manufacturing, and aerospace."

Simplicity
🔹 Perplexity: "Soft robotics is advancing mechanical engineering by using flexible materials like polymers and textiles to create adaptive robots. They mimic biological systems, making them ideal for interacting with humans and delicate objects. Key innovations include artificial muscles and untethered robots that can self-heal, impacting fields like healthcare and wearable tech."

Speed
# Analysis Notes (Zero-shot):

User experience

## Algorithm
# 2.	Prompt Type: Few-Shot Prompt
Question: The paragraph given for text summarization will be summarized as the example give below.
Example:
Summarize this paragraph:
“Quantum computing uses quantum bits (qubits) that can exist in multiple states simultaneously, allowing for much faster computations in specific tasks compared to traditional computers. It holds potential for breakthroughs in cryptography, material science, and optimization problems.”
# Summary:
"Quantum computing uses qubits to enable faster computations and has promising applications in cryptography and material science."
🔹 ChatGPT:
"Soft robotics uses flexible materials like silicones and polymers to build adaptive robots that can safely interact with humans. They mimic biological forms, enabling movements like crawling and squeezing. Innovations include artificial muscles, self-healing robots, and applications in healthcare, aerospace, and wearable technology."
🔹 Claude: 
"Soft robotics focuses on building robots from flexible materials such as polymers and smart textiles, enabling safe human interaction and adaptability. They mimic biological organisms and are advancing with artificial muscles, self-healing capabilities, and uses in healthcare, food handling, and aerospace."
🔹 Perplexity: 
"Soft robotics is a mechanical engineering innovation using flexible materials to build adaptive, bioinspired robots. Developments like artificial muscles, self-healing designs, and soft grippers enable new applications in healthcare, wearables, and delicate manufacturing tasks."

# Analysis Notes (Few-shot):
AI Tools	Performance	User Experience	Response Quality	Notes
ChatGPT	A	A	A	Comprehensive summary, includes the material, application, and technology well.
Claude	B+	A	B+	Correct examples but less detail in explaining the relationship between them.
Perplexity	B	B+	B	Includes all elements but the connections feel slightly forced.











3.	Prompt Type: Chain-of-Thought Prompt

Question: Follow the below given instructions 
Prompt:
"First, identify the main materials used in soft robotics. Then, describe how these robots mimic biological systems. Next, list recent innovations. Finally, summarize the paragraph about soft robotics."
🔹 ChatGPT:
•	Main materials: Flexible materials like polymers, smart textiles, and soft silicones.
•	Mimicking biological systems: By enabling robots to crawl, squeeze, adapt shapes like living organisms.
•	Innovations: Artificial muscles, untethered robots, self-healing capabilities.
•	Final summary: "Soft robotics uses flexible materials to create adaptive, bioinspired robots, introducing innovations like artificial muscles and self-healing designs for healthcare, aerospace, and wearable applications."
🔹 Claude:
•	Materials: Polymers, soft textiles, other flexible substances.
•	Biomimicry: Robots imitate movements such as squeezing and bending like living creatures.
•	Innovations: Self-healing robots, soft grippers, untethered systems.
•	Summary: "Soft robotics is advancing mechanical engineering with flexible robots that mimic biological systems and introduce features like artificial muscles and self-healing properties, expanding into healthcare and aerospace industries."
🔹 Perplexity:
•	Materials: Soft materials like polymers and textiles.
•	Biomimicry: They replicate biological flexibility and adaptability.
•	Innovations: Soft grippers, artificial muscles, self-healing designs.
•	Summary: "Soft robotics leverages flexible materials to build robots that mimic living systems, enabling safer human interaction and expanding applications in healthcare and manufacturing."

Analysis Notes (Chain-of-Thought):

Model	Performance	User Experience	Response Quality	Notes
ChatGPT	A	A	A	Detailed, structured explanation that builds logically from one point to another.
Claude	A-	A	B+	Good explanation, but slightly less clarity on how steps connect to real-world applications.
Perplexity	B+	B+	B+	Explanation is clear but slightly less detailed in stepwise development.










4.	Prompt Type: Role-based Prompt
Question: Follow the below given instructions 
Prompt:
"You are a Mechanical Engineering Professor specializing in Robotics. Summarize the key developments in the field of soft robotics, highlighting the materials, biological inspirations, and innovations mentioned."
🔹 ChatGPT : 
"As a Mechanical Engineering Professor, I observe that soft robotics is rapidly advancing through the use of flexible materials such as polymers and smart textiles. Inspired by biological systems, these robots mimic movements like crawling and squeezing. Notable innovations include artificial muscles, self-healing materials, untethered robots, and their integration into healthcare, aerospace, and wearable technology sectors."
🔹 Claude: 
"In soft robotics, engineers use materials like polymers and soft fabrics to develop machines that mimic the movements of living organisms, such as squeezing and bending. Recent innovations such as artificial muscles, self-healing designs, and soft grippers have broadened applications into healthcare, aerospace, and food industries. The field reflects a trend towards safer and more adaptable robotic systems."

🔹 Perplexity: 
"Soft robotics, employing flexible polymers and smart textiles, is advancing mechanical systems that mimic biological motions. Key developments include artificial muscles, self-healing robots, and untethered systems, creating new possibilities in healthcare, wearable devices, and delicate manufacturing processes." 



Analysis Notes (Role-based):

Model	Performance	User Experience	Response Quality	Notes
ChatGPT	A	A	A	Clear, authoritative explanation fitting the role of an expert in the field.
Claude	A-	A-	B+	Good technical explanation, but lacks a bit of depth in terms of future impact.
Perplexity	B+	B	B	A bit too generic and lacks the authoritative tone needed for an expert response.


















5.	Prompt Type: ReAct Prompting
Question: Follow the below given instructions
 Prompt:
"First, think about what materials are required for soft robotics. Then reason about how these materials help in mimicking biological systems. Identify recent innovations mentioned. Finally, summarize everything clearly. Think step-by-step."
🔹 ChatGPT:
Step 1: Materials needed include flexible polymers, smart textiles, and soft silicone-based substances.
Step 2: These materials allow robots to adapt shapes, move flexibly, and squeeze like biological organisms.
Step 3: Recent innovations include artificial muscles, self-healing robots, and untethered systems.
Final Summary: Soft robotics leverages flexible, bio-inspired materials to create adaptive systems, with innovations like artificial muscles and self-repairing capabilities that benefit industries like healthcare, aerospace, and wearable technology.

🔹 Claude:
Step 1: Materials are flexible — polymers, fabrics, and soft substances.
Step 2: Flexibility enables robots to replicate crawling, squeezing, and shape-changing behaviors found in nature.
Step 3: Innovations include artificial muscles, self-healing robots, and untethered designs.
Final Summary: Soft robotics is revolutionizing engineering by using flexible materials to build systems that imitate biological organisms and expand robotic applications in healthcare, aerospace, and wearable devices.

🔹 Perplexity:
Step 1: Polymers and smart textiles are the main materials.
Step 2: These enable the soft robots to mimic flexible biological movements.
Step 3: Notable innovations are soft grippers, artificial muscles, and untethered robots.
Final Summary: Soft robotics uses flexible materials to create machines mimicking biology, driving innovation in healthcare and manufacturing fields.

 Analysis Notes (ReAct):

Model	Performance	User Experience	Response Quality	Notes
ChatGPT	A	A	A	Logical reasoning followed by a relevant real-world example (surgery).
Claude	A-	A	B+	Strong reasoning, but the example could be more detailed.
Perplexity	B+	B	B	Good reasoning but the example was weak and less applicable to the industry.


6.	Prompt Type: Instruction-following Prompt
Question: Follow the below given instructions
Prompt:
"Strictly list 5 key developments in soft robotics based on the paragraph. Do not elaborate."
🔹 ChatGPT:
1.	Use of flexible polymers and smart textiles
2.	Development of artificial muscles
3.	Integration of self-healing materials
4.	Creation of untethered, autonomous robots
5.	Expansion into healthcare, aerospace, and wearables

🔹 Claude:
1.	Flexible polymers and soft materials
2.	Artificial muscles
3.	Self-healing robotic components
4.	Untethered robot designs
5.	Applications in healthcare and aerospace

🔹 Perplexity:
1.	Use of polymers and smart materials
2.	Development of artificial muscles
3.	Self-healing robot structures
4.	Autonomous untethered robots
5.	Adoption in wearable tech and healthcare


Analysis (Instruction-following):

Model	Performance	User Experience	Response Quality	Notes
ChatGPT	A	A	A	Follows instructions well, concise and accurate list.
Claude	A-	A-	A-	Good listing but a bit generic; could improve with more specific examples.
Perplexity	B+	B	B+	List format is correct, but some points are not as detailed or relevant.







7.Prompt Type: Context-enriched Prompt
Question: Follow the below given instruction
Prompt:
"Soft robotics is a rapidly evolving subfield of mechanical engineering, inspired by biological organisms and requiring materials that offer flexibility and resilience. Considering this context, summarize the latest material innovations and their impact on robotic capabilities."
🔹 ChatGPT:

"Building on the biological inspirations and need for flexibility, soft robotics has introduced materials like flexible polymers and smart textiles that enable bending, crawling, and squeezing movements. Innovations such as artificial muscles and self-healing systems have enhanced the adaptability, resilience, and autonomy of robots across healthcare, aerospace, and wearable technology fields."

🔹 Claude:
"Given the biologically inspired origins of soft robotics, researchers have focused on materials like polymers and smart textiles. These allow robots to mimic natural movements such as squeezing and adapting shapes. Innovations like artificial muscles and self-healing structures have significantly expanded the versatility of robotic applications in critical industries."

🔹 Perplexity:
"Soft robotics leverages flexible polymers and fabrics inspired by biological systems to enhance movement. New developments like artificial muscles and self-healing robots have made robots more resilient and suitable for industries such as healthcare and aerospace."


Analysis (Context-enriched):

Model	Performance	User Experience	Response Quality	Notes
ChatGPT	A	A	A	Well-structured response with a detailed explanation linking flexibility and precision to recovery time.
Claude	A-	A	B+	Good explanation but less connection to the specific benefits of flexibility and precision.
Perplexity	B+	B	B	Provides good context but lacks in-depth analysis of how soft robotics can reduce recovery time.


Result:
Summary of Experiment Results:
In this experiment, various AI models (ChatGPT, Claude, and Perplexity) were evaluated on their performance, user experience, and response quality across multiple prompting types (Zero-shot, Few-shot, Chain-of-thought, Role-based, ReAct, Instruction-following, and Context-enriched). The task involved evaluating their ability to answer technical questions related to soft robotics in mechanical engineering, specifically how soft robotics innovations can aid in reducing recovery time in surgical applications.
Key Findings:
1.	ChatGPT:
o	Overall Winner: Consistently provided the most detailed, coherent, and accurate responses across all prompt types. ChatGPT demonstrated the highest level of flexibility in adapting to different question formats and providing insightful answers with adequate technical depth.
o	Best Performance: In Chain-of-thought, Context-enriched, and Instruction-following prompts, where clear and structured responses were necessary.
2.	Claude:
o	Second Best: Claude performed well, especially in Instruction-following and Context-enriched prompts, but lacked the depth and coherence of ChatGPT in some complex technical questions. In cases where more detailed analysis was required, Claude occasionally provided answers with less specific examples or a less clear connection to the question at hand.
o	Strength: Its ability to provide structured responses but with occasional shortcomings in deeper explanations.
3.	Perplexity:
o	Third Place: Perplexity often delivered adequate responses but showed inconsistent performance, especially in detailed technical discussions. It sometimes failed to provide responses that were both coherent and relevant to the question's core, especially in context-rich or role-based prompts.
o	Limitations: The responses from Perplexity lacked in-depth technical reasoning and often missed out on connecting key points that were necessary for a complete answer.





Prompt Type Performance Comparison:

Prompt Type	ChatGPT	Claude	Perplexity
Zero-shot	A	A-	B+
Few-shot	A	B+	B
Chain-of-thought	A	A-	B+
Role-based	A	A-	B+
ReAct	A	A-	B
Instruction-following	A	A-	B+
Context-enriched	A	B+	B

•	ChatGPT earned A grades in nearly every category, excelling in coherence, depth, and accuracy. Its responses were highly structured, making it a powerful tool for handling both broad and technical questions.
•	Claude performed well, earning A- grades in most categories, but it occasionally lacked the necessary depth in complex technical explanations.
•	Perplexity scored the lowest across the board, with B grades, indicating its struggles in handling detailed, technical content while maintaining coherence in responses.

Overall Observations:
•	ChatGPT demonstrated the best overall consistency in both technical depth and clarity, making it the ideal model for handling complex, technical topics like soft robotics.
•	Claude provided competent responses, though sometimes falling short of ChatGPT in depth, especially for technical topics that required a more nuanced understanding of engineering concepts.
•	Perplexity, while offering helpful answers, struggled the most with complexity and coherence, making it less suitable for tasks that require high-level technical reasoning or detailed explanations.

Conclusion:
The experiment successfully illustrated the comparative strengths and weaknesses of different AI models when responding to prompts of varying complexity. ChatGPT stood out as the top performer, followed by Claude, with Perplexity lagging behind in technical tasks. The findings underscore the importance of choosing the right AI model based on the type of question and the level of technical complexity involved.
For applications in mechanical engineering, specifically related to soft robotics, ChatGPT would be the most reliable tool due to its ability to provide clear, accurate, and detailed responses, while Claude could be a useful backup for less complex tasks. Perplexity, despite its utility in simpler contexts, would need further refinement for technical engineering tasks.

## Result
Claude with chain-of-thought prompting produced the most accurate and structured summaries.
ChatGPT performed well with few-shot prompting, balancing clarity and relevance.
Copilot and Gemini were fast but less nuanced, especially in zero-shot and role-based modes.

