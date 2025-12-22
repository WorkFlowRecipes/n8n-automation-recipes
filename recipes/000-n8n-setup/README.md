# 000 – n8n Master Setup (15 Minutes)

This quick-start guide gets you from **zero → ready to import recipes** in about 15 minutes.

You have two options:

- **Option A (easiest):** n8n Cloud (hosted)  
- **Option B (cheapest):** Self-hosted (your own server)

---

## ✅ Option A – n8n Cloud (Recommended for Beginners)

1. Go to https://n8n.io and click **Start for free**.  
2. Create an account and workspace.  
3. Once inside, click **Workflows → New** to confirm it loads.  
4. You’re done – you can now import any JSON recipe from this repo.

Use this if you want zero server management and are OK with a monthly fee once the trial ends.

---

## ✅ Option B – Self-Hosted (Budget-Friendly)

> If you already followed the full self-host guide from the welcome email, you can skip this section.

Basic steps (high level):

1. **Provision a server**  
   - Create a small VPS (e.g. DigitalOcean $6/month, 1GB RAM).  
   - Point a subdomain like `n8n.yourdomain.com` to the server IP.

2. **Install n8n with Docker**  
   - Install Docker and Docker Compose.  
   - Run the official `n8nio/n8n` image with a persistent volume.

3. **Secure with SSL**  
   - Use a reverse proxy (Nginx) + Let’s Encrypt for HTTPS.

Once you can open your n8n instance in the browser and log in, you’re ready to use recipes.

*(Full step-by-step instructions are in your welcome email and on workflowrecipes.co.)*

### 🎥 External walkthrough (optional)

If you prefer a visual guide, this video shows how to set up n8n on DigitalOcean step-by-step 
(not made by me, but very helpful):

[Watch on YouTube] 
https://www.youtube.com/watch?v=hO_KWrosh7M

This is a third-party video; details may change over time

---

## 🎯 Next Step – Import Your First Recipe

1. Pick **Recipe 01 – Email Attachments → Drive** from this repo.  
2. Download `standard.json` from:

   `recipes/001-gmail-attachments/standard.json`

3. In n8n:

   - Go to **Workflows → Import from file**.  
   - Select the JSON.  
   - Open the workflow and update the credentials (e.g. Gmail, Google Drive).  
   - Click **Execute** to test, then **Activate**.

You now have a working n8n setup and your first automation running.  
More recipes: https://workflowrecipes.co
