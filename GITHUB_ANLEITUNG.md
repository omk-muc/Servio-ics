# Anleitung: Servionics Website auf GitHub hochladen und veröffentlichen

## Schritt 1: GitHub Repository erstellen

1. Gehe zu https://github.com und melde dich an (oder erstelle einen kostenlosen Account)
2. Klicke oben rechts auf das **+** Symbol und wähle **"New repository"**
3. Gib folgende Einstellungen ein:
   - **Repository name:** `servionics-demo` (oder einen anderen Namen deiner Wahl)
   - **Description:** "Servionics Robot-as-a-Service Demo Website"
   - **Public** auswählen (damit GitHub Pages funktioniert)
   - **NICHT** "Add a README file" anklicken (wir haben schon eine)
4. Klicke auf **"Create repository"**

## Schritt 2: Dateien hochladen

Du hast jetzt zwei Möglichkeiten:

### Option A: Via Web-Interface (Einfacher)

1. Auf der leeren Repository-Seite klicke auf **"uploading an existing file"**
2. Ziehe alle drei Dateien in den Upload-Bereich:
   - `index.html`
   - `image_8.png`
   - `README.md`
3. Gebe als Commit message ein: "Initial commit"
4. Klicke auf **"Commit changes"**

### Option B: Via Git Command Line (Fortgeschritten)

Wenn du Git auf deinem Computer installiert hast:

```bash
# In dem Ordner mit den Dateien:
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/DEIN-USERNAME/servionics-demo.git
git push -u origin main
```

(Ersetze `DEIN-USERNAME` mit deinem GitHub Username)

## Schritt 3: GitHub Pages aktivieren

1. Gehe in deinem Repository zu **Settings** (oben rechts)
2. Scrolle in der linken Sidebar nach unten zu **"Pages"**
3. Unter "Build and deployment":
   - **Source:** Wähle "Deploy from a branch"
   - **Branch:** Wähle "main" und "/" (root)
4. Klicke auf **"Save"**
5. Warte 1-2 Minuten

## Schritt 4: Deine Website ist live!

Nach 1-2 Minuten erscheint oben eine grüne Box mit deiner Website-URL:

**https://DEIN-USERNAME.github.io/servionics-demo/**

Diese URL kannst du jetzt teilen!

## Tipps:

- Die Website ist öffentlich zugänglich
- Du kannst jederzeit Änderungen machen, indem du die Dateien im Repository bearbeitest
- Die Website wird automatisch aktualisiert, wenn du Änderungen committest

## Hilfe benötigt?

Falls du Hilfe brauchst, kann ich dir bei jedem Schritt helfen!
