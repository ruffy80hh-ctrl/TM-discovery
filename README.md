# TiviMate Panel - Discovery Service

**Unveränderliche API-Discovery für maximale Ausfallsicherheit**

## 🎯 Was ist das?

Dieses Repository hostet eine Discovery-Datei, die Apps sagt, wo sich die aktuelle API befindet.

**Vorteil:** Bei Hosting-Wechsel musst du nur diese Datei ändern - alle Apps funktionieren weiter!

## 📡 Discovery URL

```
https://DEIN-USERNAME.github.io/tivimate-discovery/api.json
```

Diese URL bleibt **für immer gleich**, auch wenn deine API umzieht!

## 🔄 Wie es funktioniert

```
1. App fragt GitHub: "Wo ist die API?"
2. GitHub antwortet: "Bei worker3.ruffy80hh.workers.dev"
3. App verbindet zur aktuellen API
4. ✅ Bei Umzug: Nur GitHub-Datei ändern!
```

## 📋 api.json Struktur

```json
{
  "version": "1.0.0",
  "api_url": "https://worker3.ruffy80hh.workers.dev/api",
  "backup_urls": [
    "https://backup-server.com/api/"
  ],
  "status": "online"
}
```

## 🔧 Bei Hosting-Wechsel

**Alte API:** `https://old-server.com/api`
**Neue API:** `https://new-server.com/api`

**Update:**
1. Bearbeite `api.json`
2. Ändere `api_url` zu neuer URL
3. Commit & Push
4. ✅ Fertig! Alle Apps nutzen neue URL

## 📊 Status

- **API Status:** Online ✅
- **Letzte Änderung:** 2025-10-17
- **Aktive API:** worker3.ruffy80hh.workers.dev

## 🆘 Support

Bei Problemen: support@example.com

---

**🔒 Diese Repository ist Public - enthält keine sensiblen Daten!**
