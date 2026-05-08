<div align="center">







# Edge Password Viewer

**Memory forensics tool for Microsoft Edge**

[![Windows](https://img.shields.io/badge/Windows-10%2F11-0078D4?style=flat-square&logo=windows&logoColor=white)](https://www.microsoft.com/windows)
[![Admin](https://img.shields.io/badge/Requires-Administrator-red?style=flat-square&logo=shield&logoColor=white)]()
[![License](https://img.shields.io/badge/License-MIT-95b806?style=flat-square)]()

</div>

---

## 🔍 How it works

Edge Password Viewer extracts saved credentials directly from the memory of a running `msedge.exe` process — without touching the browser's encrypted database.

It reads RAM via WinAPI `ReadProcessMemory` or parses a `.DMP` memory dump file, then searches for URL / Login / Password patterns stored in plain text in process memory.

---

## ⚡ Features

<table>
<tr>
<td width="50%">

### 🖥 Scan
- Auto-detects `msedge.DMP` in `C:\Temp` and `C:\Windows\Temp`
- File watcher — picks up new dumps automatically
- **Create Dump** — launches Edge, waits for data to load, dumps memory, then kills Edge
- Real-time progress during file scan
- **Remove Dump** — deletes dump file after scanning

</td>
<td width="50%">

### 💾 Export
- Formats: **CSV**, **JSON**, **TXT**
- Save next to executable — one click
- Or choose any location via dialog
- Output filename: `EdgePW.<fmt>`

</td>
</tr>
</table>

---

## 📋 Results format

```
Url: example.com
Login: user@mail.com
Password: hunter2
──────────────────────────
Url: another.com
Login: admin
Password: qwerty123
```

---

## 🚀 Usage

```
1. Run EdgePasswordViewer.exe as Administrator
2. Open the Scan tab
3. Click "Create Dump"  →  Edge launches, dump is created, Edge closes
   — or —
   Browse to an existing msedge.DMP file manually
4. Click "Scan"
5. Export results from the File tab
```

---

## ⚠️ Requirements

| | |
|---|---|
| OS | Windows 10 / 11 |
| Privileges | Administrator |
| Browser | Microsoft Edge (installed) |

---

## ⚠️ Disclaimer

> This tool is intended **only** for use on systems you own or have **explicit authorization** to test.
> Unauthorized use against third-party systems is illegal.

---

<div align="center">

## 👤 Developer

[![GitHub](https://img.shields.io/badge/GitHub-SelfC0de-181717?style=for-the-badge&logo=github)](https://github.com/SelfC0de)
[![Telegram](https://img.shields.io/badge/Telegram-@selfcode__dev-2CA5E0?style=for-the-badge&logo=telegram)](https://t.me/selfcode_dev)
[![VK](https://img.shields.io/badge/VK-selfcode__dev-0077FF?style=for-the-badge&logo=vk)](https://vk.com/selfcode_dev)

</div>
