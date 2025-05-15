# ChatVQL  Velociraptor Conversational VQL Agent

## Overview

ChatVQL is a project that aims to develop a conversational AI system, similar to ChatGPT, but with deep specialization in the **Velociraptor Query Language (VQL)**. The primary goal of ChatVQL is to provide an intelligent and interactive interface that allows users to harness the power of Velociraptor for endpoint monitoring, digital forensics, and incident response (DFIR) — without requiring extensive prior knowledge of VQL syntax.

This tool aims to address the current gap where general-purpose AI models lack sufficient training and accuracy with VQL due to the limited availability of comprehensive, structured documentation in their training datasets.

## The Problem

Velociraptor is an advanced DFIR tool that uses VQL to perform powerful queries and actions across fleets of endpoints. However:

* **Steep Learning Curve:** Mastering VQL can be challenging and time-consuming, especially for newcomers.
* **Limited AI Assistance:** Existing large language models (LLMs) like ChatGPT often provide inaccurate or incomplete VQL queries due to insufficient exposure to VQL nuances and the breadth of its plugins and artifacts.
* **Inefficient Query Formulation:** Users might spend considerable time consulting documentation or a trial-and-error process to construct the correct VQL queries for their specific needs.

This ultimately hinders the speed and efficiency with which security professionals and forensic analysts can respond to incidents or hunt for threats.

## The Solution: ChatVQL - An Agentic Workflow

ChatVQL will introduce an **agentic workflow** for VQL, enabling users to interact with Velociraptor through natural language. Instead of writing VQL, users will describe their goals or the information they seek in plain text. ChatVQL will then act as an intermediary:

1.  **Natural Language Understanding:** Interpret the user's request expressed in plain language.
2.  **VQL Translation:** Convert the user's intent into one or more syntactically correct and contextually appropriate VQL queries.
3.  **Multi-Action Capabilities:** Perform a sequence of VQL queries if the user's request requires multiple steps or data points.
4.  **User Authorization & Control:** Present the generated VQL queries to the user for review and explicit authorization before execution.
5.  **Velociraptor Integration:** (With user permission) Securely connect to the user's Velociraptor server to execute the authorized VQL queries.
6.  **Results Presentation:** Retrieve and present the results from Velociraptor in a clear and understandable format.

This "human-in-the-loop" agentic approach ensures that users retain control while benefiting from AI-driven VQL generation and execution.

## Key Features

* **Natural Language to VQL:** Translate plain text requests into effective VQL queries.
* **Agentic Multi-Step Operations:** Capable of orchestrating multiple VQL queries to fulfill complex user requests.
* **Interactive Query Refinement:** Allow users to clarify or modify requests to tune the generated VQL.
* **Velociraptor Server Interaction:** Securely execute queries on a Velociraptor server with user consent.
* **Educational Tool:** Help users learn VQL by showing them the queries generated from their natural language requests.

## Roadmap (Preliminary)

* [ ] **Phase 1: Core VQL Translation Engine**
    * [ ] Develop initial NLP model for understanding VQL-related requests.
    * [ ] Implement basic natural language to VQL translation for common queries.
    * [ ] Build a comprehensive VQL knowledge base for the RAG system.
* [ ] **Phase 2: Agentic Capabilities & User Interaction**
    * [ ] Develop logic for multi-step query execution.
    * [ ] Implement user authorization workflow.
    * [ ] Basic chat interface.
* [ ] **Phase 3: Velociraptor Integration**
    * [ ] Develop module for secure communication with Velociraptor API.
    * [ ] Enable execution of generated VQL on a live server (with user permission).
    * [ ] Implement results retrieval and presentation.
* [ ] **Phase 4: Advanced Features & Refinement**
    * [ ] Advanced conversational AI features (context memory, clarification dialogues).
    * [ ] Model fine-tuning based on user feedback and VQL updates.
    * [ ] Support for a wider array of VQL plugins and artifacts.

## Acknowledgements

* The **Velociraptor project** ([https://docs.velociraptor.app/](https://docs.velociraptor.app/)) and its maintainers for creating such a powerful and open tool.
* *(Feel free to add any other projects, communities, or individuals that inspire or contribute to this idea.)*
