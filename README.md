Email Agent
Email Agent is an intelligent assistant designed to handle incoming email messages by understanding the content and responding with appropriate, context-aware replies. It leverages OpenAI's function calling and message history management to maintain conversation coherence.

Features
Automatically understands and replies to email content.

Uses OpenAI's function-calling system for intelligent decisions.

Maintains context across multiple messages.

Designed for integration into broader email workflows.

How It Works
The agent uses the following tools and memory strategies:

Function Calls: Defines actions like email_reply that return structured replies.

Memory: Maintains recent message history using a chat_history memory type with message_window for limited context retention.

Prompting: The agent is instructed to always reply as if responding to an email, using professional tone and formatting.

Technologies Used
OpenAI API (function calling)

JSON-based agent configuration

Custom prompt engineering
