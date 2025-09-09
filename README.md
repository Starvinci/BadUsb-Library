# **BadUSB Library - Comprehensive Payload Collection**

##  **EDUCATIONAL PURPOSE DISCLAIMER**

**WICHTIGER HINWEIS**: Diese Sammlung von BadUSB Payloads ist ausschließlich für **Bildungszwecke** und **autorisierte Red Team Aktivitäten** bestimmt.

Die **BadUSB Library** ist eine umfassende Sammlung von 374 BadUSB Payloads, die nach dem **MITRE ATT&CK Framework** organisiert sind. Diese Bibliothek bietet eine vollständige Palette von BadUSB-Scripts für verschiedene Betriebssysteme und Angriffsszenarien.

## **Hauptmerkmale**

- **374 BadUSB Payloads** aus 3 großen GitHub Repositories
- **Multi-OS Support** - Windows, Linux, macOS, Android, iOS
- **Zwei Bereitschaftsstufen** - Directly Ready & Configuration Needed
- **Getestete Qualität** - Alle Scripts getestet und optimiert
- **Staged Attacks** - Tools werden automatisch heruntergeladen
- **Realistische Wartezeiten** - Optimiert für maximale Erfolgsrate

## **Payload-Verteilung**

### **Nach Betriebssystem:**
- **Windows**: 222 Payloads (59.4%)
- **Unix-like/Linux**: 64 Payloads (17.1%)
- **Unix-like/macOS**: 63 Payloads (16.8%)
- **Android**: 15 Payloads (4.0%)
- **iOS**: 10 Payloads (2.7%)

### **Nach Kategorien:**
- **Prank**: 92 Payloads (24.6%)
- **Destruction**: 51 Payloads (13.6%)
- **Authentication**: 33 Payloads (8.8%)
- **Utilities**: 34 Payloads (9.1%)
- **Command & Control**: 28 Payloads (7.5%)
- **Reconnaissance**: 29 Payloads (7.8%)
- **Data Exfiltration**: 26 Payloads (7.0%)
- **Remote Access**: 25 Payloads (6.7%)
- **Collection**: 15 Payloads (4.0%)
- **Social Engineering**: 13 Payloads (3.5%)
- **Defense Evasion**: 8 Payloads (2.1%)
- **Discovery**: 7 Payloads (1.9%)

### **Nach Bereitschaft:**
- **Directly Ready**: 280 Payloads (74.9%) - Sofort einsatzbereit
- **Configuration Needed**: 94 Payloads (25.1%) - Benötigen Konfiguration

## **Verzeichnisstruktur**

```
BadUsbLibrary/
├── authentication/          # Authentifizierung & Credential Harvesting
│   ├── Win/
│   ├── Unix-like/Linux/
│   ├── Unix-like/macOS/
│   ├── Android/
│   └── iOS/
├── collection/              # Datensammlung & Information Gathering
├── command_control/         # Command & Control & Remote Access
├── data_exfiltration/       # Datenexfiltration & Theft
├── defense_evasion/         # Verteidigungsumgehung & Stealth
├── discovery/               # System Discovery & Enumeration
├── destruction/             # System Destruction & Corruption
├── prank/                   # Pranks & Harmless Fun
├── reconnaissance/          # Reconnaissance & Network Scanning
├── remote_access/           # Remote Access & Backdoors
├── social_engineering/      # Social Engineering & Phishing
└── utilities/               # System Utilities & Tools
```

Jede Kategorie enthält Unterverzeichnisse für:
- `directly_ready/` - Sofort einsatzbereite Payloads
- `configuration_needed/` - Payloads die Konfiguration benötigen

## **Kategorie-Details**

### **Authentication (33 Payloads)**
**Zweck**: Credential Harvesting, Password Stealing, Biometric Bypass

### **Collection (15 Payloads)**
**Zweck**: Datensammlung, Screenshots, System-Informationen

### **Command & Control (28 Payloads)**
**Zweck**: Remote Access, Backdoors, Command Execution

### **Data Exfiltration (26 Payloads)**
**Zweck**: Datenexfiltration, File Theft, Information Leakage

### **Defense Evasion (8 Payloads)**
**Zweck**: Log Cleaning, Process Hiding, Stealth Operations

### **Discovery (7 Payloads)**
**Zweck**: System Discovery, Network Enumeration, Information Gathering

### **Destruction (51 Payloads)**
**Zweck**: System Destruction, File Corruption, Data Wiping

### **Prank (92 Payloads)**
**Zweck**: Harmless Pranks, Fun Scripts, User Annoyance

### **Reconnaissance (29 Payloads)**
**Zweck**: Network Scanning, System Enumeration, Information Gathering

### **Remote Access (25 Payloads)**
**Zweck**: Remote Access, Backdoors, Persistent Access

### ** Social Engineering (13 Payloads)**
**Zweck**: Phishing, Fake Updates, User Manipulation

### ** Utilities (34 Payloads)**
**Zweck**: System Utilities, Performance Tools, Maintenance

##  **Konfiguration**

### **Directly Ready Payloads**
Diese Payloads sind sofort einsatzbereit und benötigen keine Konfiguration:
```bash
# Beispiel: macOS Screenshot Taker
DELAY 2000
GUI SPACE
DELAY 1000
STRING Terminal
ENTER
DELAY 3000
STRING screencapture ~/Desktop/screenshot_$(date +%Y%m%d_%H%M%S).png
ENTER
```

### **Configuration Needed Payloads**
Diese Payloads benötigen Konfiguration vor der Verwendung:

**Telegram Bot Setup**:
1. Erstelle einen Telegram Bot über @BotFather
2. Erhalte den Bot Token
3. Erhalte die Chat ID
4. Ersetze `TELEGRAM_BOT_TOKEN` und `TELEGRAM_CHAT_ID` in den Scripts

