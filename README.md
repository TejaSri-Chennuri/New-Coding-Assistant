
# AI-Powered Chatbot for Code Generation and Refactoring. 

## Project Description  
This chatbot uses **AI-powered code generation and refactoring** to assist developers in writing and improving code.  
It is built using **FastAPI, Hugging Face Transformers, CodeT5, and Meta Llama 3**, making it an efficient and intelligent coding assistant.  

---

## Features  
- **Code Generation**: Generates AI-powered code snippets based on user input.  
- **Code Refactoring**: Enhances and optimizes existing code.  
- **FastAPI Integration**: Provides a REST API for easy integration with applications.  
- **Meta Llama 3 Support**: Uses an advanced AI model for better responses.  
- **Local Model Usage**: Loads models from local storage to reduce API dependency.  

cd chatbot-project
2️. Create a Virtual Environment (Recommended)
sh
Copy
Edit
python -m venv chatbot-env
Activate the virtual environment:

Windows:
sh
Copy
Edit
chatbot-env\Scripts\activate
Mac/Linux:
sh
Copy
Edit
source chatbot-env/bin/activate
3️. Install Dependencies
sh
Copy
Edit
pip install -r requirements.txt
 How to Run the Chatbot
1️. Run the Chatbot in Command Line
sh
Copy
Edit
python main.py
You can enter a prompt like:

python
Copy
Edit
def add(a, b):
The chatbot will generate the full function.

2️. Run the Chatbot as an API with FastAPI
sh
Copy
Edit
uvicorn main:app --host 0.0.0.0 --port 8000
Once running, test it using:

Swagger UI: http://127.0.0.1:8000/docs
FastAPI JSON API Endpoint:
sh
Copy
Edit
curl -X 'POST' 'http://127.0.0.1:8000/chat' -H 'Content-Type: application/json' -d '{"input_text": "def add(a, b):"}'
📂 Project Structure
csharp
Copy
Edit
chatbot-project/
│── main.py                 # FastAPI backend & chatbot logic
│── chatbot.py              # Command-line chatbot script
│── requirements.txt        # List of dependencies
│── models/
│   │── codet5-base/        # Local CodeT5 model files
│── README.md               # Project documentation
 License
This project is open-source under the MIT License.


