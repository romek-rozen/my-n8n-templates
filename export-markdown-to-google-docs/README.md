# 📝 Export Markdown Content to Google Docs Document

Convert Markdown content to Google Docs document with automatic formatting, timestamping, and Drive organization.

![n8n workflow](https://img.shields.io/badge/n8n-workflow-FF6D5A?style=flat-square&logo=n8n)
![Google Drive](https://img.shields.io/badge/Google%20Drive-integration-4285F4?style=flat-square&logo=google-drive)
![Markdown](https://img.shields.io/badge/Markdown-support-000000?style=flat-square&logo=markdown)

## 🎯 Who is this for?

This workflow is perfect for **technical writers**, **content creators**, **marketers**, and **developers** who write in Markdown but need to collaborate or publish using Google Docs format. Ideal for teams that want to streamline their content creation and review process.

## 🔧 What problem does this workflow solve?

Manual conversion from Markdown to Google Docs is time-consuming and often loses formatting. This workflow eliminates the tedious copy-paste process, automatically preserves formatting, and creates organized, timestamped documents in your Google Drive. Perfect for content teams who write in Markdown but need Google Docs for collaboration and review.

## ✨ What this workflow does

- **Converts Markdown to HTML** with proper formatting preservation (headers, lists, links, tables)
- **Creates timestamped Google Docs** documents with automatic naming
- **Adds Drive location metadata** for better organization and reference
- **Maintains document structure** including emojis, tables, and text formatting
- **Automates file creation** in specified Google Drive folders

## 📋 Prerequisites

- **n8n instance** (local or cloud) - version 1.0.0+
- **Google account** with Google Drive access
- **Basic understanding** of n8n workflow configuration

## 🚀 Quick Setup

### Step 1: Import the Workflow

1. **Open n8n** and navigate to `Workflows`
2. **Click** "Add workflow" → "Import from JSON"
3. **Upload** the `export-markdown-to-google-docs.json` file
4. **Save** the workflow with a descriptive name

### Step 2: Configure Google Drive Credentials

#### Create Google Drive OAuth2 Credentials

1. **In n8n**, go to `Settings` → `Credentials`
2. **Click** "Add credential" → "Google Drive OAuth2 API"
3. **Follow the OAuth setup** to authorize n8n access to Google Drive:
   - Visit Google Cloud Console
   - Create or select a project
   - Enable Google Drive API
   - Create OAuth2 credentials
   - Add authorized redirect URI for your n8n instance
4. **Name the credential** (e.g., "Google Drive - Markdown Converter")

#### Configure Google Drive Nodes

**Update these nodes with your Google Drive credentials:**
- `Create Empty File`
- `Update Document with Correct HTML Formatting`

**In each node:**
1. **Select your Google Drive credential** from the dropdown
2. **Test the connection** to ensure it works properly

### Step 3: Prepare Your Google Drive

1. **Go to Google Drive** (drive.google.com)
2. **Create a new folder** for your converted documents
3. **Copy the folder URL** (format: `https://drive.google.com/drive/folders/FOLDER_ID`)
4. **Ensure the folder has proper permissions** for your Google account

### Step 4: Configure Input Data

1. **Open the "Set Input Data" node**
2. **Update the assignments** with your preferences:

   **Google Drive URL:**
   ```
   https://drive.google.com/drive/folders/YOUR_FOLDER_ID
   ```

   **Content Title:**
   - Set a default title or leave placeholder text
   - This will be used in the document filename

   **Content in Markdown:**
   - Add your Markdown content or keep example for testing
   - Supports standard Markdown syntax (headers, lists, links, tables)

## 📖 How to Use

1. **Configure Google Drive credentials** in n8n settings
2. **Update "Set Input Data" node** with:
   - Google Drive URL (target folder)
   - Content Title (document name)
   - Content in Markdown (your text)
3. **Click "Test workflow"** to execute
4. **Check your Google Drive** for timestamped document

## 🎨 Customization Options

### Modify HTML Formatting Options

**In the "Change Markdown To HTML" node:**
- **Enable/disable emoji support** (currently enabled)
- **Adjust table formatting** (currently enabled)
- **Modify header ID generation** (currently disabled)
- **Configure space requirements** for headers

### Update File Naming Pattern

**In the "Create Empty File" node:**
- **Change the naming convention**: Currently uses `_PUB {Content Title} {timestamp}`
- **Modify timestamp format**: Currently `yyyy-MM-dd HH:mm:ss`
- **Add prefixes or suffixes** as needed for your organization

### Adjust Drive Location Metadata

**In the "Add Information About Google Drive Location" node:**
- **Modify the HTML template** that gets added to documents
- **Change the link text and formatting**
- **Add additional metadata** as needed

### Configure MIME Type Handling

**In the "Change Mime Type of The File" node:**
- **Adjust MIME type conversion** if needed
- **Add additional file processing** logic
- **Modify binary data handling**

## 💡 Use Cases

- **Technical documentation** (README → Google Docs)
- **Content publishing workflow** (draft → review)
- **Blog/article preparation** (Markdown → collaborative editing)
- **Report generation** with automated formatting
- **Team collaboration** on written content
- **Documentation standardization** across projects

## 🔧 Troubleshooting

### Google Drive Permission Errors
- Verify OAuth2 credentials are properly configured
- Check that the target folder exists and is accessible
- Ensure Google Drive API is enabled in Google Cloud Console

### Markdown Conversion Issues
- Check that your Markdown syntax is valid
- Test with simple content first (headers, paragraphs, lists)
- Verify the "Change Markdown To HTML" node settings

### File Creation Problems
- Confirm the Google Drive folder URL format is correct
- Check that the folder ID in the URL is valid
- Ensure your Google account has write permissions to the folder

### Common Solutions
- **Timeout errors**: Increase wait time in "Wait for Document Creation"
- **Authentication failures**: Refresh Google OAuth2 credentials
- **Formatting issues**: Test with simpler Markdown first

## ⚙️ Advanced Configuration

### Batch Processing

To process multiple documents:
1. **Modify the input node** to accept arrays of content
2. **Add loop functionality** using Split In Batches node
3. **Implement error handling** for failed conversions

### Integration Options

**Webhook Integration:**
- Add a Webhook trigger to accept external Markdown content
- Useful for automated content publishing workflows

**Schedule Integration:**
- Add Schedule trigger for regular document generation
- Process queued content at specific intervals

**Email Integration:**
- Add email notifications when documents are created
- Include links to generated Google Docs

### Performance Optimization

- Adjust the "Wait for Document Creation" timing if needed
- Optimize for larger documents by increasing wait time
- Consider file size limits for Google Docs

## 📁 Project Files

- `export-markdown-to-google-docs.json` - Main n8n workflow file
- `description.txt` - Detailed workflow description and features
- `setup-instructions.txt` - Comprehensive setup guide
- `sticky-note-content.txt` - Quick reference guide
- `template-name.txt` - Template name for submissions
- `template-submission-guidelines.md` - Guidelines for template submissions
- `README.md` - This documentation file

## 📊 Workflow Details

**Total setup time:** ~15-20 minutes  
**Difficulty level:** Intermediate  
**Requirements:** Google account, n8n instance, basic OAuth2 setup knowledge

## 🎯 Key Features

- ✅ **Automatic formatting preservation**
- ✅ **Timestamped document creation**
- ✅ **Metadata injection**
- ✅ **Emoji and table support**
- ✅ **Customizable naming patterns**
- ✅ **Error handling**
- ✅ **Easy customization**

## Support

If you find this template useful, consider [supporting my work](https://github.com/sponsors/romek-rozen)!
