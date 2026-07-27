# Vooroo — Espace client

Pages de handoff design déployées via GitHub Pages.
Version du **26 juillet 2026** (messagerie : 25 juillet 2026).

👉 **Accueil : https://meljoestein.github.io/vooroo-espace-client/**

## Espace client

L'application complète (sidebar + header + les 8 menus montés directement dedans) :

- **[CRM — application complète](https://meljoestein.github.io/vooroo-espace-client/espace-client/crm.dc.html)**

Les mêmes pages en accès direct :

| Page | Lien |
|---|---|
| Contacts | [contacts.dc.html](https://meljoestein.github.io/vooroo-espace-client/espace-client/contacts.dc.html) |
| Prospects | [prospects.dc.html](https://meljoestein.github.io/vooroo-espace-client/espace-client/prospects.dc.html) |
| Affaires | [affaires.dc.html](https://meljoestein.github.io/vooroo-espace-client/espace-client/affaires.dc.html) |
| Projets | [projets.dc.html](https://meljoestein.github.io/vooroo-espace-client/espace-client/projets.dc.html) |
| Produits | [produits.dc.html](https://meljoestein.github.io/vooroo-espace-client/espace-client/produits.dc.html) |
| Activités | [activites.dc.html](https://meljoestein.github.io/vooroo-espace-client/espace-client/activites.dc.html) |
| Devis & Factures | [devis-factures.dc.html](https://meljoestein.github.io/vooroo-espace-client/espace-client/devis-factures.dc.html) |
| Équipe | [equipe.dc.html](https://meljoestein.github.io/vooroo-espace-client/espace-client/equipe.dc.html) |

## Messagerie de vente

- [Messagerie de vente](https://meljoestein.github.io/vooroo-espace-client/messagerie/messagerie-de-vente.dc.html)

## Paramètres — Devis & Factures

- [Paramètres Devis & Factures](https://meljoestein.github.io/vooroo-espace-client/parametres-facturation/parametres-devis-factures.dc.html)

---

## Notes techniques

- Les pages sont les exports bruts de l'outil de design (format `.dc.html`) : elles sont servies
  telles quelles, le runtime `support.js` les rend côté navigateur.
- Chaque dossier embarque **son propre `support.js`** (les versions diffèrent entre les livraisons)
  et **uniquement les images réellement utilisées** par les pages.
- Le CRM monte les autres pages en DOM direct via `<dc-import>`, qui va chercher le fichier frère
  `<nom>.dc.html`. Les fichiers ont donc été renommés en ASCII (`Activités Vooroo.dc.html` →
  `activites.dc.html`) et les `dc-import` du CRM mis à jour en conséquence, pour éviter les URLs
  encodées.
- Deux ajustements par rapport à l'export d'origine : le renommage ci-dessus, et l'ajout du libellé
  `equipe: 'Équipe'` manquant dans `MENU_LABELS` du CRM (le header affichait `equipe` en minuscules).
