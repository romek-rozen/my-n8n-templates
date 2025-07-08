# Template submission guidelines

## 🔥 TLDR
🎯 **Your template [should look something like this](https://n8n.io/workflows/4817-composestitch-separate-images-together-using-n8n-and-gemini-ai-image-editing/)** 

📒 **Use sticky notes (it’s mandatory)**

🔐 **Don't use hardcoded API keys in the HTTP node**

📝 **Use markdown (not <HTML tags>) and `## H2 Headings`  for the description**

🚫 **Don't repost/steal other people's workflows (you’ll be banned)**

## 📌 General Guidelines

### ✅ What Makes a Template Successful
	•	Make your templates high quality and relevant to common user needs.
	•	Focus on real, practical use cases (eg. AI support chatbot, content creation, sales automation)
	•	Aim for broad appeal, but with enough specificity to be actionable (e.g., instead of “email notification,” go for “Slack DM for high-priority Zendesk ticket”).
	•	Be original. Check out our teamplte library to see what’s already out there and fill the gaps.

### ⛔ What Not to Do
	•	Do not plagiarize or resell someone else’s template (this will get your account banned)
	•	Do not submit low-effort templates (they won’t get published). Templates should demonstrate thoughtful design, utility, and real-world value.
	•	Do not ignore these guidelines – save yourself (and us) the back-and-forth on reviews and resubmissions.

## 📄 Description Page Guidelines (for SEO & Presentation)

### ✍️ Language & Formatting
	•	Write in clear, grammatically correct English. Use an AI to proofread your content.
	•	Use proper Markdown formatting. No <HTML tags> please.
	•	Use ## H2 Headings (not H1) to split your content into sections.

### 🔍 SEO Optimization
	•	Use main nodes in the title with sentence-style capitalization.
	•	The title should be in the following format:
Action verb thing being manipulated to/on/in/from where
Example: One-way contact sync from Pipedrive to HubSpot
	•	Avoid spammy, overhyped titles with emojis. Use a clear, objective title that reflects what the template does (if not, we’ll change it).
	•	Aim for ~200 words in the description.
    
### 🧾 Suggested Sections
	•	Who’s it for
	•	How it works / What it does
	•	How to set up
	•	Requirements
	•	How to customize the workflow

### ❗Special Cases
	•	If your template uses a community node, add:
	•	A disclaimer that it’s self-hosted only.
	•	A workflow image at the top (since previews don’t render).

## 🛠️ Workflow Guidelines

### 🧱 Structure & Clarity
	•	Rename all nodes to describe their purpose.
	•	Use Sticky notes for context and instructions.
	•	Always include one (preferably yellow color) that explains the template. Include the entire description in it.
	•	Link to external setup guides (e.g., Notion) if needed.
	•	Use additional sticky notes (preferably neutral / white color) to outline individual steps. Here’s an example.
	•	Do embed Youtube videos and images in sticky notes.
	•	Consider adding a quick Loom video for setup (optional but highly encouraged).

### 🔐 Best Practices
	•	Follow security guidelines (e.g., don’t store credentials directly in the HTTP node)
	•	Don’t forget to remove personal identifiers like Google Sheets IDs, Telegram channels, real email addresses, etc.
	•	Use the Set Fields node to group variables the user needs to configure.

### 🧠 User Empathy
	•	Assume the user may be new to n8n.
	•	Minimize friction by making the workflow plug-and-play where possible.

## 💰 Payment Guidelines

### 🚀 Becoming a Verified Creator
	•	You must submit at least 3 high-quality templates to become eligible to offer paid templates.

### 🛒 Selling Templates
	•	Paid templates must:
	•	Be delivered reliably after purchase (you’re the one responsible for tracking incoming payments and delivering the template).
	•	Remain accessible to the buyer.

### ⚠️ Enforcement
	•	Failure to deliver a paid template may result in account suspension or banning.

## To do for submission
- [ ] Create Template name e.g. Enrich new HubSpot contacts and deals with Clearbit. File name: template_name.txt
- [ ] Description. File name: template_description.txt
  - How it works
    - Distill what your flow does in a few high-level steps
  - Set up steps
    - Give users an idea of how long set up will take. Don't describe every detail.
	- Keep detailed descriptions in sticky notes inside your workflow