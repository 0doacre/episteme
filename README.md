# Épistémê — Cartographie Didactique des Controverses Scientifiques & Épistémiques

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Format](https://img.shields.io/badge/Format-Standalone_HTML5-emerald.svg)](index.html)
[![UI](https://img.shields.io/badge/Theme-Notion_%2F_Linear-neutral.svg)](index.html)

**Épistémê** est une application web autonome et minimaliste conçue pour explorer et travailler sur les controverses scientifiques actives à travers le prisme de la didactique des sciences et des **Questions Socialement Vives (QSV)**.

L'application permet d'échapper au dogmatisme comme au relativisme naïf, en fournissant une grille rigoureuse d'analyse, un corpus documentaire gradué à 4 paliers et un atelier de décentration cognitive (méthode de Johnson & Johnson).

---

## 🧭 Principes Épistémologiques & Didactiques

1. **La controverse comme moteur de la science (*Science-in-the-making*) :**
   Le savoir scientifique n'est pas un bloc statique de dogmes tombés du ciel, mais une dynamique d'épreuves empiriques, de débats méthodologiques et d'arbitrages de pairs. Aborder un domaine par ses lignes de fracture permet de comprendre la fabrication de la preuve.
2. **Le filtre Anti-Faux Équilibre (*No False Balance*) :**
   Une controverse scientifique n'est pas une confrontation d'opinions médiatiques. Elle ne réunit que des positions rationnelles et étayées au sein du champ académique. Sont formellement exclus : les négationnismes, pseudosciences, complotismes et dénis de consensus établis (ex. climat, vaccination).
3. **La progression documentaire à 4 paliers :**
   - **Facile :** Vulgarisation réflexive et clarification conceptuelle sans jargon inutile.
   - **Moyen :** Articles de référence, revues de littérature et synthèses méthodologiques.
   - **Difficile :** Articles de recherche primaires avec formalisation et données empiriques.
   - **Expert :** Traités canoniques, monographies universitaires et méta-analyses exhaustives.
4. **Atelier de Décentration (*Steelman* & Johnson & Johnson) :**
   Pour valider l'appropriation rationnelle d'un sujet, l'app invite l'apprenant à formuler avec un maximum de charité épistémique le meilleur argument de la position adverse.

---

## 🔬 Corpus Initial Inclus

L'application est préconfigurée avec 5 controverses majeures couvrant différents domaines de la connaissance :

1. **Neurosciences & IA :** *Théories de la conscience & Architecture des LLM* (Fonctionnalisme computationnel & GNWT vs Biologisme strict & IIT).
2. **Sciences de l'Éducation :** *Enseignement explicite vs Pédagogies par découverte guidée* (Direct Instruction / Théorie de la charge cognitive vs Échec productif / Socio-constructivisme).
3. **Physique Fondamentale :** *Unification : Théorie des Cordes vs Gravité Quantique à Boucles* (Supersymétrie d'espace-temps vs Réseau de spin indépendant du fond).
4. **Sciences Cognitives & Anthropologie :** *Psychologie Évolutionniste : Modularité massive vs Plasticité culturelle* (Adaptationnisme pléistocène vs Co-évolution gène-culture).
5. **Économie & Sciences de la Décision :** *Rationalité Limitée vs Théorie du Choix Rationnel* (Heuristiques et biais cognitifs vs Modélisation néoclassique et maximisation de l'utilité).

---

## 🚀 Utilisation & Déploiement

### Exécution Locale Immédiate
Aucun serveur ni installation Node.js n'est nécessaire :
1. Téléchargez ou clonez ce dépôt.
2. Double-cliquez sur `index.html` pour l'ouvrir dans n'importe quel navigateur moderne (Chrome, Firefox, Safari, Edge).

### Fonctionnalités Clés
- **Recherche & Filtrage :** Filtrage instantané par domaine et recherche plein texte (titres, définitions, auteurs repères).
- **Liens Documentaires Directs :** Accès direct vers les articles fondateurs (arXiv, DOI, Revues) ou requêtes ciblées sur Google Scholar.
- **Import / Export JSON :** Exportez vos données en un clic ou importez de nouveaux corpus personnalisés.
- **Persistance Navigateur :** Vos notes de décentration et corpus importés sont conservés automatiquement dans le `localStorage`.

### Déploiement sur GitHub Pages
Le dépôt inclut une configuration prête pour GitHub Pages :
1. Rendez-vous dans les **Settings** de votre dépôt GitHub > **Pages**.
2. Dans **Branch**, sélectionnez `main` et dossier `/ (root)`, puis validez.
3. L'application sera immédiatement accessible en ligne publiquement.

---

## 🤖 Alimentation par Agents IA

Vous pouvez étendre le corpus à l'infini en demandant à un modèle d'IA (Gemini, Claude, GPT-4) d'analyser un sujet selon notre schéma strict.

👉 Consultez le guide dédié : **[README_AGENT_IA.md](README_AGENT_IA.md)** pour le prompt d'amorce et le schéma JSON normé.

---

## 📄 Licence

Ce projet est sous licence MIT — libre d'utilisation, de modification et de distribution.
