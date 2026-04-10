# How to run?

### STEPS:

Clone the repository

```bash
git clone https://github.com/vishxlkr/MedAI.git
cd MedAI
```

### STEP 01- Create a virtual environment after opening the repository

```bash
python -m venv venv
# On Windows, activate using: venv\Scripts\activate
# On macOS/Linux, activate using: source venv/bin/activate
venv\Scripts\activate
```

### STEP 02- Install the requirements

```bash
pip install -r requirements.txt
```

### Create a `.env` file in the root directory and add your Pinecone & OpenAI credentials as follows:

```ini
PINECONE_API_KEY = "xxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
OPENAI_API_KEY = "xxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
```

```bash
# run the following command to store embeddings to pinecone
python store_index.py
```

```bash
# Finally run the following command
python app.py
```

Now,

```bash
open up http://localhost:8080/
```

### Tech Stack Used:

- Python
- LangChain
- Flask
- GPT
- Pinecone
