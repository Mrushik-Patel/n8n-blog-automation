# n8n Blog Automation 🚀

This project is an end-to-end blog automation system built using **n8n**, designed to automatically generate and publish blog posts from multiple RSS sources using AI-assisted workflows.

The automation handles content sourcing, keyword generation, blog writing, image generation, and publishing — all with minimal manual intervention.

---

## What This Automation Does

- Fetches articles from multiple RSS feeds (news & tech sources)
- Filters and processes feed data
- Generates blog keywords and titles using AI
- Creates full blog content automatically
- Generates meta descriptions
- Generates images for blog posts
- Publishes blogs to Blogger
- Logs published content to Google Sheets
- Manages API usage with key rotation and limits

---

## Workflow Overview

### 1. RSS Feed Triggers
Fetches data from multiple RSS sources:
- BBC Feed  
- Google News Feed  
- TechCrunch Feed  
- OpenAI RSS Feed  

### 2. Data Processing
- Merges RSS data into a single workflow
- Cleans and formats content using JavaScript nodes
- Filters duplicate entries and limits execution size

### 3. API Key Management
- Removes previously used API keys
- Applies request limits
- Rotates API keys automatically to avoid rate limits

### 4. AI Content Generation
Using AI models, the workflow:
- Generates SEO-friendly keywords
- Creates optimized blog titles
- Writes full blog content
- Generates meta descriptions

AI tools assist with content generation, while the workflow logic, sequencing, and automation design are implemented and controlled by me.

### 5. Image Generation & Publishing
- Generates images for each blog post
- Uploads images to Blogger
- Publishes blog posts automatically
- Logs results into Google Sheets for tracking

---

## Tools & Technologies Used

- n8n (workflow automation)
- JavaScript (custom logic inside n8n nodes)
- RSS Feeds
- Groq / AI APIs
- Image Generation API
- Google Sheets API
- Blogger API
- API key rotation & rate limiting

---

## My Contribution

- Designed the complete automation workflow from scratch
- Configured RSS triggers and data merging
- Implemented JavaScript logic for data processing
- Set up API key rotation and usage limits
- Integrated AI models for content, metadata, and image generation
- Automated blog publishing and logging
- Tested, debugged, and optimized the workflow

**Note:** AI tools were used as part of the automation process.  
I fully understand the workflow and can recreate, modify, or extend it independently.

---

## How to Use This Workflow

1. Install and run **n8n**
2. Import the provided workflow JSON file
3. Configure required API credentials (AI, Blogger, Google Sheets)
4. Set environment variables and usage limits
5. Run the workflow manually or schedule execution

---


## Use Case

This automation is suitable for:
- Automated content websites
- SEO-driven blog generation
- Marketing teams
- Experimenting with AI-powered publishing workflows

## Note

If you are running n8n **locally**, please replace the **RSS Feed Trigger** nodes with a **Manual Trigger** node and standard **RSS Read** nodes.

The RSS Feed Trigger nodes used in this workflow require **n8n cloud/online execution** and may not run as expected in a local n8n setup.


<img width="1352" height="623" alt="n8n-blog-workflow" src="https://github.com/user-attachments/assets/87366a5c-b319-4dee-bcce-57fae4d90ad3" />

