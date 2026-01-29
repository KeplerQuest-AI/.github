# KeplerQuest-AI (K-QUEST-AI)

**KeplerQuest-AI (K-QUEST-AI)** is a modular and reproducible software framework that integrates **augmented reality (AR)** and **large language model (LLM)–powered conversational agents** to support the interactive exploration of **Kepler’s laws of planetary motion**.

The repositories in this organization provide the **technological infrastructure** used in the study reported in this [paper](). This repository collection is intended to enable **reproducibility, inspection, and technical reuse** of the AR and AI components described therein.

Pedagogical design, experimental methodology, and learning outcomes are documented exclusively in the associated research publication (see **Related Publication**).

---

## Scope of the Software

KeplerQuest-AI provides:

- A **Unity-based augmented reality application** for visualizing planetary motion according to Kepler’s laws.
- A **web-based LLM-powered chatbot system** designed to support guided inquiry through conversational interaction.
- A **client–server architecture** that decouples AR visualization from AI-driven dialogue.
- An implementation designed to operate reliably under typical classroom network and device conditions.

The software is focused on **technology implementation**, not on prescribing a specific instructional activity.

---

## System Architecture Overview

KeplerQuest-AI is organized as a **multi-repository system**, separating AR and AI components to support maintainability and reproducibility.

### Core Components

#### Augmented Reality Client (`arkepler-unity`)
- Developed using **Unity 2022.3**
- Uses **Vuforia** for image-based tracking
- Runs locally on **Android mobile devices**
- Activates 3D simulations of planetary motion when image targets are detected
- Optimized for mid-range smartphones to ensure stable frame rates

#### LLM-Based Chatbot Backend (`arkepler-llm`)
- Implemented as a **web-based application using Streamlit**
- Powered by **Open LLaMA 3.3–70B**, deployed locally via **Ollama**
- Provides conversational agents framed as narrative guides
- Uses structured prompts based on:
  - Narrative framing
  - Socratic questioning
  - Observation-driven reasoning
  - Qualitative evaluative feedback
- Average response latency of approximately **four seconds**, with no reported connectivity failures under study conditions

---

## Design Principles

The technological design of KeplerQuest-AI follows these principles, as described in the paper:

- **Complementarity of modalities**  
  AR externalizes dynamic and spatial phenomena, while LLM-based chatbots scaffold interpretation and reflection through dialogue.

- **Inquiry preservation**  
  Conversational agents are explicitly instructed not to name Kepler’s laws, even if prompted, to avoid shortcut learning and encourage reasoning from observation.

- **Modularity and separation of concerns**  
  Visualization and conversational intelligence are implemented as independent components connected through a defined interface.

---

## Reproducibility

This repository collection contains the **core technological elements** required to reproduce the system described in the paper, including:

- AR visualization logic
- Image-based tracking configuration
- Chatbot prompt structures
- Backend deployment setup

Configuration details and dependencies are documented within each individual repository.

---

## Related Publication

The educational intervention, research questions, methodology, and learning outcomes enabled by this software are reported in the following paper:

> **Gamified Augmented Reality and LLM-Powered Chatbots for Teaching Kepler's Laws**  
> John F. Suárez-Pérez, Edgar André Ramírez-Alonso  
> *EDUCON 2026 - IEEE Conference Proceedings* (accepted)

Please cite this publication when using or referencing KeplerQuest-AI in academic or research work.

---

## Research Context

As described in the paper, KeplerQuest-AI contributes to research in:

- Augmented reality for physics education
- Generative AI and conversational agents for learning
- Gamified and immersive learning environments
- Human–AI interaction in STEM education

---

## License

This project is licensed under the **Creative Commons Attribution–NonCommercial–ShareAlike 4.0 International (CC BY-NC-SA 4.0)** license.

---

## Contact

For technical questions related to the implementation, please refer to the documentation within the individual repositories or contact the corresponding author listed in the related publication.
