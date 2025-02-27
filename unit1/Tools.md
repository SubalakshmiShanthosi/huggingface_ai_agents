# Tools in AI Agent

A tool is a function given to LLM. The function should fulfill a clear objective.
Example tools - web_search, image generation, retrieval, API interface (ext API interaction ex: spotify/youtube/github)

Actual LLM model trained with prior data - would answer and reason with it's own knowledge (might hallucinate if it's not on top of the current situation data)
Example - Consider an LLM model is asked with detail on How it's the weather today at location X? LLMs predict the completion of a prompt based on their training data, but for up-to-date information sync - you need tool (web_search)
    Without web_search only LLM model (i.e without tools) - Hallucinate- predict weather that doesn't align to current weather
    Agent that has web_search tool - Gives proper accurate weather information.

What all information does the Tool need?
    1. A textual description of what this tool does
    2. A Callable(something to perform action)
    3. Arguments with typings
    4. (Optional) Output with typings

Previous example of using web_search tool weather to give accurate weather information for user ask -
    LLM will generate text in form of code, to invoke the tool

Example instruction in system_message
    You will have access to the following tools:
    {tools_Description}

Precise and accurate description of - what functionality the tool does and the exact inputs to the tool - JSON format
Auto-formatting Tool sections is also possible instead of providing textual description of what tool does and what input it expects.
Programmatically describe what the tool does, what input it expects - @tool decorator python function code for tool

Breakdown of generic tool class
    1. tool name
    2. tool description
    3. tool callable (functions)
    4. arguments (inputs to the tool)
    5. outputs (expected output of the tool)
