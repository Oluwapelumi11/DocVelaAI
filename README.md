# DocVela

DocVela is an AI-powered web application that allows users to upload, analyze, and manage PDF documents. The application leverages GPT-4o-mini for natural language processing and a vectorization model (text-embedding-3-small) to generate embeddings and semantic search capabilities. Users can interact with the app through a chatbot to learn from the content of their documents, get summaries, ask for elaborations, delete files, and list available PDFs.

## Features

- **File Upload**: Upload PDFs to the platform for processing.
- **Text Analysis**: Use GPT-4o-mini to analyze and summarize the content of PDFs.
- **Semantic Search**: Perform semantic searches to find relevant information in documents.
- **File Management**: List uploaded files and delete them through the interface.
- **Error Handling**: Clear and informative error messages are provided for smooth user experience.

## Tech Stack

- **ASP.NET Core**: Backend framework for web application development.
- **Blazor**: For building interactive web UIs.
- **GPT-4o-mini**: Language model used for processing and responding to user queries.
- **Text-embedding-3-small**: Vectorization model used to generate embeddings for documents.
- **C#**: The primary programming language.
- **Microsoft.Extensions.AI**: A library to integrate AI functionalities.
- **GitHub Personal Access Token**: Required for integration with GitHub models.

## Installation

To run this project locally, follow the steps below:

### Prerequisites

- .NET 9.0 
- Visual Studio 2022 or any other preferred IDE
- GitHub Personal Access Token (for AI model integration)

### Steps to Set Up

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/DocVela.git
   cd DocVela
2. **Install dependencies**:
   Make sure all necessary dependencies are installed by running:

   ```bash
   dotnet restore
3. **Set up your GitHub Personal Access Token**:
   Store your GitHub token securely in the user secrets or in the `appsettings.json` file:
   Or using user secrets (recommended for security):

   ### In `appsettings.json`:
   ```json
   {
      "GitHubModels:Token": "YOUR_TOKEN_HERE"
   }
4. **Run the application**:
   Launch the app with:
   ```bash
   dotnet run
   
 # Usage

### Interacting with the Chatbot

#### Upload a PDF
Upload any PDF to the system through the web interface.

#### Ask Questions
After uploading, interact with the chatbot to learn from the document. For example, ask questions like:

- "Can you explain what microservices are?"
- "What are the main components of a microservices architecture?"

### File Management

- To list all uploaded PDFs, simply type:
  - "List all uploaded files"
  
- To delete a specific file, ask:
  - "Delete the file [filename]"

### Example Queries

#### Ask about content:
- "What does the document say about distributed systems?"
- "Summarize the chapter on microservices."

#### File Management:
- "List uploaded PDFs."
- "Delete the file 'microservices_overview.pdf'."

 
