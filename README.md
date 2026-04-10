# Sankadon-Addon
Advanced Addon System for TwintailLauncher

🧠 Overview

Sankadon est un addon avancé pour le launcher basé sur
TwintailLauncher

Il ajoute :

🎮 Gestion complète de profils de mods
📦 Installation automatique de collections (sans compte Nexus)
🌍 Support multi-langue (FR/EN auto)
🧩 Interface intégrée au launcher (style AAA)
🔄 Auto-update + sync upstream
✨ Features
🧩 Addon System
Intégration via <AddonIcon />
UI complète via panneau dynamique
Aucun impact sur le launcher de base
📦 Mod Profiles System
Création / duplication / suppression
Export / import JSON
Stockage local (AppData/sankadon/profiles/)
📥 Collection Installer (NO NEXUS ACCOUNT)
Compatible :
Nexus Mods
GameBanana
Collections custom (.sankadon)

👉 Fonctionnement :

Ouvre les pages dans le navigateur
L'utilisateur clique "Download"
🔍 Détection automatique dans Downloads
⚙️ Installation automatique

➡️ 100% sans API / sans compte Premium

👁️ Download Watcher
Scan temps réel du dossier Downloads
Ignore fichiers incomplets (.part / .crdownload)
Support :
.zip
.rar
.7z
.pak
🎨 UI Components
ProfileCard (rename inline ✏️)
CollectionInstallPanel (progress live)
ProfilesView (dashboard principal)
🌍 i18n
Détection automatique Windows (FR/EN)
Override utilisateur (localStorage)
⚙️ Config centralisée
sankadon.config.ts
couleurs
liens
langues
📁 Structure
src/
 ├── components/sankadon/
 ├── core/
 │   ├── ProfileManager.ts
 │   ├── CollectionManager.ts
 │   ├── DownloadWatcher.ts
 │   └── CollectionInstaller.ts
 ├── i18n/
 └── types/
⚡ Installation (DEV)
pnpm install
pnpm dev:tauri
🛠️ Setup
Fork :
👉 TwintailTeam / TwintailLauncher
Copier les fichiers Sankadon
Modifier :
SETUP.md → 2 lignes
Ajouter :
<AddonIcon />
🚀 Release automatique
GitHub Actions inclus
build Windows + Linux
création release auto
Déployer :
git tag v1.0.0
git push --tags

➡️ 🎉 Release automatique

🔄 Upstream Sync

Workflow :

vérifie chaque lundi
ouvre une issue si update disponible
📜 Scripts inclus
install.ps1 → Windows
install.sh → Linux
update.ts → sync upstream
🧠 Architecture
Core Systems
ProfileManager → gestion profils
CollectionManager → parsing sources
DownloadWatcher → détection fichiers
CollectionInstaller → orchestration
🎯 Philosophie

👉 Pas de dépendance Nexus API
👉 Pas de compte requis
👉 UX simple + automatisée

⚠️ Limitations
téléchargement manuel requis (click utilisateur)
dépend du navigateur
vitesse variable
🔥 Roadmap
Auto-detection jeux
UI améliorée
Support multi-launchers
Plugins système
💬 Contribution

Pull requests bienvenues 👍
