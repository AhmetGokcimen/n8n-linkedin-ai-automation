# LinkedIn AI Post Automation (n8n)

This n8n workflow fully automates the process of creating and publishing engaging content on LinkedIn. It utilizes Generative AI to write professional posts, generates relevant images, and handles the publishing process automatically.

![Workflow Diagram](preview.png)
## 🚀 Features

* **AI Content Generation:** Uses **Google Gemini** to write engaging, trend-aware LinkedIn posts based on defined topics.
* **Dynamic Image Creation:** Generates a custom image prompt based on the post text and creates a visual using **Replicate (Imagen-4-fast)**.
* **Automated Publishing:** Posts the text and image directly to your **LinkedIn** profile via API.
* **History & Context:** Logs published posts to a **Supabase** database to maintain context and ensure future posts are sequential (e.g., "AI Insights #5").

## 🛠️ Prerequisites

To use this workflow, you need credentials for the following services:
* **n8n** (Self-hosted or Cloud)
* **Google Gemini (PaLM) API** (for text generation)
* **Replicate API** (for image generation)
* **Supabase** (for database/logging)
* **LinkedIn API** (OAuth2 for publishing)

## ⚙️ Setup & Usage

1.  **Download:** Download the `n8n-linkedin-automation.json` file from this repository.
2.  **Import:** Go to your n8n dashboard, click **"Add Workflow"** > **"Import from..."** and select the JSON file.
3.  **Credentials:**
    * Open the nodes with warning signs (red triangles).
    * Create or select your own credentials for Google Gemini, Replicate, Supabase, and LinkedIn.
4.  **Database:** Ensure you have a table in Supabase (e.g., `LinkedInPosts`) with columns matching the workflow logic (or adjust the node to match your table).
5.  **Activate:** Toggle the workflow to **Active** to start the schedule.

## 📄 License

This project is open-source and available for personal or educational use.
