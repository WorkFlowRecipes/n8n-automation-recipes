# 000 – n8n Master Setup (15 Minutes)

This quick-start guide gets you from **zero → ready to import recipes** in about 15 minutes.

You have two options:
- **Option A (easiest):** n8n Cloud - hosted, managed, $20/month after trial
- **Option B (cheapest):** Self-hosted - your own server, ~$6/month

---

## ✅ Option A – n8n Cloud (Recommended for Beginners)

**Best for:** People who want to start immediately without server setup.

**Cost:** Free trial, then $20/month

### Setup Steps:

1. **Create account:**
   - Go to [https://n8n.io](https://n8n.io)
   - Click **Start for free**
   - Sign up with email or Google

2. **Verify it works:**
   - Once inside, click **Workflows** → **New**
   - You should see a blank canvas
   - Close it (you don't need to build anything yet)

3. **You're ready!** 
   - You can now import any recipe from this repo
   - Skip to "Next Step" section below

**When to upgrade:** The free trial gives you 2,500 workflow executions. Once you hit the limit, you'll need to upgrade to the Starter plan ($20/month).

---

## ✅ Option B – Self-Hosted (Budget-Friendly)

**Best for:** People comfortable with basic server management who want to save money long-term.

**Cost:** ~$6-12/month (VPS hosting only)

### What You'll Need:

- A domain name (or subdomain like `n8n.yourdomain.com`)
- A VPS (Virtual Private Server) - DigitalOcean, Linode, Vultr, etc.
- 30-45 minutes for initial setup (not 15 - this is more involved)

### High-Level Steps:

1. **Provision a server:**
   - Create a VPS with at least 1GB RAM (DigitalOcean $6/month droplet works)
   - Choose Ubuntu 24.04 LTS as the OS
   - Point a subdomain (e.g., `n8n.yourdomain.com`) to your server's IP address

2. **Install n8n with Docker:**
   - SSH into your server
   - Install Docker and Docker Compose
   - Run the official `n8nio/n8n` image with persistent storage
   - Configure environment variables (webhook URL, timezone, etc.)

3. **Secure with HTTPS:**
   - Install Nginx as reverse proxy
   - Use Certbot to get a free SSL certificate from Let's Encrypt
   - Configure Nginx to forward traffic to n8n

4. **Test access:**
   - Open `https://n8n.yourdomain.com` in your browser
   - Create your admin account
   - Verify you can create a new workflow

### 🎥 Detailed Video Walkthrough

If you're going the self-hosted route, **watch this first** (before you start):

**[n8n Self-Hosted Setup on DigitalOcean](https://www.youtube.com/watch?v=hO_KWrosh7M)** (Third-party tutorial)

> ⚠️ **Note:** This is an external video not created by Workflow Recipes. The steps may vary slightly based on your VPS provider, but the core concepts remain the same.

### Alternative: Quick Self-Host Script

If you want a faster self-hosted setup, the n8n community has created one-click install scripts. Check the official docs:

**[n8n Self-Hosting Guide](https://docs.n8n.io/hosting/)**

---

## 🔧 First-Time Configuration (Both Options)

Once you're logged into n8n (cloud or self-hosted), do this quick configuration:

### 1. Set Your Timezone
- Click your profile icon (top right)
- Go to **Settings** → **Personal**
- Set your timezone (important for scheduled workflows)

### 2. Test Credentials
We'll add actual credentials when you import Recipe #1, but verify the system works:

- Click **Credentials** in the left sidebar
- Click **Add Credential**
- Search for "Gmail" 
- You should see the credential form
- **Don't configure it yet** - just verify you can access this menu
- Click Cancel

### 3. Enable Webhooks (Self-Hosted Only)

If you're self-hosted, verify your webhook URL is set correctly:

- Settings → **Environments** → Check that "Webhook URL" shows your domain
- It should be: `https://n8n.yourdomain.com/`

---

## 🎯 Next Step – Import Your First Recipe

Now that n8n is running, let's get your first automation working:

### 1. Pick Recipe #1

Go to: **[Recipe 001 - Email Attachments → Drive](../001-email-attachments-to-drive/)**

> ⚠️ **Note:** As of today, Recipe #1 is still being built and tested. Check back in 1 week (or subscribe at [workflowrecipes.co](https://workflowrecipes.co) to get notified when it's published).

### 2. Download the JSON

Once Recipe #1 is published:
- Download `workflow.json` from the recipe folder
- Save it to your computer

### 3. Import to n8n

In your n8n instance:
1. Click **Workflows** in the left sidebar
2. Click **Add Workflow** → **Import from File**
3. Select the downloaded `workflow.json`
4. The workflow will open in the editor

### 4. Configure Credentials

The workflow will have red warning icons on nodes that need credentials:

1. Click on a node with the warning
2. Click **Create New Credential**
3. Follow the authentication flow (usually OAuth for Gmail/Drive)
4. Repeat for each node that needs credentials

### 5. Test It

1. Click **Execute Workflow** (play button at bottom)
2. Check if it runs without errors
3. Verify the results (check your Google Drive for test files)

### 6. Activate It

1. Toggle the **Active** switch at the top right
2. The workflow now runs automatically based on its trigger

---

## 🆘 Troubleshooting

### n8n Cloud Issues

**Problem:** "Workflow execution limit reached"  
**Solution:** Upgrade to Starter plan ($20/month) or wait until next month for limit reset

**Problem:** "Credentials not working"  
**Solution:** Make sure you've authorized the OAuth connection and granted all requested permissions

### Self-Hosted Issues

**Problem:** "Can't access n8n at my domain"  
**Solution:** 
- Check DNS propagation (can take 1-24 hours)
- Verify Nginx is running: `sudo systemctl status nginx`
- Check SSL certificate: `sudo certbot certificates`

**Problem:** "Webhooks not triggering"  
**Solution:** Verify webhook URL in Settings → Environments matches your domain exactly

**Problem:** "Workflows not saving"  
**Solution:** Check Docker volume is mounted correctly - data should persist in `/root/.n8n/`

---

## 📚 Additional Resources

- **Official n8n Docs:** [https://docs.n8n.io](https://docs.n8n.io)
- **n8n Community Forum:** [https://community.n8n.io](https://community.n8n.io)
- **Workflow Recipes Newsletter:** [https://workflowrecipes.co](https://workflowrecipes.co)

---

## ✅ You're Ready!

If you can:
- ✅ Log into your n8n instance
- ✅ Create a new workflow
- ✅ See the credentials menu

**You're all set!** Head back to the [main README](../../README.md) to browse available recipes.

---

**Next up:** [Recipe 001 - Email Attachments → Auto-Filed in Google Drive](../001-email-attachments-to-drive/) *(coming soon)*
