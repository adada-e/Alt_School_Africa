# 🌐 AI Bulk Reconciliation — Node.js Deployment

This project demonstrates the deployment of a Node.js web app with a branded landing page using Nginx on a DigitalOcean cloud instance.

---

## ✅ Steps Taken

### 1. Provisioned a Linux server (Ubuntu 22.04) on DigitalOcean
- 1 vCPU, 512MB RAM, 10GB SSD
- Logged in via SSH using `root` and created a new user `adadauser`

### 2. Installed Node.js and Express
```bash
sudo apt update
sudo apt install nodejs npm -y

----

mkdir ~/myapp && cd ~/myapp
npm init -y
npm install express


-----

const express = require('express');
const app = express();
const port = 3000;

app.use(express.static('public'));

app.listen(port, () => {
  console.log(`Server is running on http://localhost:${port}`);
});


----

Added the custom landing page

----

Ran the app
node server.js

----
Configured Nginx as reverse proxy (optional)
To make it accessible via port 80 and show your domain or IP cleanly.

----
Hosted public IP

http://134.122.87.230:3000


----


---

## ✅ 3. **Take and Add the Screenshot**

1. Open your landing page in a browser
2. Take a screenshot (`Win + Shift + S` on Windows)
3. Save it as `screenshot.png` in your project folder
4. Stage and push it:
   ```bash
   git add screenshot.png README.md
   git commit -m "Added screenshot and documentation"
   git push

