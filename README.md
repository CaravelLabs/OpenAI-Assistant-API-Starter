# OpenAI Assistant API Starter - Conversational Threads

A repository which leverages OpenAI's latest Assistant APIs to create conversational threads. Built on [Next.js](https://nextjs.org/) and uses [OpenAI's Assistant API](https://platform.openai.com/docs/assistants/overview)
## Environment Setup Instructions

### Pre requisites

- OpenAI API Key - You can obtain the API key by signing up at [OpenAI](https://platform.openai.com/signup/)
- OpenAI Assistant ID - You can obtain the Assistant ID by creating a new Assistant at [OpenAI Assistants](https://platform.openai.com/docs/assistants/overview)

**Note: You need to signup with a Credit Card to use Assistants API from OpenAI**

### Getting Started Steps

- Install dependencies from the `/web` folder - `npm install`

- Rename `.env.sample` to `.env` and set appropriate variables.

    - OPENAI_API_KEY - Your OpenAI API Key
    - OPENAI_ASSISTANT_ID - Your OpenAI Assistant ID
    - SITE_URL - Your site URL (for example, http://localhost:3000)

- Start the project - `npm run dev`

<br />
<br />

## Technical Documentation

### Tech Stack

| Name | Description |
| :--- | ---: |
| [Next.js](https://nextjs.org/) | React framework |
| [OpenAI's Assistant API](https://platform.openai.com/docs/assistants/overview) | API service to create conversational threads with OpenAI's custom Assistants that serve a niche purpose of your choice |
| [Azure App Service](https://learn.microsoft.com/en-us/azure/app-service/) | App Hosting PaaS |

<br />

### Folder Structure (for `/web/src`)
```bash
📦src
 ┣ 📂lib
 ┃ ┣ 📜read-data-stream.ts
 ┃ ┗ 📜stream-parts.ts
 ┣ 📂pages
 ┃ ┣ 📂api
 ┃ ┃ ┣ 📂assistant
 ┃ ┃ ┃ ┗ 📜index.ts
 ┃ ┃ ┗ 📜hello.ts
 ┃ ┣ 📜_app.tsx
 ┃ ┣ 📜_document.tsx
 ┃ ┗ 📜index.tsx
 ┣ 📂styles
 ┃ ┣ 📜Home.module.css
 ┃ ┗ 📜globals.css
 ┗ 📂utils
 ┃ ┗ 📜OpenAI.ts
```

<br />

### High Level Technical Architecture

<img src="https://ambitustemplateassets.blob.core.windows.net/assets/diagram-export-19-02-2024-19_24_08.png" width='100%' height='auto' />

<br />

### Cost to host in Azure

Official estimate from Azure Pricing Calculator - [Azure Pricing Calculator](https://azure.com/e/bbec79326663486ebfb3c76d30b1a9fc)

| Service Category | Service Type | Description | Estimated Monthly Cost | Estimated Upfront Cost |
| :---: | :---: | :---: | :---: | :---: |
| Compute | Azure App Service | *Basic Tier; 1 B1 (1 Core(s), 1.75 GB RAM, 10 GB Storage) x 730 Hours; Linux OS; 0 SNI SSL Connections; 0 IP SSL Connections; 0 Custom Domains; 0 Standard SLL Certificates; 0 Wildcard SSL Certificates* | $12.41 | $0 |
| Developer Tools | Azure DevOps | *Basic Plan; 5 User(s)* | $0 | $0 |
| Total | | | $12.41 | $0 |

***NOTE: This estimate does not include the costs that might be incurred in using OpenAI's services.***

***Disclaimer: The above cost is an estimate and may vary based on the actual usage. Caravel Labs or Microsoft is not responsible for additional costs incurred.***
