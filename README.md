Sustainable Smart City Assistant: Empowering Urban Interaction with AI
This project, developed as part of the SmartBridge Generative AI Virtual Internship, introduces a Sustainable Smart City Assistant. This intelligent AI interface aims to facilitate seamless interaction between citizens and their city's resources, leveraging the power of large language models. The assistant is designed to be a comprehensive tool, offering insights into sustainability, promoting eco-friendly practices, providing real-time weather updates, and supporting various smart city functionalities like transport, waste management, and energy conservation.

Project Overview
The core objective of this initiative is to create an accessible and intelligent platform that enhances citizen engagement with urban sustainability efforts. While the initial vision included IBM Watsonx Granite LLM, the project successfully integrated the Falcon-7B-Instruct model due to availability considerations, demonstrating adaptability and robust implementation.

Project Phases Breakdown
Phase 1: Ideation and Research
The foundational phase involved conceptualizing a Smart City Assistant with a strong emphasis on sustainability and AI-driven interaction. Extensive research was conducted into suitable technologies, including IBM Granite LLM, Hugging Face models, Streamlit, FastAPI, and optionally Pinecone for future enhancements.

Phase 2: Dataset Preparation and LLM Setup
Given the constraints with IBM Granite's availability, the Falcon-7B-Instruct large language model was chosen as the base. The model was integrated using .safetensors files (model-00001-of-00002.safetensors, model-00002-of-00002.safetensors) and successfully loaded via the Hugging Face Transformers library and pipeline.

Phase 3: Application Development
This phase focused on building the interactive components of the assistant. A user-friendly front-end was developed using Streamlit, providing an intuitive interface for citizens. A FastAPI (or Flask) backend was set up to manage interactions with the LLM and process user inputs. Modular components were integrated, including:

Natural language input processing.

Efficient response generation from the LLM.

Optional support for weather APIs (e.g., OpenWeather).

Integration of eco-friendly tips and smart suggestions.

Access to city development facts and government initiatives.

Phase 4: Final Integration & Deployment
The project was deployed locally due to the substantial size of the language model. Significant attention was paid to ensuring a clean and intuitive user interface, facilitating easy prompt input and clear assistant output. A comprehensive demo video was recorded, and the complete codebase has been made available on GitHub.

Tech Stack
Area	Technology Used
Frontend UI	Streamlit
Backend API	FastAPI / Flask
LLM	Falcon-7B-Instruct / IBM Granite (Planned)
Model Source	Hugging Face (Offline Setup)
Model Format	.safetensors
Language	Python
Directory Structure
smart-city-assistant/
├── app.py
├── backend/
│   └── api.py
├── models/
│   ├── config.json
│   ├── model-00001-of-00002.safetensors
│   ├── model-00002-of-00002.safetensors
│   └── tokenizer/
├── templates/
│   └── ui.html
├── README.md
└── requirements.txt

How to Run
To set up and run the Sustainable Smart City Assistant locally, please follow these steps:

Install dependencies:

Bash

pip install -r requirements.txt
Run Streamlit App:

Bash

streamlit run app.py
If you are using FastAPI for the backend, ensure it's running:

Bash

uvicorn backend.api:app --reload
Model Setup:
Ensure you have the following .safetensors model files and associated configuration within the models/ folder:

model-00001-of-00002.safetensors


Key Features
The Sustainable Smart City Assistant offers a range of powerful features designed to enhance citizen interaction and promote sustainability:

💡 Natural Language Interaction: Users can ask sustainability-related questions using natural language.

🌤️ Real-time Information: Provides access to real-time weather updates and relevant smart city information.

🧠 Offline LLM Power: Powered by Hugging Face LLM models set up for offline access, ensuring performance and privacy.

🛠️ User-Friendly Interface: Built with Streamlit for an intuitive and easy-to-use graphical interface.

♻️ Sustainability Focus: Designed with sustainability at its core, promoting eco-friendly practices and awareness.

Acknowledgements
We extend our sincere gratitude to the following for their invaluable support and resources:

SmartBridge: For hosting this impactful Generative AI Internship program.

IBM Watsonx and Hugging Face: For providing access to powerful LLM technologies.

Mentors and Reviewers: For their continuous guidance, insights, and support throughout the project development.

Submission Details
Student Name: K. Sai Charan

Team ID: LTVIP2025TMID32000

Project Title: Sustainable Smart City Assistant

Internship: SmartBridge - Generative AI Virtual Internship

Re-submission: ✅ Updated with complete files and demo video.
#