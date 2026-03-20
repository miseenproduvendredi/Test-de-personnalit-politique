# Test de personnalité politique

Un outil citoyen pour explorer les programmes politiques par soi-même, sans influence.

Ce dépôt regroupe les éditions du test pour chaque élection présidentielle française.

---

## Éditions disponibles

| Édition | Statut | Candidats | Questions |
|---------|--------|-----------|-----------|
| [2027](./2027/) | 🚧 Simulation — en préparation | 8 pressentis | 62 |
| [2022](./2022/) | ✅ Disponible | 12 | 62 |
| [2017](./2017/) | ✅ Disponible | 11 | 62 |

---

## Ce que c'est

Ce test compare les opinions de l'utilisateur aux positions des candidats à l'élection présidentielle française, sur des questions couvrant 13 thèmes : économie, immigration, sécurité, Europe, écologie, santé & social, société, démocratie, valeurs, international, éducation, agriculture et numérique.

Il produit :
- Un **score de compatibilité** (0–100 %) avec chacun des candidats
- Une **boussole politique** en deux dimensions (économique / sociétal)
- Des **éliminations par ligne rouge** (mode Filtre Décisif) avec détection de paradoxes

**Ce test ne dit pas pour qui voter. Il aide à comprendre les programmes.**

---

## Philosophie

- ✅ **Indépendant** — aucune affiliation politique, aucun financement partisan
- ✅ **Anonyme** — aucune donnée personnelle collectée ni transmise
- ✅ **Transparent** — algorithme documenté, biais reconnus, code source ouvert
- ✅ **Neutre** — chaque argument présenté positivement, sans jugement

---

## Structure du dépôt

```
test-personnalite-politique/
├── README.md                   ← Vous êtes ici
├── LICENSE                     ← AGPL-3.0
├── LICENSE_SUPPLEMENT.txt      ← Restrictions : usage commercial, neutralité politique
├── CONTRIBUTING.md             ← Guide de contribution (toutes éditions)
├── CODE_OF_CONDUCT.md          ← Valeurs du projet
├── DOCUMENTATION.md            ← Algorithme, biais, protocole éditorial
│
├── index.html                  ← Page d'accueil (liste toutes les éditions)
│
├── 2022/
│   ├── README.md               ← Présentation de l'édition 2022
│   └── index.html              ← Application autonome (12 candidats, 62 questions)
│
├── 2017/
│   ├── README.md               ← Présentation de l'édition 2017
│   └── index.html              ← Application autonome (11 candidats, 62 questions)
│
└── 2027/
    ├── README.md               ← Présentation de l'édition 2027 (simulation)
    └── index.html              ← Application autonome — positions provisoires
```

Chaque édition est **une application HTML/CSS/JS autonome** : aucune dépendance, aucun serveur, aucune installation. On ouvre `index.html` directement dans un navigateur.

---

## Contribuer

Lisez [`CONTRIBUTING.md`](CONTRIBUTING.md) avant de soumettre une PR.

| Type | Statut |
|------|--------|
| Corrections factuelles sourcées | ✅ |
| Amélioration de la neutralité éditoriale | ✅ |
| Bugs, accessibilité, performance | ✅ |
| Encodage d'une édition historique (avec sources) | ✅ sous conditions |
| Modifications favorisant un parti/candidat | ❌ rejet automatique |
| Ajout de tracking, analytics ou publicité | ❌ rejet automatique |

---

## Licence

**GNU Affero General Public License v3.0 (AGPL-3.0)** + [`LICENSE_SUPPLEMENT`](LICENSE_SUPPLEMENT)

L'AGPL-3.0 garantit la liberté d'utiliser, modifier et distribuer le projet, avec **obligation de publier le code source** de toute version modifiée déployée en ligne. Le supplément ajoute l'interdiction d'usage commercial et la clause de neutralité politique.

---

## Données personnelles

Ce projet ne collecte **aucune donnée personnelle** : pas de serveur, pas de cookies, pas de localStorage, pas d'analytics. Les réponses de l'utilisateur existent uniquement en mémoire vive et disparaissent à la fermeture de l'onglet.

---

*Projet citoyen indépendant — Liberté, Égalité, Fraternité*
