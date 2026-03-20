# Guide de contribution

> Projet : Test de personnalité politique
> Licence : AGPL-3.0 + LICENSE_SUPPLEMENT.txt

Merci de l'intérêt que vous portez à ce projet. Lisez ce document avant de soumettre une contribution.

---

## Philosophie

Ce projet a une mission unique : **aider les citoyens à comprendre les programmes politiques par eux-mêmes, sans influence**.

Il n'est ni un outil de communication politique, ni un produit commercial. Il est un outil de démocratie.

---

## Types de contributions

### ✅ Contributions bienvenues

**Sur les données (questions et positions)**
- Correction d'une erreur factuelle dans une position de candidat (avec source vérifiable)
- Correction d'un chiffre obsolète ou d'un lien mort dans un contexte factuel
- Amélioration de la neutralité éditoriale (reformulation plus équilibrée, moins connotée)
- Ajout d'une nouvelle question respectant le protocole éditorial (voir §Protocole)

**Sur le code**
- Correction de bugs
- Amélioration de l'accessibilité (WCAG)
- Performance et compatibilité navigateur
- Améliorations de l'interface utilisateur sans modification des données ni de l'algorithme

**Sur la documentation**
- Clarification de l'algorithme ou des choix de conception
- Corrections typographiques ou de formulation

**Nouvelles éditions**
- Adaptation du projet à une nouvelle élection présidentielle française (2027, etc.)
- Adaptation à d'autres pays ou niveaux d'élection, sous réserve du respect strict du protocole éditorial et de la licence

### Format attendu pour une PR

Toute pull request doit inclure :

1. **Une description claire** de ce qui est modifié et pourquoi.
2. **Des sources** pour toute modification factuelle.
3. **La justification de neutralité** : en quoi la modification ne favorise ni ne défavorise aucun camp.
4. **L'édition concernée** (2022, 2027, etc.) clairement indiquée.

---

## Ce que nous refusons systématiquement

### ❌ Motifs de rejet automatique

1. **Toute modification tendant à favoriser ou défavoriser un parti, un candidat ou une idéologie**, quelle que soit la subtilité de la formulation.

2. **Toute modification de l'algorithme de compatibilité** visant à amplifier ou réduire les scores d'un candidat particulier sans justification mathématique indépendante.

3. **L'ajout de mécanismes de collecte de données** : tracking, analytics, cookies, `localStorage`, `sessionStorage`, transmission des réponses vers un serveur tiers, fingerprinting.

4. **L'insertion de contenu publicitaire, de liens sponsorisés ou de tout élément commercial**.

5. **Le remplacement de sources institutionnelles neutres** par des sources partisanes ou des médias d'opinion.

6. **Toute modification des arguments Pour/Contre** présentant l'un des camps de façon plus favorable, plus longue ou mieux sourcée que l'autre.

7. **L'utilisation du projet à des fins commerciales ou d'orientation politique** (voir `LICENSE_SUPPLEMENT.txt`).

---

## Protocole éditorial

### La question (proposition normative)
- Affirmation à laquelle l'utilisateur peut répondre d'accord ou en désaccord.
- Sans adverbe évaluatif : pas de *"enfin"*, *"malheureusement"*, *"encore"*.
- Sans présupposé implicite dans la formulation.

### Le contexte factuel
- Uniquement des données vérifiables : chiffres officiels, dates, définitions légales.
- Zéro opinion, zéro jugement, zéro argument.

### Les arguments Pour et Contre
- Chaque camp défend **sa propre position positivement**, jamais en attaquant l'autre.
- Format obligatoire : *"Ses partisans estiment que…"* / *"Ses opposants estiment que…"*
- Longueur comparable (±20 % de mots).
- Aucun terme évaluatif : *"légitime"*, *"inacceptable"*, *"évident"*, *"démagogie"*.

### Les positions candidats
- Basées sur les programmes officiels, votes en assemblée ou déclarations formelles.
- Chaque position modifiée doit être sourcée dans la PR.

---

## Ajouter une nouvelle édition

Pour créer l'édition 2027 ou toute autre édition :

1. Créez un dossier `2027/` à la racine du dépôt.
2. Copiez la structure de `2022/` comme point de départ.
3. Mettez à jour `README.md` à la racine pour référencer la nouvelle édition.
4. Respectez strictement le protocole éditorial pour toutes les nouvelles données.
5. Ouvrez une Issue avec le label `[nouvelle-édition]` avant de commencer pour coordonner le travail.

Chaque édition doit rester un fichier `index.html` autonome.

---

## Labels d'Issues

| Label | Usage |
|-------|-------|
| `[données-2022]` | Erreur dans les données de l'édition 2022 |
| `[données-2027]` | Erreur dans les données de l'édition 2027 |
| `[neutralité]` | Biais éditorial perçu |
| `[algorithme]` | Question sur le calcul |
| `[nouvelle-édition]` | Discussion sur une nouvelle édition |
| `[licence]` | Question sur l'usage du projet |
| `[vie-privée]` | Mécanisme de collecte de données détecté |

---

## Obligation AGPL sur les forks déployés en ligne

Si vous modifiez ce projet et le déployez comme service accessible sur un réseau, vous avez l'obligation de rendre votre code source modifié disponible aux utilisateurs, sous la même licence AGPL-3.0. Cela s'applique même sans distribution de binaire.

---

## Questions

Si vous hésitez sur la recevabilité d'une contribution, **ouvrez d'abord une Issue** avant de soumettre une PR.

---

*Ce guide est lui-même soumis aux mêmes principes de neutralité. Toute modification affaiblissant les critères de neutralité sera refusée.*
