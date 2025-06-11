# 📦 SyncFlow – Inventory Management That Just Works

**SyncFlow** is a portable, dark-themed inventory management system designed for real-world use across multiple devices. Whether you're running it solo or syncing across an entire team, SyncFlow adapts.

---

## 🚀 What’s Included

* 🖥️ **Dark-themed GUI** with dynamic overview panels
* 🔍 **Searchable, tabbed Excel viewer** for each inventory category
* 📊 **Live stock-level pie chart** with real-time status coloring
* 🔐 **Secure OneDrive integration** using Microsoft Authentication
* 📁 **Automatic file discovery** – no hardcoded paths
* 🔁 **Smart lock/unlock logic** for safe file handling
* 📦 **Weekly delta tracking** for usage and stockout awareness

---

## 🔧 Setup Instructions

1. **Ensure OneDrive is installed and signed in.**

   * If using a shared folder, click "Add shortcut to My files" and wait for sync.

2. **Place `MainInventoryList.xlsx` inside a folder named `Hi-Tech Inventory`**.

   * This folder must be inside OneDrive (e.g. `C:/Users/You/OneDrive/Hi-Tech Inventory`)

3. **Run SyncFlow**

   * Download or build the `.exe` using PyInstaller
   * First launch will auto-locate your Excel file

---

## 🛠 For Developers

To build your own `.exe`:

```bash
pip install pyinstaller
pyinstaller --onefile --noconsole --name SyncFlow_DarkGUI_v1.3.3g SyncFlow_AutoFileLocator.py
```

---

## 💡 Features in v1.3.3g

* ✅ Auto-detects inventory file in shared OneDrive folders
* ✅ Corrects file locking and upload timing
* ✅ Works across machines with no reconfiguration
* ✅ Precompiled `.exe` requires no dependencies

---

## 📎 Files Used

* `MainInventoryList.xlsx` – live data file
* `logs/` – auto-generated change logs per week
* `token_cache.json` – OneDrive login cache

---

## 🙌 Credits

Built by [DevReed](https://github.com/DevReed), fueled by spreadsheets, frustration, and caffeine.

---

## 📬 Need Help?

If the GUI doesn’t load or your file isn’t found:

* Ensure OneDrive has synced the folder
* Close Excel before syncing
* Or manually select the file (feature coming soon!)

---

> **SyncFlow** – because inventory shouldn't require IT support every Monday.
