# Understanding AI Agents through the Thought-Action-Observation Cycle

Thought, Action, Observe cycle Example:
Thought - Prior system_message with detail on available tools for it to use the AI Agent on user prompt when decides to take action -
It first finds what available tool it can use -- example get_weather API call
Creates API call specification with inputs in JSON
Calls the get_weather API to get results
Observes the API call and respond user back in natural language.
Agents iterate through a loop until the objective is fullfilled.

## The Re-Act approach-

    A key method is the ReAct approach, which is the concatenation of “Reasoning” (Think) with “Acting” (Act).
    Generate **plan** instead of next token.
    Model is decomposing the problem to sub-problems.
    Reflect on past experiences
    Continuously adjust plan based on new information.
    These models have been trained to always include specific thinking sections (enclosed between <think> and </think> special tokens).
    This is rather a training approach where the model learns to generate these sections after analyzing thousands of examples.

    If LLM's are finetuned for function-calling thought process is optional. 
Thought on AI Agents - Agent's internal reasoning and planning processes to solve the task.

DeepSeek R1 / Open AI o1 - ReAct Approach - think before answering (Models are included with specific think instructions)
