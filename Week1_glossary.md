Week 1 Glossary: AI Foundations for High School Students
Welcome to the Week 1 Glossary! This guide is created especially for high school students. We have stripped away the dry academic jargon and replaced it with fun, real-world examples, interactive analogies, and easy-to-follow explanations.

Every term in this glossary connects directly to the stories, characters, and code experiments from your Week 1 lessons and Code Labs!

1. Episode 1: The Prediction Engine (Probability & Neural Networks)
Probability (Confidence Score)
Intuitive Definition: A decimal number between 0 and 1 (which works exactly like a percentage from 0% to 100%) that shows how sure the AI is that something will happen. 0 means "no way," and 1 means "absolute promise!"
Curriculum Analogy: In Video 1, TikTok's recommendation engine calculates a confidence score (like 0.85, or 85% sure) that you will watch a funny cat video all the way through. If that score is high enough, the video pops up on your "For You" page!
Curriculum Context: Week 1, Video 1 (Main Explainer), Scene 2
Baseline Probability
Intuitive Definition: A basic, simple guess of how likely something is to happen, based only on overall history, without looking at the current context or order of events.
Curriculum Analogy: In Video 1 Code Lab, the calculate_probabilities function looks at Kwame's daily log and finds that he spends 40% of his entire life sleeping. It can guess that there is a 40% chance Kwame is sleeping at any random moment, but it has no idea when he will sleep because it ignores what time it is or what he did right before.
Curriculum Context: Week 1, Video 1 (Code Lab), Part 2
Conditional Probability
Intuitive Definition: The chance of an event happening only because something else just happened first. It's all about context and sequence!
Curriculum Analogy: In Video 1 Code Lab, the calculate_conditional_probabilities function builds a Markov Chain transition matrix (a sequence tracking map). It reveals that if Kwame is currently doing Exercise, he has a 90% chance of doing Leisure (resting/showering) next, but almost a 0% chance of transitioning straight back to Work.
Curriculum Context: Week 1, Video 1 (Code Lab), Part 2
Perceptron (The AI's Basic Decision Maker)
Intuitive Definition: The absolute simplest building block of an AI's brain. It acts like a virtual scale: it takes in several clues (inputs), multiplies each clue by how important it is (weights), adds a little baseline nudge (bias), and if the total weight tips the scale past a threshold, it fires a "YES!" signal.
Curriculum Analogy: Video 1 uses the "bricks and blueprints" analogy. Just like a real brain cell (neuron) passes tiny electrical shocks to its neighbors when excited, a mathematical perceptron sums up its weighted signals to decide whether to "fire" its prediction.
Curriculum Context: Week 1, Video 1 (Main Explainer), Scene 3
Sigmoid Activation (The Math Squisher)
Intuitive Definition: A handy mathematical formula that takes any giant or tiny number and gently squashes it into an S-shaped curve between 0 and 1. It turns raw, messy math scores into clean probability percentages.
Curriculum Analogy: In the Video 1 Code Lab, the Sigmoid function (1 / (1 + np.exp(-x))) takes the massive output numbers from our neural network and squishes them down so we get a neat, readable 0% to 100% confidence score.
Curriculum Context: Week 1, Video 1 (Main Explainer), Scene 4 & Video 1 Code Lab, Part 3
Gradient Descent & "The Magnetic Effect"
Intuitive Definition: The step-by-step game of "hot or cold" that an AI plays to adjust its weights, slowly fixing its mistakes until its predictions match reality.
Curriculum Analogy: Video 1 explains this with the "Magnetic Effect" visual. Imagine a virtual avatar representing your tastes (your Digital Twin) floating in space. Every time you watch a soccer video, a positive magnet pulls your twin closer to the soccer coordinates. When you skip a makeup tutorial, a negative magnet pushes your twin away. These tiny magnetic pulls are gradient descent in action—nudging parameters closer and closer to what you actually love.
Curriculum Context: Week 1, Video 1 (Main Explainer), Scene 4
Digital Twin (Your AI Avatar)
Intuitive Definition: A virtual mathematical copy of a user’s habits, speech style, and personality, stored as coordinate points in a giant multi-dimensional grid.
Curriculum Analogy: In Video 1, Kwame’s Digital Twin starts out as a simple dot on a graph tracking whether he likes work or leisure. By the time we reach Video 5, this twin has evolved into a fully functional conversational agent that can talk to his friends exactly like he does!
Curriculum Context: Week 1, Video 1 (Main Explainer), Scene 1 & Scene 4

3. Episode 2: Turning Words into Math (LLM Anatomy)
Tokenization & Subword Tokenizers (Chopping Text)
Intuitive Definition: The process of slicing sentences into bite-sized puzzle pieces called "tokens" (which can be whole words, subwords, or single letters) so the computer can convert text into number codes.
Curriculum Analogy: Modern models use subword tokenization. If you give an AI the rare word pretraining, it doesn't panic with an "I don't know that word!" error. Instead, it chops it up into familiar puzzle pieces it does know: pre + train + ing.
Curriculum Context: Week 1, Video 2 (Main Explainer), Scene 2
Byte Pair Encoding (BPE) (The Word-Builder Game)
Intuitive Definition: An algorithm that builds a model's dictionary by starting with single letters and repeatedly gluing together the most common pairs of characters it sees in millions of books and web pages.
Curriculum Analogy: Video 2 teaches us that LLMs use BPE to construct a master vocabulary of about 100,000 subword puzzle pieces. This strikes a perfect balance: the dictionary is small enough to run super fast, but smart enough to spell out almost any sentence in the world.
Curriculum Context: Week 1, Video 2 (Main Explainer), Scene 2
Embeddings (The Word Galaxy)
Intuitive Definition: A giant, invisible multi-dimensional map where every word in the dictionary is placed as a coordinate point. Words with similar meanings are packed close together, while unrelated words are lightyears apart.
Curriculum Analogy: In Video 2, we visualize this as a Word Galaxy. The word apple floats right next to orange and banana in the "Fruit Solar System," but lives incredibly far away from microchip and transistor in the "Electronics Quadrant."
Curriculum Context: Week 1, Video 2 (Main Explainer), Scene 3
Vector Arithmetic (Map Math)
Intuitive Definition: Doing addition and subtraction directly on coordinate points in our Word Galaxy to discover hidden relationships between words.
Curriculum Analogy: Video 2 displays the ultimate classic formula: $\text{King} - \text{Man} + \text{Woman} = \text{Queen}$. By taking the coordinate for "King," traveling backward along the direction of "masculinity" (subtracting Man), and walking along the path of "femininity" (adding Woman), you land directly on the coordinate point for "Queen"!
Curriculum Context: Week 1, Video 2 (Main Explainer), Scene 3
Cosine Similarity (The Compass Alignment)
Intuitive Definition: A way to check how closely two arrows on our word map are pointing in the same direction, returning a score from -1 (pointing completely opposite ways) to 1 (pointing the exact same way). It ignores how long the arrows are and focuses entirely on their angle.
Curriculum Analogy: In Video 2 Code Lab, cosine similarity is calculated to see if Kwame’s latest texts point in the same direction as his target interests. If his text vector aligns perfectly with the "Tech Interest Vector," the similarity score is close to 1.0, proving he's currently talking about coding!
Curriculum Context: Week 1, Video 2 (Code Lab), Part 2
Principal Component Analysis (PCA) (The 3D-to-2D Shadow Game)
Intuitive Definition: A math trick used to squash complex, high-dimensional data maps (like a 100-dimensional word map) down to a flat 2D page so humans can look at it on a normal screen.
Curriculum Analogy: Think of PCA like holding a 3D wire sculpture of a dinosaur in front of a flashlight. The shadow cast on the flat classroom wall is a 2D picture that still lets you recognize the dinosaur. In Video 2 Code Lab, PCA squashes 100D word vectors onto a flat Matplotlib scatter plot.
Curriculum Context: Week 1, Video 2 (Code Lab), Part 3

5. Episode 3: The "Brain" — Understanding Context (Transformer & Attention)
The Static Embedding Context Problem (The "Bank" Confusion)
Intuitive Definition: The annoying limitation of older AI models where every word gets exactly one unchangeable coordinate point on the map, meaning words with multiple meanings get completely jumbled together.
Curriculum Analogy: Video 3 focuses on the word bank. In the phrase river bank (nature), and deposit bank (money), older static models gave bank the same exact coordinate point, leaving the AI hopelessly confused about whether you were going fishing or depositing a check.
Curriculum Context: Week 1, Video 3 (Main Explainer), Scene 1 & Scene 4
Self-Attention (Using Neighbor Clues)
Intuitive Definition: The magic superpower of the Transformer engine that allows words in a sentence to look at their neighboring words, figure out who is relevant, and temporarily shift their positions on the word map to fit the context.
Curriculum Analogy: Self-attention rescues the word bank! When reading river bank, the word bank stares at river, realizes we are outdoors, and temporarily shifts its coordinate away from financial banks and into nature territory.
Curriculum Context: Week 1, Video 3 (Main Explainer), Scene 2
Queries, Keys, and Values (QKV) (The Library Metaphor)
Intuitive Definition: The three distinct roles words play during self-attention to share clues with each other:
Query ($Q$): The word's search request ("Here is what I'm looking for!").
Key ($K$): The word's index label or tag ("Here is my topic description!").
Value ($V$): The word's actual content ("Here is my information once we match!").
Curriculum Analogy: Video 3 uses the Library Search Metaphor. Imagine you walk into a library with a search topic (Query). You look up index cards (Keys) in the card catalog. When you find the key card that matches your query, you go retrieve the actual textbook content (Value).
Curriculum Context: Week 1, Video 3 (Main Explainer), Scene 2
Softmax Saturation & The Scaled Factor ($\sqrt{d_k}$)
Intuitive Definition: A math guardrail that prevents the numbers inside the self-attention formula from getting so huge that the AI stops learning during its training.
Curriculum Analogy: In Video 3, when Query and Key vectors multiply in high dimensions, their scores can explode. This causes the Softmax math function to flatline, freezing training updates. To keep things stable, we divide (scale) the scores by the square root of the key dimension ($\sqrt{d_k}$) to keep the numbers in a safe, dynamic learning zone.
Curriculum Context: Week 1, Video 3 (Main Explainer), Scene 3
Attention Heatmap (The Grid of Gazes)
Intuitive Definition: A colorful grid chart that visually reveals exactly which words in a sentence are "staring" at each other to understand context.
Curriculum Analogy: In the Video 3 Code Lab, students plot heatmaps using a Yellow-Orange-Red palette. A bright red box on the grid shows that the word it is staring intently at the dog from earlier in the sentence, visually proving the AI understands pronoun references!
Curriculum Context: Week 1, Video 3 (Code Lab), Part 3
Multi-Head Attention (The Team of Specialists)
Intuitive Definition: Running several attention calculations in parallel at the same time, allowing the AI to analyze a sentence from multiple linguistic angles simultaneously.
Curriculum Analogy: Video 3 shows three heads dividing and conquering. Head 1 (The Grammarian) studies syntax (which verbs connect to nouns). Head 2 (The Pronoun Detective) tracks coreference (connecting he or she to the right person). Head 3 (The Topic Scout) tracks the general theme of the sentence.
Curriculum Context: Week 1, Video 3 (Main Explainer), Scene 4

7. Episode 4: Talking to the Machine (Prompt Engineering)
Prompt Stack (The Instruction Sandwich)
Intuitive Definition: A structured sandwich of rules, character sheets, user logs, and chat histories bundled together and sent to the LLM to trigger a perfectly customized and accurate response.
Curriculum Analogy: In Video 4, Kwame constructs a prompt stack containing his custom Digital Twin guidelines, his historical activity files, and his friend's new text message to generate a tailored chat reply.
Curriculum Context: Week 1, Video 4 (Code Lab), Intro & Step 4
Zero-Shot vs. Few-Shot Prompting (No Examples vs. Showing Examples)
Intuitive Definition:
Zero-Shot: Asking the AI to perform a task with direct commands but absolutely zero examples of how the output should look.
Few-Shot: Showing the AI 2 or 3 completed examples of the exact input-output format you want, activating its rapid pattern matching.
Curriculum Analogy: In Video 4, telling an AI "give me Kwame's data in JSON format" (Zero-Shot) often results in a messy text response that breaks your code. But pasting three clean JSON examples first (Few-Shot) triggers the LLM's pattern matching, making it output flawless JSON syntax every single time.
Curriculum Context: Week 1, Video 4 (Code Lab), Step 2
Chain-of-Thought (CoT) Prompting (Thinking Out Loud)
Intuitive Definition: Adding simple triggers like "Think step by step" to your prompt, forcing the AI to write out its intermediate logic before outputting its final answer.
Curriculum Analogy: Video 4 explains that when an AI is forced to write out its thoughts, those intermediate tokens act as a temporary scratchpad memory inside the Transformer's attention window. This prevents the model from rushing to a premature (and often incorrect) guess.
Curriculum Context: Week 1, Video 4 (Code Lab), Step 3
System Instructions Block (The Character Sheet)
Intuitive Definition: The master instructions set at the very start of a chat that locks the AI into a specific role, personality, and rule set.
Curriculum Analogy: In Video 4, Kwame builds a 4-part system block for his Digital Twin:
ROLE: Setting up the persona (Kwame's digital clone).
KNOWLEDGE: What facts the model is allowed to know.
CONSTRAINTS: Crucial boundaries (e.g., "Decline questions unrelated to Kwame's life" and "Never pretend to be a human").
TONE: Ensuring the AI speaks with a friendly, mentor-like voice.
Curriculum Context: Week 1, Video 4 (Code Lab), Step 4

8. Episode 5: Free APIs & Integration (Live Deployment)
REST API Call (The 5 Key Phone Call Elements)
Intuitive Definition: A standardized way for your local computer code to "call" a powerful AI brain sitting on a server farm far away. Every call requires five things:
Base URL (The Phone Number): Where the server is located on the web.
Authentication Key (The Passcode): Your secret API key to verify your account.
Request Headers (The Call Metadata): Information specifying that you are sending JSON data.
Model ID (The Model Choice): Which specific AI model you want to speak with (like llama-3.3-70b-versatile).
Payload (The Message): The actual prompt stack containing your chat.
Curriculum Context: Week 1, Video 5 (Code Lab), Step 1
Statelessness (The Goldfish Server)
Intuitive Definition: A rule of web APIs where the server instantly forgets who you are the millisecond it sends back an answer. Each text is treated as if you are meeting for the very first time.
Curriculum Analogy: Because the Groq and Gemini APIs are stateless, you can't just text "Who am I?" and expect the server to remember your previous texts. To hold a multi-turn conversation, the client-side code must manually append all previous messages into a growing list and re-send the entire history on every single turn!
Curriculum Context: Week 1, Video 5 (Code Lab), Step 4
Object-Oriented Wrapper (GroqClient) (The Universal Remote)
Intuitive Definition: Writing a simple, reusable Python class that hides all the messy network, payload, and header code behind one clean button.
Curriculum Analogy: In Video 5 Code Lab, students write the GroqClient wrapper. Instead of writing 20 lines of complex HTTP payload requests every time they want to chat, they write a simple .chat_completion() method that wraps all the messy plumbing inside.
Curriculum Context: Week 1, Video 5 (Code Lab), Step 3
Hallucination (AI Daydreaming)
Intuitive Definition: When an AI model generates highly confident, grammatically beautiful sentences that are completely made up and false.
Curriculum Analogy: The Facilitator's Guide warns that digital twins can easily hallucinate fake stories about Kwame's meetings or homework if they are not strictly bounded by real-time facts in the prompt stack.
Curriculum Context: Week 1, Facilitator Guide Module 1.5
Co-Occurrence Bias (Stereotype Echoes)
Intuitive Definition: An algorithmic bias where the AI copies common word associations it saw in its training texts, frequently repeating human cultural stereotypes.
Curriculum Analogy: The Facilitator's Guide reminds us that LLMs are next-token probability engines. If historic internet data frequently pairs certain jobs with specific genders, the AI will default to those combinations. We must use tight System Instructions constraints to actively prevent this bias from infecting our customized digital twins.
Curriculum Context: Week 1, Facilitator Guide Module 1.5
