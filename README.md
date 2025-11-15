<p align="center">
  <img width="180" alt="AEGIS Logo: A shield with a stylized checkmark or eye, symbolizing security and inspection." src="https://github.com/user-attachments/assets/138e059f-9188-4cc9-a38d-9b8ca60dbf2c" />
</p>

# Aegis – Security Baseline Checker 🛡️

**Ein modulares, hochgradig erweiterbares Open-Source-Tool zur automatisierten Überprüfung sicherheitskritischer System-Baselines auf Linux.**

---

<p align="center">
  <a href="https://github.com/DEINUSERNAME/Aegis/actions"><img src="https://img.shields.io/github/actions/workflow/status/DEINUSERNAME/Aegis/main.yml?branch=main&label=Build%20Status&style=flat-square" alt="Build Status"></a>
  <a href="./LICENSE"><img src="https://img.shields.io/badge/License-MIT-blue.svg?style=flat-square" alt="License: MIT"></a>
  <img src="https://img.shields.io/badge/OS-Linux-informational?style=flat-square" alt="Supported OS: Linux">
</p>

---

## 📌 Überblick: Was Aegis tut

Aegis führt schnelle und praxisnahe **Security-Baseline-Checks** durch und identifiziert kritische Fehlkonfigurationen, die oft übersehen werden. Durch sein **modulares Design** ist es ideal, um Härtungsstandards in jeder Umgebung zu gewährleisten.

| Zielgruppe | Fokus |
| :--- | :--- |
| **Cyber Security** | Schnelle Erkennung von Angriffsflächen (Red/Blue Team) |
| **IT Audit & Compliance** | Nachweis der Einhaltung von Standards (CIS, ISO 27001) |
| **DevOps & SysAdmin** | Automatisierte Überprüfung in CI/CD-Pipelines |

---

## ✨ Key Features

Das modulare System prüft wesentliche Sicherheitsbereiche:

* 🔍 **Netzwerk & Ports:** Scan offener Dienste und potenzieller Angriffsflächen.
* 🔥 **Firewall-Analyse:** Überprüfung von **UFW** und **iptables** Regeln.
* 🔐 **SSH-Konfiguration:** Check auf unsichere Einstellungen (`PermitRootLogin`, veraltete Ciphers).
* 🛠️ **Patch-Status:** Warnung bei ausstehenden und sicherheitsrelevanten Updates.
* 👥 **Benutzerverwaltung:** Analyse von Passwörtern, Hashes und Gültigkeitsdauern.
* 📑 **Reporting:** Ausgabe in **Markdown** (menschlich) und **JSON** (maschinenlesbar).
* 🧩 **Erweiterbarkeit:** Einfache Implementierung eigener Check-Module.

---

