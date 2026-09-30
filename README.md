English：
 
⚠️ Important Note
This project is only a high-level concept.
Engineering details such as hardware circuits, PCB layout, low-level scheduling firmware, and model sharding drivers are not fully designed yet.
I do not have the capital or team to finish all development alone. This concept is open, no patents. The goal is to share this idea, invite global hardware and AI software developers to join together, supplement details, build prototypes and iterate.
Anyone can continue research based on this high-level concept.
English
 
Modular Offline AI Box (Open Concept)
 
Project Introduction
 
This is an open-source hardware concept. It is a pluggable modular AI computing box, reusing mature mobile SoC and LPDDR memory chips, adopting pipeline layer-by-layer inference architecture.
 
- Target spec: Expandable up to 4TB memory pool

- Capability: Run large language models (Hermes, etc.) offline locally, process documents, spreadsheets, images and segmented AI video rendering.

- Privacy: All computation runs locally. Build a small private encrypted local network. Devices transfer files and images with multi-layer encryption, no reliance on telecom operators.

- Architecture tradeoff: Remove expensive high-speed inter-chip interconnect. Each module independently computes one full model layer. Only small output tensors are passed between modules to cut hardware cost.

- Use case: Offline creation, local document analysis, private AI. Not designed for large-scale model training or high-concurrency cloud real-time chat.
 
Statement: This is only a concept. No patents reserved. Fully open for humanity. Anyone may freely use this idea for prototyping and mass production.
 
Working Principle
 
1. Module: Each pluggable module consists of mobile SoC + LPDDR memory. Hot-plug expansion for more memory and compute. Unused modules can sleep to save power.

2. Pipeline inference: Split the large model into layers. Each layer is assigned to one independent module. Only final outputs are passed to next module to reduce communication pressure.

3. Terminal: Connect to mobile phone or PC. Mobile phone is only for user interaction, all heavy AI computation runs on the box.

4. Private network: Devices communicate on license-free private wireless LAN. End-to-end multi-layer encryption for file/image transfer. Data never flows through public telecom networks.
 
Goal
 
Create a low-cost path beyond expensive high-end GPUs, so ordinary people can access local large AI models with strong data privacy.