**Discord Webhook Setup**:
1. Erstelle einen Discord Webhook
2. Kopiere die Webhook URL
3. Ersetze `WEBHOOK_GOES_HERE` in den Scripts

**Beispiel Konfiguration**:
```bash
# Vor der Verwendung ersetzen:
BOT_TOKEN="TELEGRAM_BOT_TOKEN"  # → "1234567890:ABCdefGHIjklMNOpqrsTUVwxyz"
CHAT_ID="TELEGRAM_CHAT_ID"      # → "123456789"
```

##  **Verwendung**

### **1. Payload auswählen**
```bash
# Beispiel: macOS Screenshot Taker
cat collection/Unix-like/macOS/directly_ready/Screenshot-Taker.txt
```

### **2. Auf Flipper Zero übertragen**
```bash
# Kopiere den Inhalt in die Flipper Zero
# Oder verwende qFlipper für den Transfer
```

### **3. Ausführen**
- Verbinde das Flipper Zero mit dem Zielgerät
- Wähle den Payload aus
- Führe ihn aus

##  **Sicherheitshinweise**

 **WICHTIG**: Diese Payloads sind ausschließlich für:
- **Bildungszwecke**
- **Penetration Testing** (mit schriftlicher Erlaubnis)
- **Sicherheitsforschung**
- **Eigene Systeme**

 **NICHT verwenden für**:
- Illegale Aktivitäten
- Unbefugte Zugriffe
- Schädigung fremder Systeme

##  **Quellen**

Die Payloads stammen aus folgenden GitHub Repositories:

1. **[beigeworm/BadUSB-Files-For-FlipperZero](https://github.com/beigeworm/BadUSB-Files-For-FlipperZero)** - 93 Payloads
2. **[FalsePhilosopher/badusb](https://github.com/FalsePhilosopher/badusb)** - 109 Payloads  
3. **[hak5/usbrubberducky-payloads](https://github.com/hak5/usbrubberducky-payloads)** - 70 Payloads
4. **BadUSB Library** - 102 zusätzliche Payloads

##  **Lizenz**

Siehe [License.md](License.md) für Details.

##  **Contributing**

Beiträge sind willkommen! Hier ist wie du helfen kannst:

### ** Neue Payloads hinzufügen:**
1. **Fork** das Repository
2. **Erstelle** einen Feature Branch: `git checkout -b feature/neuer-payload`
3. **Füge** deinen Payload in die richtige Kategorie ein:
   - Wähle die passende OS-Kategorie (Win, Unix-like/Linux, Unix-like/macOS, Android, iOS)
   - Entscheide zwischen `directly_ready/` oder `configuration_needed/`
   - Verwende das MITRE ATT&CK Framework für die Kategorisierung
4. **Teste** deinen Payload gründlich
5. **Dokumentiere** den Payload mit REM-Kommentaren
6. **Committte** deine Änderungen: `git commit -m "Add new payload: [Name]"`
7. **Erstelle** einen Pull Request

### ** Bestehende Payloads verbessern:**
- **Bug Fixes** - Korrigiere Fehler in bestehenden Payloads
- **Optimierungen** - Verbessere Wartezeiten oder Effizienz
- **Dokumentation** - Erweitere Kommentare und Beschreibungen
- **Kategorisierung** - Korrigiere falsche Einordnungen

### ** Dokumentation verbessern:**
- **README Updates** - Erweitere die Dokumentation
- **Beispiele** - Füge Verwendungsbeispiele hinzu
- **Tutorials** - Erstelle Anleitungen für komplexe Payloads
- **Übersetzungen** - Übersetze in andere Sprachen

### ** Testing & Qualitätssicherung:**
- **Funktionalitätstests** - Teste Payloads auf verschiedenen Systemen
- **Syntax-Überprüfung** - Überprüfe Ducky Script Syntax
- **Duplikat-Erkennung** - Finde und entferne doppelte Payloads
- **Performance-Tests** - Teste Wartezeiten und Zuverlässigkeit

### ** Pull Request Guidelines:**
- **Beschreibung** - Erkläre was geändert wurde und warum
- **Tests** - Zeige dass deine Änderungen funktionieren
- **Dokumentation** - Aktualisiere README wenn nötig
- **Code Style** - Folge dem bestehenden Format
- **Ein Payload pro PR** - Erstelle separate PRs für verschiedene Payloads

### ** Was NICHT beitragen:**
- **Malware** - Keine schädlichen oder destruktiven Payloads
- **Illegale Inhalte** - Keine Payloads für illegale Aktivitäten
- **Ungetestete Payloads** - Alle Payloads müssen getestet sein
- **Schlechte Dokumentation** - Alle Payloads brauchen REM-Kommentare

### ** Ideen für Beiträge:**
- **Neue OS-Unterstützung** - Payloads für andere Betriebssysteme
- **Kreative Ansätze** - Innovative Wege BadUSB zu nutzen
- **Educational Content** - Lernmaterialien und Tutorials
- **Tools & Utilities** - Hilfstools für die Entwicklung
- **Bug Reports** - Melde Probleme die du findest

##  **Support**

Bei Fragen oder Problemen:
- **Issues** - Erstelle ein Issue im Repository für Bugs oder Feature Requests
- **Discussions** - Nutze GitHub Discussions für Fragen und Ideen
- **Maintainer** - Kontaktiere die Maintainer bei wichtigen Fragen

---

**Die BadUSB Library - 374 getestete Payloads für maximale Effizienz und Flexibilität!**

*Letzte Aktualisierung: $(date)*