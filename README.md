---
# Memory-In-LLM

Welcome to **Memory-In-LLM**, a comprehensive learning repository for understanding and experimenting with memory mechanisms in Large Language Models (LLMs). This project is structured for hands-on exploration, with detailed notebooks and scripts covering both Long Term Memory (LTM) and Short Term Memory (STM).

## 📚 Project Overview

This repository is designed for students, researchers, and enthusiasts to:
- Learn the theory and practice of memory in LLMs
- Implement and experiment with LTM and STM
- Integrate LLMs with external databases
- Explore advanced memory management techniques

## 🗂️ Detailed File Analysis

### Root Files

- **main.py**: Simple script to verify your environment. Prints a greeting message. Use as a template for custom experiments.

- **pyproject.toml**: Project configuration. Specifies Python 3.11+, and dependencies for LangChain, LangGraph, HuggingFace, Google GenAI, and Postgres integration. Use Poetry or pip to install dependencies.

### Long Term Memory/

**Purpose:** Explore persistent memory for LLMs, including in-memory and database-backed storage.

- **6_ltm_basics.ipynb**: 
	- Introduces the concept of long-term memory in LLMs.
	- Demonstrates creating an in-memory store and namespace for user data using LangGraph.

- **7_ltm_implementation.ipynb**:
	- Step-by-step implementation of a chatbot with long-term memory.
	- Uses Google Generative AI, LangChain, and LangGraph.
	- Shows how to read, store, and retrieve user memories.

- **8_llm_postgres.ipynb**:
	- Advanced notebook integrating Postgres for persistent LTM.
	- Demonstrates setup, system prompts, and user-specific memory retrieval.
	- Uses LangGraph's PostgresStore for scalable memory.

- **docker-compose.yml**:
	- Defines a Postgres service for database-backed experiments.
	- Exposes port 5442 for local access.

### Short Term Memory/

**Purpose:** Focus on temporary, session-based memory in LLMs, including persistence, trimming, deletion, and summarization.

- **1_stm.ipynb**:
	- Introduces STM concepts and basic usage.
	- Uses HuggingFace models and LangGraph for state management.

- **2_stm_persistence.ipynb**:
	- Shows how to persist STM using Postgres checkpoints.
	- Demonstrates saving and restoring session state.

- **3_stm_trimming.ipynb**:
	- Explains trimming STM to manage token limits.
	- Uses utility functions to count and trim messages.

- **4_stm_deletion.ipynb**:
	- Demonstrates deletion of specific STM entries.
	- Uses custom message removal logic.

- **5_stm_summary.ipynb**:
	- Summarizes STM contents for efficient context management.
	- Integrates summarization with HuggingFace models.

- **docker-compose.yml**:
	- Identical to LTM setup; provides Postgres for STM persistence.

## ⚙️ Installation & Usage

1. **Clone the repository**
	 ```bash
	 git clone https://github.com/your-username/Memory-In-LLM.git
	 ```

2. **Install dependencies**
	 - With pip:
		 ```bash
		 pip install -r requirements.txt
		 ```
	 - Or with Poetry:
		 ```bash
		 poetry install
		 ```

3. **Run Notebooks**
	 - Open any notebook in Jupyter or VS Code.
	 - Follow the step-by-step instructions and code cells.

4. **Start Docker Services (if needed)**
	 - For database-backed experiments:
		 ```bash
		 cd "Long Term Memory"
		 docker-compose up
		 ```

## 🎯 Learning Goals

- Understand LTM vs STM in LLMs
- Implement memory stores and checkpoints
- Integrate LLMs with HuggingFace and Google GenAI
- Use Postgres for persistent memory
- Manage STM with trimming, deletion, and summarization

## 📝 Contributing

This repository is for learning and experimentation. Fork, modify, and share your findings. Pull requests for improvements or new modules are welcome!

## 📄 License

MIT License. See LICENSE for details.

---

Happy Learning! 🚀
`bash
	 pip install -r requirements.txt
	 `
Or use `pyproject.toml` with Poetry:
`bash
	 poetry install
	 `

3. **Run Notebooks**
   Open any notebook in Jupyter or VS Code and start experimenting!

4. **(Optional) Start Docker Services**
   For database-backed experiments, use Docker Compose:
   ```bash
   cd Long\ Term\ Memory
   docker-compose up
   ```

## 🎯 Learning Goals

- Understand the difference between Long Term and Short Term Memory in LLMs.
- Implement basic and advanced memory mechanisms.
- Experiment with persistence, trimming, deletion, and summarization.
- Integrate LLM memory with external databases.
- Build intuition for real-world applications of memory in LLMs.

## 📝 Contributing

This repository is for learning and experimentation. Feel free to fork, modify, and share your findings. Pull requests for improvements or new learning modules are welcome!

## 📄 License

This project is licensed under the MIT License. See the LICENSE file for details.

---

Happy Learning! 🚀
