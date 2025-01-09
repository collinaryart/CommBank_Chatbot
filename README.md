# Multilingual Chatbot for Commonwealth Bank

This chatbot integrates Azure Function Apps for serverless computing, Azure Cognitive Services for language detection and translation, and OpenAI's API for AI-driven response generation. This approach aims to provide seamless engagement for customers of CommBank across various linguistic backgrounds. 

The initiative assists customers by:
- Auto-detecting the language used by the user.
- Processing banking inquiries in multiple languages.
- Utilising user-friendly interfaces that consider cultural nuances to bridge the communication gap.

Developed with Tony Hsieh, Akshita Mediratta and Kimme Tan.

## Tech Stack

- **Azure Function Apps**: Serverless computing for chatbot logic.
- **Azure Cognitive Services & Translator Text API**: For multilingual support.
- **OpenAI API**: Advanced AI for context-aware responses.
- **Cosmos DB**: NoSQL database for storing scraped data.
- **Azure AI Search & RAG**: Enhancing data retrieval and response generation.
- **Azure Key Vault**: Securing secrets.
- **Selenium**: Web scraping.
- **React**: Frontend interface.
- **GitHub Actions**: CI/CD for deployment.
- **Visual Studio Code**: IDE with Azure and Python extensions.
- **Python 3.11**: Programming language.


## Setup and Installation

### Prerequisites

- An Azure account with access to Azure Function Apps and Azure Cognitive Services.
- An OpenAI API key for integrating chatbot intelligence.
- Python 3.11 installed on your machine.
- Visual Studio Code with Azure Function App and Python extensions installed.
- Git for version control.

### Basic Infrastructure Setup

1. **Azure Function App Setup**
   - Create a new Function App resource in Azure.
   - Follow the Azure documentation for initial setup: [Azure Function Apps Documentation](https://docs.microsoft.com/en-us/azure/azure-functions/).
2. **Azure Cognitive Services Integration**
   - Set up an instance of Azure Cognitive Services for language detection and translation capabilities.
   - Securely store the API key and endpoint URL for later use in the application.

3. **OpenAI API Integration**
   - Sign up for an OpenAI API key.
   - Securely store the API key for use in the chatbot's response generation logic.

### Running the Project

1. Clone the project repository to your local machine.
    ```bash
    git clone https://github.com/ITU-0327/CBA_Multilingual_Chatbot
    ```

2. Install the required Python dependencies.
   ```bash
   pip install -r requirements.txt
   ```

3. Set up environment variables for Azure and OpenAI API keys.
   - Create a .env file in the root directory of your project.
   - Add your Azure Cognitive Services and OpenAI API keys as follows:
     ```
     AZURE_TRANSLATOR_TEXT_KEY=<your-translator-text-api-key>
     AZURE_SERVICE_REGION=<your-service-region>
     OPENAI_API_KEY=<your-openai-api-key>
     ```

4. Start the Azure Function App locally for testing.
   - Follow the Azure Functions extension in Visual Studio Code to run your app.

## License

Distributed under the MIT License. See [LICENSE](LICENSE) for more information.
