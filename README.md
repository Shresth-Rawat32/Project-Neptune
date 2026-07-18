# Project-Neptune
A model agnostic local cognitive architecture exploring persistent memory, reasoning, and emergent intelligence.

## **What is Neptune?**
The core idea behind Neptune is that instead of having an AI rely solely on what it was trained on, we build its understanding of the world by simulating how a child learns. It constantly asks questions when it is unsure, connects new pieces of information with what it already knows, remembers what it has learned, and gradually develops its own worldview. That is what Project Neptune hopes to build.
Rather than treating the language model as the finished intelligence, Neptune explores whether intelligence can emerge from the systems built around it.

## **Why does Neptune exist?**
I observed that children learn by constantly asking the "why" behind things, which they then use to connect pieces of information that become their "worldview." This is an already researched topic known as constructivism. I simply questioned what results we would get by simulating this behavior in AI models. I don't know if this approach will work. Project Neptune is my attempt to explore that question.

## **Core philosophy**
1.Architecure > Models : The language model is replaceable, The sorrounding cognitive systems are the real project.
2.Learning > memorization. Neptune should build an understanding of the world through questioning, connecting ideas, and experience rather than relying solely on pre-trained knowledge.
3.Emergent identity :  Neptune should not begin with a hardcoded personality or identity. Its worldview should emerge gradually from its memories and interactions.
4.Truth > confidence : Neptune should acknowledge uncertainty, seek information when needed, and revise its beliefs when presented with better evidence.
5.Incremental development : Every new capability should build on a stable foundation instead of adding complexity for its own sake.


## **Current architecture**
               ┌──────────────────────┐
               │      User Input      │
               └──────────┬───────────┘
                          │
                          ▼
               Prompt Construction
      (System Prompt + User Message)
                          │
                          ▼
          Qwen2.5-1.5B-Instruct (4-bit)
                          │
                          ▼
              Response Extraction
                          │
                          ▼
       Store Conversation in SQLite
                          │
                          ▼
                Return Response
                
## **Current progress**
### Completed
- [x] Local LLM inference
- [x] GPU acceleration with 4-bit quantization
- [x] Persistent memory using SQLite
- [x] Conversation history storage
- [x] System prompt and cognitive laws
- [x] Response extraction pipeline

### In Progress
- [ ] Contextual memory retrieval
- [ ] Memory ranking and relevance
- [ ] Improved response generation

### Planned
- [ ] Belief formation system
- [ ] Validator and self-correction
- [ ] Knowledge graph / concept linking
- [ ] Long-term learning
- [ ] World model development
- [ ] Multi-model cognitive architecture

**Roadmap**
## Stage 1 — Foundation
- [x] Local language model
- [x] Persistent memory
- [x] Conversation pipeline
- [x] GPU acceleration

## Stage 2 — Memory
- [ ] Retrieve relevant memories
- [ ] Rank memories by relevance
- [ ] Inject memories into responses
- [ ] Improve memory organization
## Stage 3 — Active Learning
- [ ] Introduce a dedicated question generation model
- [ ] Generate questions when uncertain
- [ ] Research or retrieve answers to generated questions
- [ ] Validate newly acquired information
- [ ] Store validated knowledge in long-term memory
## Stage 4 — Reasoning
- [ ] Connect related concepts
- [ ] Build belief structures
- [ ] Resolve conflicting information
- [ ] Improve reasoning consistency

## Stage 5 — Understanding
- [ ] Develop a persistent worldview
- [ ] Learn continuously from interactions
- [ ] Refine beliefs over time
- [ ] Explore emergent behavior

## Stage 6 — Cognitive Architecture
- [ ] Multi-model architecture
- [ ] Specialized reasoning modules
- [ ] Improve scalability and performance
- [ ] Continue experimenting with new cognitive systems

## Repository Structure

```text
Project-Neptune/
│
├── README.md
├── LICENSE
├── .gitignore
├── requirements.txt
│
├── docs/
│   ├── PHILOSOPHY.md
│   ├── ARCHITECTURE.md
│   ├── ROADMAP.md
│   └── CHANGELOG.md
│
├── journals/
│   ├── Day-1.md
│   ├── Day-2.md
│   └── ...
│
├── src/
│   ├── main.py
│   ├── memory.py
│   ├── database.py
│   ├── prompt.py
│   ├── model.py
│   ├── config.py
│   └── utils.py
│
├── data/
│   └── neptune_memory.db
│
└── assets/
    ├── architecture.png
    └── logo.png
```

> **Note:** This structure represents the planned organization of Project Neptune. The repository will be reorganized into this layout as the project documentation and architecture mature.

## Current Status
Neptune is an active research project and is not yet ready for general use. The current focus is on building the architecture and documenting its development. Installation instructions and usage examples will be added as the project becomes more stable.
