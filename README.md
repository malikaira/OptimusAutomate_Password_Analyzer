# OptimusAutomate_Password_Analyzer
Password Strength Analyzer — Optimus Automate Cybersecurity Internship Task 1

What it does
- Evaluates password strength based on length, complexity & common patterns
- Detects leet-speak variants of breached passwords (e.g. P@ssw0rd)
- Provides actionable feedback with a concrete suggested improvement
- Shows entropy bits and realistic offline crack time (100B guesses/sec)
- Generates cryptographically shuffled strong passwords

Security concepts implemented
- Shannon entropy calculation
- Offline GPU attack modeling (MD5/SHA-1 threat model)
- XSS-safe DOM manipulation (textContent over innerHTML)
- Leet-speak normalization for dictionary matching

Tech
HTML · CSS · Vanilla JavaScript — no frameworks, no dependencies

Live Demo
https://malikaira.github.io/OptimusAutomate_Password_Analyzer/Password_Analyzer.html
