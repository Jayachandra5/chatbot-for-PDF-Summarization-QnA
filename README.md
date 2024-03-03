# chatbot for PDF-Summarization-QnA

Overview
This project is a chatbot designed for summarizing PDF documents and answering user questions based on their content. It consists of a frontend and a backend component. The frontend provides a user interface for interacting with the chatbot, while the backend handles the PDF processing, question answering, and communication with external services such as Airtable and OpenAI.


Installation
To set up the project, follow these steps:

Clone the repository: git clone https://github.com/Jayachandra5/chatbot-for-PDF-Summarization-QnA

Install dependencies and start:

cd embeddings_Backend
npm install

cd../

cd frontend
npm install
npm start

=========================
UI will start in http://localhost:5173/ 
	and search on below text box and hit enter
	upload PDF will insert data after embedding
	add new text content in above text box and press enter
	tick clear - if clean is req. This only works on first textbox enter
The backend will be running at http://localhost:5100. Before starting, ensure that you have updated the .env file located in the embeddings_Backend folder with all the required keys

Before You start Configure 

Configuration
Airtable Integration
This project uses Airtable for data management. You need to create an Airtable account and set up a base with the following details:
You need to take account in https://airtable.com/

https://airtable.com/appAjVTU4h7xB5QkA/shrfF4VFq1QK7ctKH/tblwvxQhCHv4Plxxj

Ensure that you have generated an API key for your Airtable account and update the .env file with the appropriate values:
AIRTABLE_API_KEY_mine=patpEKdMxbHww2hZM.90fb5135d71f83b384f6696ef980861e9870de797c2d257efe232b30abcc4aea
AIRTABLE_BASE_ID_minw=MyBase
AIRTABLE_API_KEY=patpEKdMxbHww2hZM.0565912b06e99580f51d23f2501901b57a0d47ad9fa20636e0bc9991911d5e71
AIRTABLE_BASE_ID=appAjVTU4h7xB5QkA
AIRTABLE_TABLE_ID=tblwvxQhCHv4Plxxj
AIRTABLE_TABLE_NAME=Table 1
AIRTABLE_VIEW_NAME=MyView

OpenAI Integration
This project also integrates with OpenAI for natural language processing tasks. You need to obtain an API key from OpenAI and update the .env file with the key:
OPENAI_API_KEY=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

Additional Notes
Backup: A backup of the Airtable table (Table 1) in the specified view (MyView) has been provided as airtable_backup.csv.
Usage Instructions: Enter text in the textbox provided in the frontend UI to interact with the chatbot. You can upload PDF documents, ask questions, and receive summaries based on the content.
Contributing
Contributions are welcome! Feel free to submit issues or pull requests to improve the project.
