# Unit 1 - Introduction to AI Agents

Understanding Agents:
    What is an AI Agent? how does it work?
    How AI Agents make decisions using reasoning and planning?

Role of LLM in Agents:
    LLM Brain of Agents under hood
    LLM - Conversation structuring via Messages.

Tools and Action
    How Agents communicate with other external tools in the environment.
    How to build and integrate tools for your agents.

Steps taken by Agent while serving User Request

         Example: Agent Alfred
            Step 1 : For the user request, REASON and PLAN
            Step 2: Act/"Execute" using tools (or multiple tools) which Alfred has
            Step 3: Present the results to user

What is an AI Agent

    An Agent is a system that leverages an AI model to
    interact with its environment in order to achieve a user-defined objective. 
    It combines reasoning, planning, and the execution of actions (often via external tools) to fulfill tasks.

Think of AI having
    [a] Brain (AI Model) - All thinking happens - handles reasoning and planning, this part decides what action to take based on situation.
    [b] Body (Capabilities and tools) - This part represents everything (scope of possible ACTIONS) the agents is equipped to do.

AI Agent -- What type of AI models are used
    LLM - Works to generalise the outcome well as it is trained to understand large text corpus.
    VLM - LLM but can understand image inputs

LLM hits appropriate tools to provide outcomes other than textual content.

**Design of tools is very crucial for determining the quality of the agent.**

Example tool: web_search

Example AI Agent --: Personal Virtual Assistants --> understand user query and context, Try to map data from databases and knowledge base and present the result to the user. Or use other tools depending upon the ask - example: schedule some meeting or controlling smart devices

Customer care center chatbot - Find out the issue reported by customer from query, guide users through troubleshooting steps, open issues - internal databases or complete transactions.

AI Non-playable character in games --> Responds in different ways based on context and adapt to player interactions.

AI Agents summary
    1. Understand natural language - Interpret and respond to users in a meaningful way.
    2. Reason and plan - Analyze information, make decisions and devise strategies to solve problem.
    3. Interact with it's environment - Gather information, take actions and observe the results of the action.
