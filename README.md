# 🙏 Sabarimala 2026 Expense Tracker - Setup Guide

A beautiful web application to track group expenses and automatically calculate who owes whom. Data is stored in Google Sheets and accessible to everyone via a shared link.

## ✨ Features

- 👥 Manage participants easily
- 💰 Track expenses with checkboxes for splitting
- 🧮 Automatic settlement calculations
- 📱 Mobile-friendly responsive design
- ☁️ Data stored in Google Sheets (synced for everyone)
- 🆓 Completely free to use

## 🚀 Setup Instructions

### Part 1: Google Sheets Backend Setup (5 minutes)

1. **Create a new Google Sheet**
   - Go to [Google Sheets](https://sheets.google.com)
   - Click "Blank" to create a new spreadsheet
   - Name it "Sabarimala 2026 Expenses"

2. **Open Apps Script Editor**
   - In your Google Sheet, click **Extensions** → **Apps Script**
   - Delete any existing code in the editor

3. **Add the Backend Code**
   - Copy ALL the code from `google-script.gs` file
   - Paste it into the Apps Script editor
   - Click **Save** (💾 icon) and name the project "Expense Tracker API"

4. **Deploy as Web App**
   - Click **Deploy** → **New deployment**
   - Click the gear icon ⚙️ next to "Select type"
   - Choose **Web app**
   - Fill in the settings:
     - **Description**: Expense Tracker API
     - **Execute as**: Me (your email)
     - **Who has access**: **Anyone** (important!)
   - Click **Deploy**
   - **Important**: Copy the **Web App URL** (it looks like: `https://script.google.com/macros/s/XXXX/exec`)
   - Click **Done**

5. **Authorize the Script** (first time only)
   - You may need to click "Authorize access"
   - Choose your Google account
   - Click "Advanced" → "Go to Expense Tracker API (unsafe)"
   - Click "Allow"
   - This is safe - you're authorizing your own script!

### Part 2: Deploy Website to GitHub Pages (3 minutes)

1. **Create a GitHub Account** (if you don't have one)
   - Go to [GitHub.com](https://github.com)
   - Click "Sign up" and create a free account

2. **Create a New Repository**
   - Click the **+** icon in the top right → **New repository**
   - Repository name: `sabarimala-expenses` (or any name you like)
   - Description: "Sabarimala 2026 Expense Tracker"
   - Make it **Public**
   - Check ✅ "Add a README file"
   - Click **Create repository**

3. **Upload the HTML File**
   - In your new repository, click **Add file** → **Upload files**
   - Drag and drop the `index.html` file
   - Click **Commit changes**

4. **Enable GitHub Pages**
   - Go to your repository **Settings** (top menu)
   - Scroll down to **Pages** (left sidebar)
   - Under "Source", select **main** branch
   - Click **Save**
   - Wait 1-2 minutes for deployment

5. **Get Your Website URL**
   - Your site will be live at: `https://YOUR-USERNAME.github.io/sabarimala-expenses/`
   - Copy this URL and share it with your group!

### Part 3: Connect Everything (1 minute)

1. **Open Your Website**
   - Visit your GitHub Pages URL
   - You'll see the expense tracker

2. **Configure the API**
   - Click on the **⚙️ Setup** tab
   - Paste the **Web App URL** you copied from Google Apps Script
   - Click **💾 Save & Connect**
   - Click **🔍 Test Connection**
   - You should see "✅ Connected successfully!"

3. **Start Using!**
   - Go to **👥 Participants** tab and add your group members
   - Go to **💰 Expenses** tab and start adding expenses
   - Go to **🧮 Settlements** tab to see who owes whom

## 📱 How to Use

### Adding Participants
1. Go to **Participants** tab
2. Type a name and click "Add Participant"
3. Participants are saved to Google Sheets immediately

### Adding Expenses
1. Go to **Expenses** tab
2. Fill in:
   - Date (defaults to today)
   - Description (e.g., "Temple offerings")
   - Amount in ₹
   - Who paid
   - Check boxes for who should split this expense
3. Click "Add Expense"

### Viewing Settlements
1. Go to **Settlements** tab
2. See everyone's balance:
   - **Green** = Should receive money
   - **Red** = Should pay money
3. See exact transactions needed to settle all debts

## 🔄 Sharing with Your Group

**Option 1: Share the Website Link**
```
https://YOUR-USERNAME.github.io/sabarimala-expenses/
```
Everyone can add expenses and see real-time updates!

**Option 2: Share via WhatsApp**
- Copy your GitHub Pages URL
- Send to your Sabarimala group
- Everyone uses the same link - all data synced via Google Sheets

## 🛠️ Troubleshooting

### "Connection failed" error
- Make sure you deployed as "Web app" in Apps Script
- Check "Who has access" is set to "Anyone"
- Try redeploying: Deploy → Manage deployments → Edit → Deploy

### Data not syncing
- Check your internet connection
- Refresh the page (F5)
- Make sure everyone is using the same website URL

### Can't see Google Sheet data
- Open your Google Sheet
- Check if there are "Participants" and "Expenses" sheets
- They will be created automatically when you add first participant/expense

## 💡 Tips

- **Mobile Use**: Works great on phones! Save the URL to home screen
- **Offline**: You can view data offline, but need internet to add new items
- **Backup**: Your Google Sheet is the backup - all data is there
- **Privacy**: Only people with the link can access
- **Updates**: To update the app, just upload a new `index.html` to GitHub

## 📊 Example Workflow for Sabarimala Trip

1. **Before Trip**: Add all participants
2. **During Trip**: Anyone can add expenses when they happen
3. **After Trip**: Check Settlements tab to see who owes whom
4. **Settle Up**: Use UPI/cash based on settlement calculations

## 🎉 You're All Set!

Your expense tracker is now live and ready for your Sabarimala 2026 pilgrimage!

### Your Links:
- **Website**: `https://YOUR-USERNAME.github.io/sabarimala-expenses/`
- **Google Sheet**: Your Google Sheet URL (data backup)
- **Apps Script**: Can modify backend logic anytime

---

## 📞 Need Help?

If something isn't working:
1. Check the Setup tab in the app
2. Test the connection
3. Verify Google Apps Script deployment
4. Make sure "Who has access" = "Anyone"

Swamiye Saranam Ayyappa! 🙏
