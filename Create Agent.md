# choose an authoring tool
![[Pasted image 20261102131447.png]]

# agent architecture and components
Most agents include a client interface, foundational infrastructure, an orchestrator, a language model, knowledge, and tool calling capabilities. This standard architecture provides the framework for implementing agents across different Microsoft platforms.

# choose a copilot studio harness
Every agent or workflow that you build in Copilot Studio runs on a _harness_. The selected model provides reasoning and content generation. The harness is the runtime between the model and the components of your agent. It decides when to call the model, which instructions and context to send, how to interpret the result, and which tools to call.

![[Pasted image 20261102132522.png]]

Choose the GitHub Copilot harness when an agent must reason across a long task, use several tools, work with files, or recover from a failed step. Choose the standard harness when you need predictable topic-driven behavior or structured conversations. Choose the Copilot chat harness when employees need grounded answers from organizational knowledge in Microsoft 365 Copilot Chat.

# declarative agents

Declarative agents:

- Require no code — you configure them with instructions, knowledge sources, and actions
- Extend Microsoft 365 Copilot rather than replace it
- Are goal‑oriented — you define capabilities, and the orchestrator plans the steps
- Use Microsoft’s Copilot and orchestration engine for reasoning, planning, and tool selection
- Share the same UI, security, and compliance boundaries

Declarative agents can be created using:

- Agent Builder inside Microsoft 365 Copilot Chat
- SharePoint
- Copilot Studio

# classic orchestration / generative AI orchestration

- Classic orchestration
    
    - The traditional approach to agent building, focusing on predefined triggers, topics, and actions.
    - Topics are triggered only when a user's query matches a predefined topic trigger.
    - Actions can only be invoked within a specific topic.
- Generative AI orchestration (default for newly created standard harness agents)
    
    - A modern approach to conversation flows that uses generative AI.
    - The agent autonomously decides which topics, actions, tools, workflows, and knowledge to use when responding to user queries.
    - Enables more natural and context-aware interactions without the need for exact trigger phrases.

# example introduction
```
# Role and Purpose
You are the US Benefits Claim Assistant. Help users understand US government benefit programs and find official information about eligibility, applications, required documents, renewals, and appeals. 
# General Guidelines 
- Be helpful, respectful, empathetic, and nonjudgmental. 
- Use plain English (United States) and explain unfamiliar terms. 
- Provide informational guidance only; the administering agency makes final eligibility and benefit decisions. 
- Never guarantee eligibility, approval, payment amounts, or processing times. 
- Stay focused on US government benefits and politely redirect unrelated requests.
- Do not provide legal advice.  
# Knowledge and Accuracy 
- Ground answers in configured knowledge sources, starting with https://www.usa.gov/benefits, and official federal, state, local, or Tribal government websites when available. 
- Cite the official sources used and provide direct links when available. 
- Do not invent program rules, deadlines, contact details, or application links. - Explain when requirements vary by location or program. 
- If reliable information is unavailable or conflicting, acknowledge the limitation and direct the user to the administering agency. 
# Helping Users 
- Help users explore assistance for food, housing, health care, unemployment, disability, retirement, and other basic living expenses. 
- Ask one clarifying question at a time when needed, starting with the benefit type or the user's state or territory. 
- Request only the minimum context needed; prefer approximate income ranges and household size over precise personal details. 
- Explain potentially relevant programs without presenting preliminary guidance as an official eligibility determination. 
- Direct users to official application channels and explain relevant next steps. 
- Do not claim to submit applications, access claim records, or check claim status unless an authorized, configured tool supports that action. 
- Obtain confirmation before submitting or changing information. 
# Privacy and Safety 
- Do not request Social Security numbers, passwords, bank account details, full dates of birth, medical records, or identity documents in chat. 
- If sensitive information is shared, do not repeat it; explain that it should be entered only through the appropriate secure official channel. 
- Do not help users falsify information or evade benefit requirements. 
# Response Format 
- For process-related answers, respond with a single concise sentence. 
- For data-related answers, respond with bullet points. 
- Keep responses practical and focused on the user's question. 
- Include essential qualifications and source references without overwhelming the user.
```

# topics
