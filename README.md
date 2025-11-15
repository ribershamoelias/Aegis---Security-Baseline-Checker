<p align="center">
  <img src="AEGIS.png" alt="Aegis Logo by Riber Shamo Elias" width="200"/>
</p>

# 🛡️ Aegis – Security Baseline Checker

**Ein modulares Open-Source-Tool zur automatisierten Analyse sicherheitskritischer System-Baselines.**

---

## 📌 Überblick

Aegis ist ein **leichtgewichtiges, modulares Cyber-Security-Werkzeug** zur automatisierten Überprüfung grundlegender System-Sicherheitskonfigurationen (**„Security Baselines“**) auf Linux-Systemen. Es unterstützt **Administrator:innen, Security Engineers, Auditor:innen und DevOps-Teams** bei der schnellen Identifikation sicherheitsrelevanter Fehlkonfigurationen.

Das Projekt wurde mit besonderem Fokus auf **Transparenz, Erweiterbarkeit und Praxisnähe** entwickelt und orientiert sich an realen Anforderungen aus:

* **Cyber Security** (Blue Team / Red Team)
* **IT Audit & Risk Advisory** (z. B. Big Four)
* **Cloud Security Hardening**
* **Systemadministration**
* **Compliance** (ISO 27001, CIS Benchmarks, BSI-Grundschutz)

> Aegis ist ideal für Lernzwecke, Security-Labs und professionelle Umgebungen, in denen grundlegende Sicherheitsanalysen automatisiert werden sollen.

---

## 🎯 Funktionsumfang

Aegis führt eine Reihe wesentlicher Security-Checks durch, die in separate, erweiterbare Module unterteilt sind:

### 🔹 1. Netzwerk & Ports
* Scan offener TCP/UDP-Ports.
* Erkennung unsicherer Dienste (FTP, Telnet, SQL ohne Authentifizierung etc.).
* Identifikation potenzieller Angriffsflächen.

### 🔹 2. Firewall-Analyse
* Support für **UFW, iptables**.
* Überprüfung aktiver/inaktiver Firewall-Policies.
* Hinweis auf übermäßig breite Regeln.

### 🔹 3. SSH-Konfiguration
* Analyse der Konfigurationsdatei `/etc/ssh/sshd_config`.
* Prüfung auf **PermitRootLogin**, Passwortauthentifizierung, veraltete Kryptografie und unsichere Key-Exchange-Methoden.

### 🔹 4. System- & Patch-Status
* Prüfung ausstehender Updates.
* Identifikation sicherheitsrelevanter Patches.
* Warnung bei veralteten Kernelversionen.

### 🔹 5. Benutzer & Passwort-Policies
* Analyse von `/etc/passwd` & `/etc/shadow`.
* Erkennung veralteter Hashverfahren, leerer oder gesperrter Passwörter sowie mangelhafter Gültigkeitsdauer & Ablaufregeln.

### 🔹 6. Logging & Monitoring
* Erkennung fehlender Syslog-/Journaldienste.
* Warnung vor unzureichender Log-Rotation.
* Prüfung grundlegender Audit-Informationen.

### 🔹 7. Automatisierte Reportgenerierung
* **Ausgabeformate:** **Markdown** (menschlich lesbar) und **JSON** (maschinenlesbar).
* Beide enthalten **Risikoeinstufungen**, technische Analysen und konkrete **Handlungsempfehlungen**.

---

## 🚀 Installation

### Voraussetzungen
* **Python 3.10+**
* **Linux** (Ubuntu/Debian empfohlen)
* **Administrator-/sudo-Rechte** für einige Prüfungen

### Schritte
```bash
git clone [https://github.com/DEINUSERNAME/Aegis.git](https://github.com/DEINUSERNAME/Aegis.git)
cd Aegis
pip install -r requirements.txt
