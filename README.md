# OptimusAutomate_Password_Analyzer
Password Strength Analyzer — Optimus Automate Cybersecurity Internship Task 1
# 🔐 PassGuard — Password Strength Analyzer

> **Optimus Automate Cybersecurity Internship — Task 1**

A browser-based password strength analyzer that gives real-time feedback, detects breached passwords (including leet-speak variants), and generates cryptographically shuffled strong passwords — all in a single HTML file with zero dependencies.

---

## 🚀 Live Demo

🔗 *(paste your GitHub Pages link here after enabling it)*

---

## 📸 Preview

| Dark Mode | Light Mode |
|---|---|
| Real-time strength bar, entropy stats, checklist | Same UI with light theme toggle |

---

## ✨ Features

- **Real-time analysis** — strength bar, entropy bits, and crack time update as you type
- **Leet-speak detection** — catches variants like `P@ssw0rd`, `p4ssword`, `pa$$word` against a breached password list
- **Actionable suggestions** — shows a concrete improved version of your actual password, not just generic advice
- **Realistic crack time** — modeled on offline MD5/SHA-1 attack at 100 billion guesses/sec (single GPU estimate)
- **8-rule checklist** — length, uppercase, lowercase, numbers, symbols, 12+ chars, no sequences, no repeats
- **Strong password generator** — cryptographically shuffled, guaranteed mix of all character classes
- **Dark / Light theme toggle**
- **Mobile responsive** — works on screens from 320px to 1920px
- **Zero dependencies** — single HTML file, no frameworks, no backend

---

## 🧠 Security Concepts Implemented

| Concept | Implementation |
|---|---|
| Shannon Entropy | Pool-size formula: `len × log₂(pool)` across 4 character classes |
| Offline GPU Attack Modeling | 100B guesses/sec (conservative RTX 4090 MD5 rate) |
| Leet-speak Normalization | Character map (`@→a`, `0→o`, `3→e`, `$→s`…) before dictionary lookup |
| Common Password Detection | 150+ entry list including Pakistani city names and common patterns |
| XSS-safe DOM Manipulation | `textContent` + `createElement` — never `innerHTML` for user-derived content |
| Fisher-Yates Shuffle | Used in the password generator for unbiased randomness |

---

## 📂 File Structure

```
passguard/
│
├── Password_Analyzer.html    # Complete app — single self-contained file
└── README.md
```

---

## 🚀 Quick Start

```bash
# Clone the repo
git clone https://github.com/your-username/passguard.git

# Open in browser — no server needed
open Password_Analyzer.html
```

---

## 🎨 Tech Stack

| Layer | Technology |
|---|---|
| Structure | HTML5 |
| Styling | CSS3 (CSS Variables, Flexbox, Grid, animations) |
| Logic | Vanilla JavaScript (ES6+) |
| Fonts | Google Fonts — DM Sans, Space Mono |

---

## 📱 Browser Support

| Browser | Supported |
|---|---|
| Chrome / Edge 90+ | ✅ |
| Firefox 88+ | ✅ |
| Safari 14+ | ✅ |
| Mobile Chrome / Safari | ✅ |

---

## 🛡️ Privacy

- **No data is collected or transmitted.** All analysis runs locally in the browser.
- Passwords never leave your device.
- No external requests except Google Fonts.

---

## 📄 License

Built for educational purposes as part of the **Optimus Automate Cybersecurity Internship** program.  
© 2025 Optimus Automate. All rights reserved.

## 📄 Live Demo
https://malikaira.github.io/OptimusAutomate_Password_Analyzer/Password_Analyzer.html
