# 🌐 Website Uploader

Website Uploader is a simple and secure tool for uploading website files (HTML, CSS, JavaScript, images, etc.) directly to **GitHub**, which serves as the database.  
The uploaded files can then be deployed seamlessly to **GitHub Pages** or other hosting platforms like **Vercel**.

🔗 **Example Website**: [madz-uploader.vercel.app](https://madz-uploader.vercel.app)

---

## ✨ Features
- 📂 Upload website files via browser or CLI
- 🔑 GitHub repository used as a **database**
- 🔒 File **encryption** before storing
- ⚡ Real-time synchronization with GitHub
- 🚀 One-click deployment to **GitHub Pages**

---

## 📂 File Input & Process
1. User selects files from local storage (HTML, CSS, JS, images, etc.).
2. Files are **encrypted** for security.
3. Encrypted files are uploaded to GitHub repository using **GitHub API**.
4. GitHub stores the files, acting as the backend database.
5. Files can then be deployed as a static website.

---


##📦 Prerequisites

Before using this project, make sure you have:

· Node.js v18 or higher
· Git installed
· GitHub account with Personal Access Token with repo permissions

---

##🚀 Installation & Setup

1. Clone Repository

```bash
git clone https://github.com/Madzz14Stt/madzoffc-webuploader.git
cd webuploader
```

2. Install Dependencies

```bash
npm install
```

3. Configure Environment Variables

Create a .env file in the root directory and add the following configuration:

```env
GITHUB_TOKEN=your_github_personal_access_token_here
GITHUB_OWNER=your_github_username
GITHUB_REPO=your_repository_name
ENCRYPTION_KEY=your_32_character_encryption_key_here
PORT=3000
```

4. Run the Web

Test Mode:

```bash
npm test
```

Production Mode:

```bash
npm start
```

The Website will run at http://localhost:3000

---

##🗂️ Project Structure

```
website-uploader/
├── public/                 # Static files
│   ├── css/               # Stylesheets
│   ├── js/                # Client-side JavaScript
│   └── index.html         # Main page
├── routes/                # Route handlers
│   └── upload.js          # API upload handler
├── utils/                 # Utilities
│   ├── github.js          # GitHub API helper
│   └── encryption.js      # Encryption utilities
├── .env                   # Environment variables
├── .gitignore            # Git ignore rules
├── index.js                # Main Website
├── package.json          # Dependencies and scripts
└── README.md             # This documentation
```

---

###📝 License

This project is licensed under the MIT License - see the LICENSE file for details.

---