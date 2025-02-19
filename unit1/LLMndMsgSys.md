# LLM and Message System

Decoder based transformer models that can **understand human language and generate content**
Transformer model size with billions of parameters.

Underlying principle of LLM - "objective to predict next token,given a series of previous tokens."
Token - smallest unit of information an LLM works with.

Each LLM will have some special tokens to indicate end of message/instruction text.
The LLM uses these tokens to open and close the structured components of its generation
Also, input query will also contain these special tokens for structuring.

You can find special tokens configuration of a model in tokenizer_config.json

LLMs are autoregressive (output of previous pass is the input of next pass for next word prediction) this next word prediction process till EOS.

## Role of LLM in AI Agent

LLM is **key** component of AI Agents, it provides the foundation for understanding and generating human language.

LLM is used to understand and interpret the user instructions, define a plan and decide what tools to use. LLM is brain of the agent.

## Messages and Special Tokens

How the LLM structure their generations through chat templates.
LLM- conversational chatbot - exchange of messages -- behind UI abstraction
    Conversation messages are concatenated and formatted into a prompt that the model can understand

![PromptImg](/unit1/prompt_message_concat.png)

System message:
    Persistant instruction to system.
    Also called as system prompt - defines how the model should behave.
    In agents system prompt will also include information about list of available tools and provides information about how to format actions to take
    and guidelines of how the thought process should be segmented.

Conversation - role - user/assistant, content - chat message from the respective person/entity. 

Chat Templates - structing conversation between user and LLM.

Two different types of model in AI Agent - Base model and Instruct Model.
    Base Model - Trained on raw text to predict next token. 
    Instruct Model - Specifically trained to follow instructions and engage in conversation.

To make base model understand like instruct model - Use chatML chat markup language  - format our prompts in a consistent way that the model can understand.

ChatML completion - Code completion, Few shot learning, Text summarization

Messages to Prompt - AutoTokenizer apply_chat_template method , previously - model selected - HuggingFaceTB/SmolLM2-1.7B-Instruct" add_generation_prompt = true,tokenize=False