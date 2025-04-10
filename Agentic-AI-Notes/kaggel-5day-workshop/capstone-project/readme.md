
# Smart Recipe Generator from Pantry Photos

![GitHub](https://img.shields.io/badge/license-MIT-blue.svg)
![Python](https://img.shields.io/badge/python-3.9+-green.svg)
![Google Cloud](https://img.shields.io/badge/Google%20Cloud-Vertex%20AI-yellow.svg)

## Overview

The **Smart Recipe Generator from Pantry Photos** is an AI-powered tool that helps users decide "what's for dinner" by analyzing pantry photos, identifying ingredients, and suggesting personalized recipes. Built as a Capstone Project for the [5-day Gen AI Intensive Course with Google](https://kaggle.com/competitions/gen-ai-intensive-course-capstone-2025q1), this project leverages Google’s Agent Development Kit (ADK) and showcases generative AI capabilities to solve a real-world problem with creativity and practicality.

### Features
- **Photo-to-Ingredients:** Upload a pantry photo and get a list of detected ingredients.
- **Recipe Suggestions:** Retrieve recipes tailored to your ingredients using Retrieval-Augmented Generation (RAG).
- **Personalization:** Remembers dietary preferences (e.g., "no dairy") across sessions with context caching.
- **Scalable Deployment:** Ready to deploy on Google Cloud’s Vertex AI Agent Engine or Cloud Run.

### Gen AI Capabilities Demonstrated
1. **Image Understanding:** Identifies ingredients from photos using Gemini 2.0 Flash.
2. **Retrieval Augmented Generation (RAG):** Matches ingredients to recipes via a vector store.
3. **Context Caching:** Stores user preferences for personalized outputs.

---

## Project Context

This project was developed as part of the [Gen AI Intensive Course Capstone 2025Q1](https://kaggle.com/competitions/gen-ai-intensive-course-capstone-2025q1), hosted by Google and Kaggle. The competition ran from April 4 to April 20, 2025, with the goal of applying at least three Gen AI capabilities to a creative use case. See the [Kaggle competition page](https://kaggle.com/competitions/gen-ai-intensive-course-capstone-2025q1) for details.

---

## Prerequisites

- **Python 3.9+**
- **Google Cloud Account** (for API access and deployment)
- **Kaggle Account** (optional, for running the notebook)
- Dependencies (see `requirements.txt`):
  - `adk` (Agent Development Kit)
  - `google-cloud-aiplatform`
  - `sentence-transformers`

---

## Installation

1. **Clone the Repository**
   ```bash
   git clone https://github.com/Ajmalniz/smart-recipe-generator.git
   cd smart-recipe-generator
   ```

2. **Set Up a Virtual Environment**
   ```bash
   python -m venv venv
   source venv/bin/activate  # Linux/Mac
   venv\Scripts\activate     # Windows
   ```

3. **Install Dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Configure Google Cloud**
   - Set up a Google Cloud project and enable the Vertex AI API.
   - Export your API key:
     ```bash
     export GOOGLE_API_KEY="your-api-key-here"
     ```
   - Initialize Vertex AI:
     ```python
     from google.cloud import aiplatform
     aiplatform.init(project="your-gcp-project", location="us-central1")
     ```

---

## Usage

### Running Locally
1. **Prepare a Sample Photo**
   - Place a pantry photo (e.g., `sample-pantry.jpg`) in the project directory.

2. **Run the Main Script**
   ```bash
   python main.py --photo sample-pantry.jpg
   ```
   - Output: Detected ingredients and a suggested recipe (e.g., "Spaghetti Marinara (no dairy)").

### Running in a Kaggle Notebook
- Upload the code and a sample image to a Kaggle Notebook.
- Execute the cells as shown in `notebook.ipynb`.
- See the [Kaggle submission](#kaggle-submission) section for submission details.

### Example Output
```
Detected ingredients: ['pasta', 'tomato', 'cheese']
Suggested recipe: Spaghetti Marinara (substitute cheese with plant-based alternative)
```

---

## Project Structure

```
smart-recipe-generator/
├── main.py              # Main script to run the agent
├── notebook.ipynb       # Kaggle Notebook submission
├── Dockerfile          # Container for deployment
├── requirements.txt     # Python dependencies
├── README.md           # This file
└── sample-pantry.jpg   # Sample input image (optional)
```

---

## Deployment

Deploy the agent to Google Cloud for scalability using ADK’s supported options:

### Option 1: Vertex AI Agent Engine
1. **Build the Docker Image**
   ```bash
   docker build -t gcr.io/your-project/recipe-agent .
   ```
2. **Push to Google Container Registry**
   ```bash
   docker push gcr.io/your-project/recipe-agent
   ```
3. **Deploy to Vertex AI**
   - Follow the [ADK Vertex AI guide](https://google.github.io/adk-docs/deployment/vertex-ai) to deploy via the Google Cloud Console or `gcloud`.

### Option 2: Cloud Run
1. **Build and Deploy**
   ```bash
   gcloud run deploy recipe-agent \
     --image gcr.io/your-project/recipe-agent \
     --platform managed \
     --region us-central1
   ```
2. **Access the Endpoint**
   - Get the URL from the Cloud Run console and query it with a photo upload.

---

## Kaggle Submission

For the Capstone Project (due April 20, 2025):
1. **Notebook:** Submit `notebook.ipynb` via the [Google Form](https://example.com/google-form-link).
2. **Optional Bonus:**
   - **Blogpost:** Write about the use case, code snippets, and limitations (e.g., image quality). Host it publicly (e.g., Medium).
   - **YouTube Video:** Record a demo with visuals and voiceover. Upload publicly.
3. **Scoring Goals:**
   - Max score: 22.5 (Notebook: 10 pts * 1.5x Blogpost * 1.5x Video).
   - Focus on clear documentation and innovative use case.

---

## Future Improvements

- Integrate a real vector database (e.g., Vertex AI Vector Search) for RAG.
- Add voice input for hands-free recipe queries.
- Improve image recognition with larger datasets or fine-tuned models.

---

## Acknowledgments

- Built with [Google’s Agent Development Kit (ADK)](https://google.github.io/adk-docs).
- Part of the [Gen AI Intensive Course Capstone 2025Q1](https://kaggle.com/competitions/gen-ai-intensive-course-capstone-2025q1) by Google and Kaggle.
- Inspired by the need to make dinner decisions easier!

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

**Author:** Ajmal Khan  
**GitHub:** [Ajmalniz](https://github.com/Ajmalniz)  
**Date:** April 2025

---

