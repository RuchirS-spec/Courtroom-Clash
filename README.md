# ⚖️ Courtroom Clash: An AI Legal Simulator

**Simulate a chaotic courtroom battle between a meticulous prosecutor and an unpredictable defense lawyer using Retrieval-Augmented Generation (RAG) and Large Language Models.**

This project uses **Langflow** to create and visualize a complex agent-based system where AI personas argue a court case provided by the user. The case facts are stored and retrieved from a vector database powered by **Astra DB**, ensuring all arguments are grounded in the provided evidence.

---
## ✨ Features

* **Dynamic AI Personas:** Experience the clash between a fact-driven prosecutor and a creative, sometimes chaotic, defense lawyer.
* **Retrieval-Augmented Generation (RAG):** All arguments are grounded in the facts of the case you provide, retrieved from an **Astra DB** vector store.
* **Powered by GPT-3.5 Turbo:** Utilizes the speed and capability of `gpt-3.5-turbo` for generating compelling legal arguments.
* **Bring Your Own Case:** Input any peculiar or famous court case and watch the AI agents dissect and argue it.
* **Visual Flow:** Built with **Langflow** for easy visualization and modification of the agent's logic.

---
## ⚙️ Tech Stack

* **Orchestration:** [Langflow](https://langflow.org/)
* **Vector Database:** [Astra DB](https://www.datastax.com/products/astra-db) (via DataStax)
* **LLM:** OpenAI GPT-3.5 Turbo
* **Core Framework:** LangChain

---
## 🛠️ Setup and Installation

Follow these steps to get the project running on your local machine.

### 1. Prerequisites

* Python 3.9+
* Git
* An [OpenAI API Key](https://platform.openai.com/api-keys)
* A free [Astra DB](https://astra.datastax.com/) account

### 2. Clone the Repository

```bash
git clone [https://github.com/YourUsername/courtroom-clash.git](https://github.com/YourUsername/courtroom-clash.git)
cd courtroom-clash
