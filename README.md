# Vooroo — Espace client (handoff design)

Maquettes de conception de l'espace client Vooroo, publiées pour le handoff développement.

**En ligne :** https://meljoestein.github.io/vooroo-espace-client/

Version du **8 août 2026** — 14 modules montés dans une coquille CRM commune.

## Contenu

| Chemin | Rôle |
|---|---|
| `index.html` | Portail de handoff : liens vers l'application et vers chaque écran |
| `espace-client/CRM Vooroo.dc.html` | Coquille de l'application (sidebar + header + montage des modules) |
| `espace-client/*.dc.html` | Les 20 composants d'écran |
| `espace-client/support.js` | Runtime `dc` : parsing des composants, chargement à la demande, rendu React |
| `espace-client/_ds/` | Design system Vooroo — tokens (couleurs, typographie, espacements, effets), styles et bundle JS |
| `espace-client/uploads/` | Illustrations et icônes référencées par les écrans |
| `.nojekyll` | Requis : sans ce fichier GitHub Pages ignorerait `_ds/` (dossier préfixé par `_`) |

## Modules

**Métier** — Affaires · Prospects · Contacts · Produits · Activités · Projets · Devis & Factures

**Collaboration & pilotage** — Statistiques · Messagerie · Planificateur · Équipe · Documents

**Paramètres & aide** — Paramètres · Entreprise · Devis & Factures · Champs de données · Guide d'utilisation

## Fonctionnement

Chaque fichier `.dc.html` est à la fois une page autonome et un composant importable. La coquille CRM déclare ses modules via `<dc-import name="…">` ; `support.js` récupère alors le fichier correspondant par requête réseau et le monte dans la page.

Deux conséquences pratiques :

- **Il faut servir les fichiers par HTTP.** Ouvrir un `.dc.html` directement depuis le disque (`file://`) échoue : les requêtes de chargement des composants sont bloquées. En local : `python3 -m http.server` à la racine, puis http://localhost:8000/.
- **Une connexion internet est nécessaire.** React 18 et ReactDOM viennent d'unpkg, les polices de Google Fonts.

## Portée

Maquettes de conception : les données affichées sont fictives, il n'y a ni backend ni persistance. Les interactions se limitent à la navigation et aux états d'interface.
