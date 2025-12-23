# 🛠️ Workflow Recipes: Learning n8n Automation One Recipe at a Time

**One workflow every Monday. Built from scratch. Tested thoroughly. Shared honestly.**

[![Newsletter](https://img.shields.io/badge/Subscribe-Weekly_Recipes-blue?style=for-the-badge)](https://workflowrecipes.co) 
[![n8n](https://img.shields.io/badge/Built_with-n8n-orange?style=for-the-badge&logo=n8n)](https://n8n.io)
[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)

---

## 📖 What is This?

I'm learning n8n automation by building one workflow every week and documenting everything I discover.

Every Monday, I share:
- ✅ **A working workflow** (tested until it actually works)
- ✅ **What broke during the build** (error messages, wrong assumptions, dead ends)
- ✅ **How I fixed it** (what I Googled, what worked, what didn't)
- ✅ **What I learned** (concepts that clicked, "aha!" moments, resources that helped)

This is **learning in public**. No fake expertise. No polished tutorials that skip the messy parts. Just honest documentation of one person's journey from n8n beginner to (eventually) competent.

**If you're also learning automation, follow along. We'll figure this out together.**

---

## 🗂️ Available Recipes

> **Note:** I build and test one new recipe each week. Only workflows that actually work are published here.

### 🟢 Recipe #0: n8n Setup Guide
**What I learned:** Getting n8n running (cloud vs self-hosted)  
📁 [View Guide](recipes/000-n8n-setup/)

---

### 🟢 Recipe #1: Email Attachments → Auto-Filed in Google Drive
**The challenge:** Automatically file email attachments into Google Drive folders  
**What I built:** Gmail trigger → Extract attachments → Upload to Drive with smart naming  
**What broke:** Gmail trigger didn't work (forgot to enable IMAP), special characters in filenames broke uploads  
**What I learned:** How OAuth works, regex for filename sanitization, the difference between polling and webhook triggers  
**Testing:** Ran for 5 days, processed 15 test emails, hit 2 errors, fixed both  

📁 [View Recipe](recipes/001-email-attachments-to-drive/) | 📥 [Download JSON](recipes/001-email-attachments-to-drive/workflow.json)

**Includes:**
- Working workflow (import and run)
- Step-by-step setup with screenshots
- Every error I encountered + solutions
- What I'd do differently next time

---

### 🔄 Recipe #2: Customer Emails → Google Sheets Tracking
**Status:** Building this week (testing Dec 30-Jan 5)

---

### 📝 Recipe #3: Form Responses → Email + Sheets
**Status:** Starting next week

---

## 🚀 How to Use These Workflows

### Prerequisites
- An n8n instance ([setup guide](recipes/000-n8n-setup/) or use [n8n cloud](https://n8n.io))
- Gmail account (for most recipes)
- Google Drive/Sheets access
- Patience for troubleshooting (it won't work perfectly first try)

### Import and Test

1. **Pick a recipe** from the list above
2. **Read the README** in the recipe folder (has my full notes)
3. **Download the JSON** workflow file
4. **Import to n8n:**
   - Workflows → Import from File → Select JSON
5. **Configure credentials:**
   - Click nodes with warning icons
   - Add your Gmail/Drive credentials
   - Follow setup guide for specifics
6. **Test first:**
   - Click "Execute Workflow" button
   - Check execution log for errors
   - If it breaks, check the README troubleshooting section
7. **Activate when working:**
   - Toggle to Active
   - Monitor for a day or two

---

## 📬 Follow My Learning Journey

I publish one new recipe every Monday (8am AEST).

Each week you get:
- The workflow I built (with full code)
- What I was trying to solve
- What broke and how I debugged it
- What I learned this week
- Resources that helped me

**No fluff. No "expert" posturing. Just honest learning documentation.**

**👉 [Subscribe at workflowrecipes.co](https://workflowrecipes.co)**

---

## 🤔 Why Follow This?

**vs. Expert tutorials:**
- ✅ Beginner teaching beginners (more relatable)
- ✅ I show the mistakes, not just the solution
- ✅ Plain English, not jargon
- ✅ "Here's what I Googled" transparency

**vs. Official docs:**
- ✅ Practical projects, not feature lists
- ✅ Complete workflows you can copy
- ✅ Troubleshooting from real errors
- ✅ Learning progression (simple → complex)

**vs. Figuring it out alone:**
- ✅ Structured weekly path
- ✅ Someone who just learned it (not an expert from 5 years ago)
- ✅ Community of other learners
- ✅ Tested workflows that actually work

---

## 🛠️ Recipe Structure

Each recipe folder contains:
```
recipes/001-email-attachments-to-drive/
├── README.md              # Setup guide, what I learned, troubleshooting
├── workflow.json          # The working workflow (import this)
├── screenshots/           # Visual guide to setup
│   ├── gmail-trigger.png
│   ├── drive-upload.png
│   └── final-result.png
└── LEARNINGS.md           # My personal notes (mistakes, aha moments)
```

---

## 💡 My Learning Philosophy

**"Build it until it works, then share everything"**

Every recipe here:
1. Was built from scratch (not copied from tutorials)
2. Broke at least once during development
3. Was tested thoroughly (5-7 days minimum)
4. Includes the real problems I encountered
5. Is something I'd actually use

I'm not an expert. I'm just documenting what I learn as I build one workflow per week.

**Learning in public is messy. That's the point.**

---

## 🗺️ My Learning Roadmap

**Current focus (Recipes 1-10 - Beginner):**
- ✅ Email attachments → Google Drive (simple triggers)
- 🔄 Customer emails → Sheets (data extraction)
- 📝 Form responses → Email + Sheets (multi-step flows)
- 📝 Invoice reminders (scheduled workflows)
- 📝 Weekly reports (data aggregation)
- 📝 Client intake (complex multi-step)
- 📝 Expense tracking (email parsing)
- 📝 Appointment automation (calendar integration)
- 📝 Testimonial collection (web hooks)
- 📝 Lead magnet delivery (conditional logic)

**Next phase (Recipes 11-20 - Intermediate):**
- API integrations
- Error handling patterns
- Performance optimization
- Advanced data transformation

**Eventually (Recipes 21+ - Advanced):**
- AI integrations
- Complex multi-workflow systems
- Custom code nodes
- Production-grade error recovery

---

## 🤝 Learning Together

**Found an error in my workflow?** Please tell me! Open an issue.

**Have a suggestion?** Fork, improve, and submit a PR.

**Want to request a workflow?** [Open a discussion](../../discussions) - if I don't know how to build it yet, we can learn together.

**Built something cool?** Share it! This is a learning community.

---

## 📊 My Progress

**Week 0 (Dec 23-29):** Building Recipe #1  
**Week 1 (Dec 30-Jan 5):** Documenting Recipe #1, setting up infrastructure  
**Week 2 (Jan 6):** Publishing Recipe #1, starting Recipe #2  

**Goal:** 52 workflows in Year 1  
**Current:** 1 completed, 51 to go  

---

## 📄 License

MIT License - Use these workflows however you want. Learn from them, improve them, share them.

---

## 📞 Connect

- 📧 **Newsletter:** [workflowrecipes.co](https://workflowrecipes.co)
- 🐦 **Twitter/X:** [@workflowrecipes](https://twitter.com/workflowrecipes) *(coming soon)*
- 💬 **Discussions:** [GitHub Discussions](../../discussions)

---

**Learning n8n one workflow at a time. Join me on the journey.**
