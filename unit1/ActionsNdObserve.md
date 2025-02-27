# Actions and Observation

AI agents concrete steps taken to interact with the environment.
Types of agents
    1. Code Agent - Action writes a code block that is interpreted externally.
    2. JSON Agent - Action to perform is specified in JSON format.
    3. Function calling Agent - Subcategory of JSON agent - fine-tuned to generate a new message for each action.

Action - Types

   1. Information gathering - like web_search / querying database / retrieving documents
   2. Tool usage - API calls/ Running calculation/ Execute code
   3. Environment interaction - Work with controlling physical devices or digital interfaces.
   4. Communication - Engaging with users - chatbot or collaborating with multiple agents.

Ability of Agent - STOp when the action is complete.
Stop and parse approach - To ensure the AI agent action is precise and ready for external processing.

## Observation

Observations are how an Agent perceives the consequences of its actions.
AI Agents observe the signals from environment - APi response/ error message in system/ system logs - fuels next cycle of thought
    AI Agents does the following in observation phase-
       Collects Feedback
       Append Results
       Adapt it's strategy
How are results appended on agent's memory
       Parse action
       Execute action
       Append results in observation
