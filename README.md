# 🛠️ Workflow Recipes: n8n Automations That Actually Work

**One copy-paste recipe every Monday. Tested on real businesses. 15-minute setup.**

[![Newsletter](https://img.shields.io/badge/Subscribe-Weekly_Recipes-blue?style=for-the-badge)](https://workflowrecipes.co) 
[![n8n](https://img.shields.io/badge/Built_with-n8n-orange?style=for-the-badge&logo=n8n)](https://n8n.io)
[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)

---

## 📖 What is This?

Small business owners and solopreneurs waste **5-15 hours per week** on repetitive admin tasks:
- Manually downloading invoice PDFs and filing them
- Copy-pasting customer emails into spreadsheets
- Sending the same follow-up emails over and over
- Tracking payments and chasing late invoices

This repository contains **human-tested n8n workflows** that automate these tasks. Each recipe:

✅ **Runs in one tool** (n8n - free and self-hostable)  
✅ **Takes 10-15 minutes to set up** (import JSON, tweak credentials, activate)  
✅ **Includes troubleshooting** (real problems I hit and how I solved them)  
✅ **Shows actual time saved** (tested on my own business for 5-7 days)  

**No coding required. No tool-hopping. Just working automations.**

---

## 🗂️ Available Recipes

> **Note:** I build and test one new recipe each week. Only proven workflows are published here.

### 🟢 Recipe #0: n8n Setup Guide
**Get n8n running in 10 minutes** (self-hosted or cloud)  
📁 [View Guide](recipes/000-n8n-setup/)

---

### 🟢 Recipe #1: Email Attachments → Auto-Filed in Google Drive
**Problem:** Manually downloading 20-50 invoices/receipts per month and organizing folders  
**Solution:** Automatically scan Gmail, extract attachments, file in Drive by client/date  
**Time Saved:** 3-4 hours/month  
**Setup:** 15 minutes

📁 [View Recipe](recipes/001-email-attachments-to-drive/) | 📥 [Download JSON](recipes/001-email-attachments-to-drive/workflow.json)

**Includes:**
- Standard version (max reliability)
- AI-enhanced version (smarter file naming)
- Troubleshooting guide
- Screenshots

---

### 🔵 Recipe #2: Customer Emails → Google Sheets Tracking
**Status:** Currently testing (launches Week 2)

---

### 🔵 Recipe #3: Form Responses → Email + Sheets
**Status:** Building next week

---

## 🚀 Quick Start

### Prerequisites
- An n8n instance ([self-host guide](recipes/000-n8n-setup/) or use [n8n cloud](https://n8n.io) - $20/month)
- Gmail account (for most recipes)
- Google Drive/Sheets access

### How to Use a Recipe

1. **Browse the recipes above** and pick one that solves your problem
2. **Read the recipe README** in its folder (has setup instructions + screenshots)
3. **Download the JSON file** from the recipe folder
4. **Import to n8n:**
   - Open n8n
   - Click **Workflows** → **Import from File**
   - Select the downloaded JSON
5. **Configure credentials:**
   - Click on each node with a warning icon
   - Add your Gmail/Drive/Sheets credentials
   - Follow the recipe's setup guide for any specific settings
6. **Test it:**
   - Click **Execute Workflow** to test
   - Check the recipe README for common errors
7. **Activate:**
   - Toggle the workflow to **Active**
   - Let it run and monitor for 1-2 days

---

## 📬 Get New Recipes Every Monday

I publish one new recipe each week (Mondays, 8am AEST).

Each recipe includes:
- The problem it solves (with real time-saved data)
- Standard version (no AI, max reliability)
- AI-enhanced version (when it adds value)
- Step-by-step setup guide
- Troubleshooting from real errors I hit
- Screenshots and examples

**👉 [Subscribe at workflowrecipes.co](https://workflowrecipes.co)**

---

## 🤔 Why These Recipes?

**vs. n8n's official templates:**
- ✅ Tested on real business data (not theoretical examples)
- ✅ Includes "gotchas" I discovered (things that break and how to fix them)
- ✅ Focused on small business pain points (not enterprise use cases)
- ✅ Plain-English instructions (zero experience assumed)
- ✅ Time-saved metrics from actual usage

**vs. Building from scratch:**
- ✅ Already debugged and working
- ✅ 15-min import vs. 2-4 hour build
- ✅ Proven to handle real-world edge cases

---

## 🛠️ Recipe Structure

Each recipe folder contains:
```
recipes/001-email-attachments-to-drive/
├── README.md              # Setup guide, troubleshooting, screenshots
├── workflow.json          # Standard version (import this first)
├── workflow-ai.json       # AI-enhanced version (optional)
├── screenshots/           # Visual guide
│   ├── setup-step-1.png
│   ├── setup-step-2.png
│   └── final-result.png
└── LEARNINGS.md           # What I discovered building this
```

---

## 💡 Philosophy

**"I run this myself"**

Every recipe in this repo:
1. Runs in my own business (not theoretical)
2. Has been tested for at least 5-7 days
3. Includes real problems I encountered
4. Shows actual time saved (not estimates)

I'm learning n8n in public and sharing working recipes as I build them.

---

## 🗺️ Roadmap

**Current focus (Recipes 1-10):**
- ✅ Email attachments → Google Drive
- 🔄 Customer emails → Sheets tracking (testing now)
- 📝 Form responses → Email + Sheets
- 📝 Unpaid invoices → Payment reminders
- 📝 Weekly business report generation
- 📝 New client intake automation
- 📝 Expense tracking from email
- 📝 Appointment confirmation automation
- 📝 Testimonials → Google Docs
- 📝 Lead magnet delivery automation

**Future (Recipes 11-20):**
- Calendar management
- Social media workflows  
- Advanced AI integrations
- Multi-step business processes

---

## 🤝 Contributing

Found a bug in a recipe? Have a suggestion?

1. **Issues:** Open an issue describing the problem
2. **Improvements:** Fork, fix, and submit a PR
3. **Requests:** What workflow should I build next? [Open a discussion](../../discussions)

---

## 📄 License

MIT License - Use these recipes however you want.

---

## 📞 Connect

- 📧 **Newsletter:** [workflowrecipes.co](https://workflowrecipes.co)
- 🐦 **Twitter/X:** [@workflowrecipes](https://twitter.com/workflowrecipes) *(coming soon)*
- 💼 **LinkedIn:** [Your LinkedIn] *(coming soon)*

---

**Built with ☕ by a solopreneur who got tired of manual admin.**
