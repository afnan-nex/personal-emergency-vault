# 🔒 Personal Emergency Vault

A secure, client-side encrypted emergency vault to store your critical contacts, links, and send emergency messages via Discord. Designed to be accessed quickly when needed while keeping your data private.

🌐 **Live Demo**: [**Try Personal Emergency Vault**](https://afnan-nex.github.io/personal-emergency-vault/index.html)

**Default Password**: 1234

---

## ⚠️ CRITICAL SECURITY WARNING ⚠️

**READ THIS CAREFULLY BEFORE DEPLOYING OR USING THIS PROJECT!**

This project **MUST** be hosted on a private domain. **DO NOT** share the name or the URL of this website with anyone. 

Because this is a client-side application, sensitive information such as:
- 🔑 Your Vault Password
- 📇 Contact Information
- 🔗 Saved Links
- 💬 Discord Webhook URLs

**can be easily exposed** if someone gains access to the source code or the live site.

### 🛡️ How to Secure Your Deployment:
1. **Use Private Hosting:** Deploy using services like **Netlify**, Vercel, or Cloudflare Pages instead of a public GitHub Pages repository.
2. **Complex Naming:** Set a highly complex, unguessable project/subdomain name so no one can guess the URL.
3. **Disable Web Indexing:** Ensure web indexing is turned off (add `noindex` meta tags or configure `robots.txt`) so your vault does not show up in search engine results.
4. **Change the Password:** It is **ESSENTIAL** that you change the default password in the code to something highly secure and complex.
5. **Keep it Hidden:** Do not share the URL. Treat it like a hidden emergency tool.

---

## ✨ Features

- 🔐 **Client-Side Encryption:** Your data is encrypted and decrypted directly in your browser.
- 📇 **Emergency Contacts:** Store and manage critical contact information securely.
- 🔗 **Important Links:** Keep essential URLs safe and accessible.
- 💬 **Discord Integration:** Send emergency messages directly via Discord Webhooks (up to 2000 characters).
- 🔄 **Auto-Lock:** Automatically locks the vault and expires the session after a period of inactivity to prevent unauthorized access.
- 📱 **Responsive Design:** Access your vault from any device.

---

## 🚀 Deployment Guide

Since this project handles sensitive data, it is highly recommended to deploy it privately.

### Deploying to Netlify (Recommended)
1. Fork this repository **privately** (do not make it public on GitHub).
2. Go to [Netlify](https://www.netlify.com/) and sign in.
3. Click "Add new site" -> "Import an existing project".
4. Connect your private GitHub repository.
5. **Important:** During setup, ensure you configure a complex site name (e.g., `x7f9-private-vault-2a.netlify.app`).
6. Deploy!

### Disabling Search Engine Indexing
To prevent search engines from crawling your vault, ensure your `index.html` contains the following in the `<head>` section:
```html
<meta name="robots" content="noindex, nofollow">
