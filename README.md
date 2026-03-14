# (Dé)coupe et (re)colle

> **Choisir · Ordonner · Exporter**  
> Un outil de repagination PDF 100 % navigateur — aucun serveur, aucune donnée transmise.

![Licence CC BY 4.0](https://img.shields.io/badge/licence-CC%20BY%204.0-e8a838?style=flat-square)
![HTML5](https://img.shields.io/badge/HTML5-standalone-5b8ad4?style=flat-square)
![Zéro dépendance serveur](https://img.shields.io/badge/serveur-aucun-3a7d44?style=flat-square)

---

## 🔒 Vos fichiers ne quittent jamais votre ordinateur

C'est le principe fondamental de cet outil, et il n'y a pas d'exception.

- **Votre PDF n'est pas uploadé** — il est lu directement dans la mémoire de votre navigateur
- **Vos sélections, titres, couleurs et polices** ne sont jamais envoyés nulle part
- **Le PDF exporté** est généré localement et téléchargé directement, sans passer par un serveur
- **GitHub Pages** héberge uniquement le code de l'outil (le fichier `index.html`), pas vos données — GitHub ne voit jamais le contenu de vos fichiers
- **Aucun cookie**, aucun tracking, aucun log de contenu

Quand vous fermez l'onglet, tout disparaît. Rien n'est conservé.

> Cet outil peut donc être utilisé en toute confiance avec des documents sensibles, confidentiels ou soumis à des obligations légales de non-divulgation.

---

## À quoi ça sert

Vous avez un PDF de 50 pages et vous voulez en extraire 12, les réordonner, ajouter des intercalaires et une page de garde — sans installer quoi que ce soit, sans envoyer votre fichier en ligne.

**(Dé)coupe et (re)colle** fait exactement ça, dans le navigateur.

---

## Fonctionnalités

- **Galerie de vignettes** — toutes les pages affichées, titrables en un clic
- **Sélection libre** — cliquez pour cocher/décocher, ou tout sélectionner d'un coup
- **Drag & drop** — réordonnez les pages sélectionnées librement
- **Intercalaires** — insérez des pages de séparation avec titre personnalisé
- **Page de garde** — titre, sous-titre, date, couleurs et police au choix
- **Table des matières** — générée automatiquement, paginée, stylisable
- **Polices flexibles** — 3 polices standard (Helvetica, Times, Courier) ou importez n'importe quelle police `.ttf` / `.otf` depuis votre ordinateur
- **Couleurs libres** — fond, texte et couleur d'accent indépendants pour chaque élément généré
- **Export PDF** — téléchargement direct, traitement 100 % local

---

## Utilisation

### Option 1 — Fichier local

1. Téléchargez [`index.html`](./index.html)
2. Ouvrez-le dans votre navigateur (Chrome, Firefox, Edge, Safari)
3. Déposez votre PDF — c'est tout

### Option 2 — GitHub Pages

Le fichier est accessible directement via GitHub Pages :  
👉 **[https://bfbf-test.github.io/pdf-composer](https://bfbf-test.github.io/pdf-composer)**  
*(activer Pages dans les réglages du dépôt si nécessaire)*

---

## Trouver ses fichiers de police

Pour importer une police de votre système :

| Système | Emplacement |
|---|---|
| **Windows** | `C:\Windows\Fonts\` — clic droit sur une police → Propriétés |
| **macOS** | App *Livre des polices* — fichiers dans `/Library/Fonts/` ou `~/Library/Fonts/` |
| **Linux** | `/usr/share/fonts/` ou `~/.local/share/fonts/` — commande : `fc-list` |

---

## Technologies

Tout le traitement se fait côté client, grâce à trois bibliothèques chargées depuis un CDN :

| Bibliothèque | Rôle |
|---|---|
| [pdf.js](https://mozilla.github.io/pdf.js/) (Mozilla) | Rendu des vignettes |
| [pdf-lib](https://pdf-lib.js.org/) | Assemblage et export du PDF final |
| [Sortable.js](https://sortablejs.github.io/Sortable/) | Drag & drop de la liste de pages |

---

## Licence

**[Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/)**

Vous êtes libre de partager, modifier et utiliser ce projet, y compris à des fins commerciales, à condition de **créditer l'auteur**.

> Auteur : **Bertrand Formet** — [github.com/BFBF-test](https://github.com/BFBF-test)

---

*Fait avec soin, sans serveur.*
