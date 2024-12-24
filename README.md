# Medical AI Assistant

The Medical AI Assistant is a Streamlit-based application designed to assist healthcare professionals by providing diagnostic insights and personalized treatment recommendations. This AI-powered tool leverages advanced language models and APIs to streamline the process of patient assessment and treatment planning.

## Features

- **Patient Information Input:** Capture patient details, symptoms, medical history, and lifestyle factors via an intuitive UI.
- **AI-Powered Diagnosis:** Analyze symptoms and medical history to provide a preliminary diagnosis.
- **Treatment Recommendations:** Generate a comprehensive treatment plan, including medication, lifestyle advice, and follow-up care.
- **Downloadable Reports:** Export diagnosis and treatment recommendations in a professional Word document format.
- **Interactive UI:** User-friendly interface with tabs for patient assessment and results display.

## Technology Stack

- **Backend:** Python
- **Frontend:** Streamlit
- **AI Model:** OpenAI GPT-3.5-Turbo (via LangChain)
- **Tools:**
  - Serper Dev Tool (for medical data queries)
  - Scrape Website Tool (for supplementary data retrieval)
- **Document Generation:** Python-docx

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/sango-07/MediAI-Medical-AI-Agent.git
    cd medical-ai-assistant
    ```

2. Create a virtual environment:
    ```bash
    python -m venv venv
    source venv/bin/activate # On Windows, use `venv\Scripts\activate`
    ```

3. Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```

4. Set up environment variables:
    - Create a `.env` file in the root directory with the following keys:
      ```
      OPENAI_API_KEY=your_openai_api_key
      SERPER_API_KEY=your_serper_api_key
      ```

5. Run the application:
    ```bash
    streamlit run app.py
    ```

6. Access the app at [http://localhost:8501](http://localhost:8501).

## Usage

1. Navigate to the **Patient Information** sidebar to input details such as gender, age, height, and weight.
2. In the **Patient Assessment** tab, enter:
    - Current Symptoms
    - Medical History
    - Optional additional information (e.g., allergies, lifestyle factors).
3. Click **Generate Analysis** to analyze the patient data.
4. View results in the **Results** tab, including:
    - Preliminary diagnosis.
    - Comprehensive treatment recommendations.
5. Download the generated report as a Word document.

## File Structure

```
medical-ai-assistant/
|-- app.py                  # Main application script
|-- requirements.txt        # Python dependencies
|-- .env                    # Environment variables
|-- assets/                 # Images and assets for documentation
|-- utils/                  # Helper functions and utilities
|-- templates/              # Templates for document generation
```

## Dependencies

- **Streamlit:** For building the web application.
- **LangChain:** For integrating OpenAI's GPT model.
- **Python-docx:** For generating Word documents.
- **dotenv:** For managing environment variables.
- **CrewAI:** For orchestrating agents and tasks.

Install all dependencies with:
```bash
pip install -r requirements.txt
```

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository.
2. Create a new branch:
    ```bash
    git checkout -b feature-name
    ```
3. Commit your changes:
    ```bash
    git commit -m "Add feature"
    ```
4. Push to the branch:
    ```bash
    git push origin feature-name
    ```
5. Open a pull request.

## License

This project is licensed under the MIT License. See the `LICENSE` file for more details.

## Acknowledgments

- OpenAI for providing powerful language models.
- Streamlit for the intuitive and flexible web application framework.
- The medical professionals whose feedback helped shape this tool.

---

### Disclaimer
The Medical AI Assistant is designed for educational and experimental purposes only. It is not a substitute for professional medical advice, diagnosis, or treatment. Always seek the advice of a qualified healthcare provider with any questions you may have regarding a medical condition.

