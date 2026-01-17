# Contact Generator - Complete Setup Guide

**You've never done this before? No problem!** This guide assumes zero technical knowledge.

---

## 📦 What You Have

On your Desktop, you now have 3 files:

1. **contact-generator.html** - The web tool (opens in browser)
2. **contact-generator-custom-gpt-instructions.md** - Instructions for ChatGPT
3. **SETUP-GUIDE.md** - This file you're reading

---

## 🎯 Setup Overview (3 Main Steps)

1. **Test the HTML tool locally** (5 minutes)
2. **Host the HTML tool online** (10 minutes)
3. **Create Custom GPT in ChatGPT** (5 minutes)

**Total time: ~20 minutes**

---

# STEP 1: Test the HTML Tool Locally

Let's make sure the tool works before we put it online.

## Mac Instructions:

1. **Find the file** on your Desktop: `contact-generator.html`
2. **Double-click it** → It will open in Safari (or your default browser)
3. **You should see** a purple gradient page with "📇 Contact Generator" at the top

### Quick Test:

1. In the paste box, paste this test data:
```
contactType=Person
firstName=John
lastName=Smith
company=TestCo - Owner - Test Contact - 🇲🇹
phone1=+356 9999 8888
phone1Label=Mobile
email1=john@test.com
email1Label=Email
```

2. Click **"📋 Parse & Fill"**
3. All fields should auto-fill
4. Click **"⬇️ Generate & Download .vcf"**
5. A file should download to your Downloads folder
6. **Double-click the .vcf file** → It should open Contacts and offer to import

**✅ If this worked, you're ready for Step 2!**

**❌ If it didn't work:**
- Make sure you're using a modern browser (Safari, Chrome, Firefox)
- Check Downloads folder permissions
- Try again with a fresh browser window

---

# STEP 2: Host the HTML Tool Online

Now we need to put the tool on the internet so you can access it from your iPhone.

## Option A: GitHub Pages (Recommended - Free Forever)

**What is GitHub?** A website where people store code. It offers free hosting.

### Step-by-Step:

#### 1. Create GitHub Account (if you don't have one)

1. Go to https://github.com
2. Click **"Sign up"**
3. Follow the prompts:
   - Enter your email
   - Create a password
   - Choose a username
   - Verify you're human
4. Check your email and verify your account

#### 2. Create a New Repository

1. Click the **"+"** icon (top right corner)
2. Click **"New repository"**
3. Fill in:
   - **Repository name:** `contact-generator` (lowercase, no spaces)
   - **Description:** "Apple Contacts VCF Generator" (optional)
   - **Public** (must be public for free hosting)
   - ✅ Check **"Add a README file"**
4. Click **"Create repository"**

#### 3. Upload Your HTML File

1. On the repository page, click **"Add file"** → **"Upload files"**
2. **Drag and drop** `contact-generator.html` from your Desktop
3. Scroll down and click **"Commit changes"** (green button)

#### 4. Enable GitHub Pages

1. Click **"Settings"** (top menu, right side - looks like a gear ⚙️)
2. In the left sidebar, click **"Pages"** (under "Code and automation")
3. Under **"Source"**, select:
   - Branch: **main**
   - Folder: **/ (root)**
4. Click **"Save"**
5. **Wait 1-2 minutes** for GitHub to build your site
6. Refresh the page - you'll see a blue/green box that says:
   **"Your site is published at https://[your-username].github.io/contact-generator/"**

#### 5. Get Your URL

Your tool is now live at:
```
https://[your-username].github.io/contact-generator/contact-generator.html
```

**Example:** If your username is `johnsmith`, your URL is:
```
https://johnsmith.github.io/contact-generator/contact-generator.html
```

### Test It:

1. **Copy your URL** (the one with your username)
2. **Open it in a browser**
3. **Open it on your iPhone** Safari
4. It should work exactly like it did on your computer!

**🎉 Success!** Now you have a permanent, free URL for your tool.

---

## Option B: Dropbox (Alternative - Simpler but Temporary Links)

**If you have Dropbox:**

1. Put `contact-generator.html` in your Dropbox folder
2. Right-click the file → **"Share"** → **"Create a link"**
3. Copy the link
4. **Change** `www.dropbox.com` to `dl.dropboxusercontent.com` in the URL
5. **Change** `?dl=0` at the end to `?raw=1`

**Example:**
- Original: `https://www.dropbox.com/s/abc123/contact-generator.html?dl=0`
- Changed to: `https://dl.dropboxusercontent.com/s/abc123/contact-generator.html?raw=1`

**Note:** Dropbox links can expire. GitHub Pages is more reliable.

---

## Option C: Google Drive (Alternative - Works but Clunky)

**Not recommended** - Google Drive doesn't serve HTML files directly in a user-friendly way. Stick with GitHub Pages.

---

# STEP 3: Create Custom GPT in ChatGPT

Now let's create the ChatGPT assistant that helps you fill in contact details.

## Prerequisites:

- **ChatGPT Plus subscription** ($20/month) - Custom GPTs require this
- If you don't have Plus, you can still use ChatGPT to help format contacts, but you won't get the streamlined experience

## Step-by-Step:

### 1. Open ChatGPT

Go to https://chat.openai.com (or open the app on your phone)

### 2. Access GPT Builder

**On Desktop:**
1. Click **"Explore GPTs"** (left sidebar)
2. Click **"Create"** (top right)

**On iPhone:**
1. Tap your profile icon (bottom right)
2. Tap **"My GPTs"**
3. Tap **"+"** (top right)

