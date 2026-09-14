ReAct Agents | Tool use and collaboration

Three Python agents exploring how a language model can request tools, use their
results and participate in a shared chat. Built as Assignment 2 during AI and
machine learning studies.

Stack: Python · OpenAI API · JSON · subprocess · REST APIs

Choose an example

Agent

What it demonstrates

Requirements

Part 1

A text-parsed agent loop with approved shell commands

OpenAI API key

Part 2

JSON-directed tool requests, file edits and conversation history

OpenAI API key

Part 3

Mentions, PASS decisions and bounded collaboration in a shared chat

OpenAI API key and access to a compatible hub

Start with Part 2: its included test_project/example.py contains an
intentional addition bug. Ask the agent to inspect it, approve the proposed edit,
and inspect the verification output. The walkthrough below describes the
expected interaction; model responses can vary.

Scope and limitations

This is an educational implementation. Parts 1 and 2 execute approved commands
on your machine; the string blocklist is not a sandbox. File-path checks do not
resolve symbolic links, and Part 2 requests JSON through its prompt rather than
validating responses against a complete tool schema.

Part 3 proposes code in chat; it does not apply that code to a shared repository.
The included bug example is a demonstration fixture, not an automated test suite.
