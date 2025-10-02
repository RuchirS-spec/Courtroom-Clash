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

1.  **Prerequisites**
    * Python 3.9+
    * Git
    * An [OpenAI API Key](https://platform.openai.com/api-keys)
    * A free [Astra DB](https://astra.datastax.com/) account

2.  **Clone the Repository**
    ```bash
    git clone [https://github.com/YourUsername/courtroom-clash.git](https://github.com/YourUsername/courtroom-clash.git)
    cd courtroom-clash
    ```

3.  **Install Dependencies**
    Install all the necessary Python packages.
    ```bash
    pip install -r requirements.txt
    ```

4.  **Set Up Credentials**
    This project requires API keys and database credentials. Your secrets are managed using a `.env` file. First, create a copy of the example environment file:
    ```bash
    cp .env.example .env
    ```
    Then, open the `.env` file and add your credentials.
    ```env
    # .env

    # OpenAI API Key
    OPENAI_API_KEY="sk-..."

    # Astra DB Credentials
    ASTRA_DB_APPLICATION_TOKEN="AstraCS:..."
    ASTRA_DB_API_ENDPOINT="https://<your-db-id>-<your-region>.apps.astra.datastax.com"
    ```

5.  **Configure Astra DB**
    * In your Astra DB dashboard, **create a new Vector Database**.
    * Create a **collection** (e.g., `court_cases`) with the appropriate embedding dimension for OpenAI models (**1536**).
    * Generate an **Application Token** with "Database Administrator" permissions and use it for `ASTRA_DB_APPLICATION_TOKEN`.

---
## 🚀 How to Use

1.  **Start Langflow:**
    Open your terminal and run the Langflow server.
    ```bash
    langflow
    ```

2.  **Import the Flow:**
    * Navigate to `http://127.0.0.1:7860` in your browser.
    * Click "Import" and select the `flow.json` file from this repository.

3.  **Run the Simulation:**
    * Open the imported "Courtroom Clash" flow.
    * Navigate to the input node on the canvas.
    * Paste the text of any court case you want to simulate.
    * Interact with the flow using the "Playground" chat interface to see the agents argue.

---
##📖 Project Structure

  * ├── flow.json               # The main Langflow project file
  * ├── .env.example            # Template for environment variables
  * ├── .gitignore              # Files to be ignored by Git
  * ├── requirements.txt        # Python dependencies
  * └── README.md               # You are here!
  
---
## 🤝 Contributing

Contributions are welcome! If you have an idea for a new feature or want to improve the agent personas, please feel free to fork the repository, create a new branch, and submit a pull request.

1.  Fork the Project
2.  Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3.  Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4.  Push to the Branch (`git push origin feature/AmazingFeature`)
5.  Open a Pull Request