### 3. Switch to Configure Tab

1. You'll see two tabs: **"Create"** and **"Configure"**
2. Click/tap **"Configure"**

### 4. Fill in Basic Info

1. **Name:** `Contact Generator Assistant`
2. **Description:** `Helps you create properly formatted Apple Contacts (.vcf files) with guided field-by-field input and validation.`
3. **Instructions:** This is the big one - open the file on your Desktop called:
   `contact-generator-custom-gpt-instructions.md`
4. **Copy everything** under the "Instructions" section (starts with "You are a Contact Generator Assistant...")
5. **Paste** into the Instructions box in GPT Builder

### 5. Update the URL in Instructions

**IMPORTANT:** Find this line in the instructions you just pasted:

```
🔗 **Step 2:** [Click here to open Contact Generator](YOUR_HOSTED_URL_HERE)
```

Replace `YOUR_HOSTED_URL_HERE` with your actual GitHub Pages URL:

```
🔗 **Step 2:** [Click here to open Contact Generator](https://your-username.github.io/contact-generator/contact-generator.html)
```

### 6. Add Conversation Starters (Optional but Helpful)

Scroll down to **"Conversation starters"** and add:

```
Create a new person contact
```
```
Create a new company contact
```
```
Show me all available fields
```

### 7. Save Your GPT

1. Click **"Save"** (top right)
2. Choose **"Only me"** (unless you want to share with others)
3. Click **"Confirm"**

**🎉 Done!** Your Custom GPT is ready!

---

# 🚀 How to Use (Complete Workflow)

## On iPhone (Recommended):

### Step 1: Open Custom GPT in ChatGPT App

1. Open ChatGPT app
2. Tap **"Explore GPTs"** (bottom)
3. Tap **"My GPTs"**
4. Select **"Contact Generator Assistant"**

### Step 2: Chat to Create Contact

```
You: "Create contact for John Smith at CleanHouse"

GPT: "👋 Welcome to Contact Generator!
[Shows all available fields]

First, is this a Person or Company?"

You: "Person"

GPT: "Let's start with basic info:
1. First Name?
2. Last Name?
3. Company/organization?"

You: "John Smith, CleanHouse"

[Continue answering questions...]
```

### Step 3: Copy & Use Web Tool

1. When GPT finishes, it shows:
   - **Formatted contact data** (copy this)
   - **Link to web tool** (tap this)
2. Safari opens with the tool
3. **Paste** the data into the text box
4. Tap **"📋 Parse & Fill"**
5. Review the fields
6. Tap **"⬇️ Generate & Download .vcf"**
7. **Open** the downloaded .vcf file
8. Tap **"Add All [X] Contacts"** in Contacts app

**Done! Contact imported!**

---

## On Desktop:

Same workflow, but:
- Use ChatGPT website instead of app
- Click links instead of tapping
- Browser opens the tool automatically

---

# 📱 Pro Tips

## Save to iPhone Home Screen (Makes it Like an App):

1. Open your GitHub Pages URL in Safari on iPhone
2. Tap the **Share** button (square with arrow)
3. Scroll down and tap **"Add to Home Screen"**
4. Name it **"Contact Generator"**
5. Tap **"Add"**

Now you have a "Contact Generator" icon on your home screen!

## Bookmark for Quick Access:

**On iPhone Safari:**
1. Open the tool URL
2. Tap **Share** → **"Add Bookmark"**
3. Save to **"Favorites"**

**On Desktop:**
- Chrome: Press `Cmd + D` (Mac) or `Ctrl + D` (Windows)
- Safari: Press `Cmd + D`

---

# 🔧 Troubleshooting

## "The tool won't download the .vcf file"

**Solution:**
- Check browser permissions for downloads
- Try a different browser (Chrome, Firefox, Safari)
- Make sure pop-ups aren't blocked

## "GitHub Pages isn't working"

**Check:**
1. Did you enable GitHub Pages in Settings → Pages?
2. Did you wait 1-2 minutes after enabling?
3. Is your repository set to **Public**?
4. Try the URL with `/contact-generator.html` at the end

## "Custom GPT won't let me create it"

**Check:**
- Do you have ChatGPT Plus subscription?
- Are you logged in to the correct account?

## "The paste function doesn't work"

**Try:**
- Click directly in the text box first
- Use `Cmd+V` (Mac) or `Ctrl+V` (Windows)
- Make sure you copied the formatted data from GPT (not the raw chat)

---

# 🆘 Need Help?

If you're stuck:

1. **Read the error message carefully** - it usually tells you what's wrong
2. **Google the error** - someone else has probably had the same issue
3. **Check GitHub's documentation:** https://docs.github.com/pages
4. **Ask ChatGPT for help** - describe the error you're seeing

---

# ✅ Final Checklist

Before you're done, verify:

- [ ] HTML tool works on your computer
- [ ] Tool is hosted online (GitHub Pages or Dropbox)
- [ ] You can access the tool from your iPhone
- [ ] Custom GPT is created in ChatGPT
- [ ] Custom GPT has the correct URL in instructions
- [ ] You've tested the complete workflow once
- [ ] Tool successfully creates and downloads .vcf files
- [ ] .vcf files import into Contacts app correctly

**All checked?** 🎉 **You're all set!**

---

# 📝 Next Steps

Now you can:
- Create contacts whenever you need them
- Share the tool URL with friends (if you want)
- Customize the tool (colors, fields, etc.) by editing the HTML
- Create more Custom GPTs for other tasks

**Enjoy your new contact creation workflow!** 📇✨
