# Kalimāt — Vocabulaire Coranique 📖

300 mots les plus fréquents du Coran · 5 modes d'étude · PWA hors-ligne

## Déployer sur GitHub Pages (5 minutes)

### 1. Crée un repo GitHub

- Va sur [github.com/new](https://github.com/new)
- Nom du repo : `kalimat` (ou ce que tu veux)
- Laisse en **Public**
- Clique **Create repository**

### 2. Upload les fichiers

- Sur la page du repo, clique **"uploading an existing file"**
- Glisse les 5 fichiers :
  - `index.html`
  - `manifest.json`
  - `sw.js`
  - `icon-192.png`
  - `icon-512.png`
- Clique **Commit changes**

### 3. Active GitHub Pages

- Va dans **Settings** → **Pages** (menu de gauche)
- Source : **Deploy from a branch**
- Branch : `main` / `/ (root)`
- Clique **Save**
- Attends 1–2 minutes

### 4. Ton app est en ligne !

L'URL sera : `https://TON-PSEUDO.github.io/kalimat/`

---

## Installer sur iPhone (PWA)

1. Ouvre le lien dans **Safari** (obligatoire, pas Chrome)
2. Appuie sur le bouton **Partager** (↑)
3. Choisis **"Sur l'écran d'accueil"**
4. L'app apparaît comme une vraie app avec son icône ✓

Elle fonctionne **même hors-ligne** grâce au service worker.

---

## Utiliser sur PC / Mac

### Option A — Dans le navigateur (aucune installation)

Ouvre simplement l'URL dans n'importe quel navigateur moderne (Chrome, Firefox, Safari, Edge). L'app s'adapte automatiquement aux grands écrans avec une barre latérale de navigation.

### Option B — Installer comme application de bureau (PWA)

L'app peut être installée localement sur PC/Mac pour une expérience native (sans barre d'adresse, icône dans le dock/barre des tâches, fonctionne hors-ligne).

**Chrome / Edge (recommandé) :**
1. Ouvre l'URL de l'app
2. Dans la barre d'adresse, clique sur l'icône **Installer** (⊕ ou écran avec flèche)  
   — ou via le menu ⋮ → **"Installer Kalimāt…"**
3. Clique **Installer**
4. L'app s'ouvre dans sa propre fenêtre et apparaît dans tes applications

**Safari sur Mac :**
1. Ouvre l'URL dans Safari
2. Menu **Fichier** → **Ajouter à la station d'accueil** (ou "Add to Dock")
3. Confirme — l'icône apparaît dans le Dock

### Option C — Serveur local (pour développer / tester sans internet)

```bash
# Python 3
python3 -m http.server 8000
# puis ouvre http://localhost:8000
```

```bash
# Node.js (npx)
npx serve .
# puis ouvre l'URL affichée
```

> ⚠️ Le service worker ne s'active pas sur `file://`. Utilise toujours un serveur local ou l'URL GitHub Pages.

---

## Fonctionnalités

| Mode | Description |
|------|-------------|
| 📇 Cartes | Flashcards avec flip, tri acquis/à revoir, étoiles |
| 🧠 Apprendre | Adaptatif : QCM → Vrai/Faux → Écrit, les ratés reviennent |
| 📝 Test | Examen complet : QCM + V/F + Écrit, score final |
| 🔗 Associer | Jeu chrono : matcher arabe ↔ français |
| ✍️ Écrire | Taper la réponse, jusqu'à 3 tours sur les ratés |

- **300 mots** en 30 lots thématiques
- Direction réversible : عربي → FR ou FR → عربي
- Layout adaptatif : mobile (iPhone/Android) et bureau (PC/Mac)
- Fonctionne hors-ligne (service worker PWA)
- Tashkeel complet sur l'arabe
- Progression sauvegardée (localStorage)
