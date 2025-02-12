# Terminal-basierter Chat-Raum

Ein einfacher, terminalbasierter Chat-Raum, der lokal läuft und es mehreren Clients ermöglicht, sich mit einem Server zu verbinden und Nachrichten in Echtzeit auszutauschen.

![image](https://github.com/user-attachments/assets/c49840cf-0789-400c-a26c-4954bd7ff648)

## Features
- Server-Client-Architektur
- Mehrere Clients können sich mit dem Server verbinden
- Nachrichten werden an alle verbundenen Clients gesendet (Broadcast)
- Der Server kann ebenfalls Nachrichten senden

## Voraussetzungen
- **Betriebssystem:** Linux/macOS/Windows (mit WSL)
- **Compiler:** g++ oder clang++
- **Bibliotheken:** pthread, socket (standardmäßig auf Unix-Systemen vorhanden)

## Installation & Nutzung

### 1️⃣ Code kompilieren
```bash
# Server kompilieren
g++ -o server server.cpp -pthread

# Client kompilieren
g++ -o client client.cpp -pthread
```

### 2️⃣ Server starten
```bash
./server
```

### 3️⃣ Clients verbinden
Jeder Client startet das Programm und verbindet sich mit dem Server:
```bash
./client
```

### 4️⃣ Chatten!
- Clients können Nachrichten in die Konsole eingeben und absenden.
- Der Server kann ebenfalls Nachrichten an alle Clients senden.

## Struktur
```
/chat_project
├── server.cpp  # Server-Code
├── client.cpp  # Client-Code
├── README.md   # Diese Datei
```

## To-Do / Verbesserungen
- [ ] Benutzername-Unterstützung
- [ ] Private Nachrichten zwischen Clients
- [ ] Verbesserte Fehlerbehandlung

## Lizenz
none
