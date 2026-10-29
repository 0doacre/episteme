# Guide Opérationnel pour Agents IA & LLM

Ce document définit les règles méthodologiques, le schéma JSON strict et le prompt d'amorce permettant à un agent d'intelligence artificielle de documenter un nouveau sujet et de générer un corpus compatible avec **Épistémê**.

---

## 🎯 Règles Méthodologiques Impératives

1. **Règle d'or : Validité Épistémique & Filtre Anti-Faux Équilibre**
   - Ne traitez **JAMAIS** une controverse sociale, politique ou médiatique résolue sur le plan scientifique comme une controverse scientifique.
   - 🚫 *Sujets strictement interdits :* "Climatoscepticisme vs GIEC", "Vaccins vs Autisme", "Terre plate vs Ronde", "Créationnisme vs Évolution", "Révisionnisme historique".
   - ✅ *Sujets scientifiques valides :* "Rythmes de la spéciation (Équilibres ponctués vs Gradualisme phylétique)", "Théorie monétaire moderne vs Monétarisme", "Nature du temps en relativité générale vs mécanique quantique", "Origine de la cognition morale".
2. **Principe de Charité Épistémique (*Steelman*)**
   - Chaque position doit être formulée sous sa forme la plus solide, la plus noble et la plus rigoureuse possible, telle qu'énoncée par ses chercheurs et théoriciens de référence.
   - Ne caricaturez jamais une thèse pour en favoriser une autre.
3. **Gradation Documentaire à 4 Paliers**
   - Fournissez toujours 4 ressources réelles et vérifiables, graduées selon l'effort cognitif requis :
     - `Facile` : Ouvrage ou article de vulgarisation de haute tenue.
     - `Moyen` : Article de synthèse, chapitre de manuel universitaire ou rapport de consensus.
     - `Difficile` : Article de recherche primaire avec protocole ou formalisme.
     - `Expert` : Monographie de référence, traité exhaustif ou méta-analyse majeure.
4. **Format de Sortie Strict**
   - L'agent doit retourner **exclusivement** un tableau JSON valide respectant la structure définie ci-dessous, sans texte d'introduction ni conclusion.

---

## 📋 Schéma JSON Strict

```json
[
  {
    "id": "identifiant-unique-en-kebab-case",
    "domain": "Discipline académique (ex. Linguistique, Économie, Neurosciences)",
    "title": "Titre synthétique et explicite de la controverse",
    "definition": "Définition concise de la ligne de fracture méthodologique ou paradigmatique (2 à 3 phrases claires).",
    "guardrail": "Exclusion explicite des dérives pseudoscientifiques ou idéologiques et précision du cadre de scientificité.",
    "positions": [
      {
        "name": "Intitulé du Courant ou Thèse 01",
        "summary": "Résumé de l'argumentaire théorique, des hypothèses centrales et des données probantes mobilisées.",
        "keyFigures": ["Auteur A", "Auteur B"]
      },
      {
        "name": "Intitulé du Courant ou Thèse 02",
        "summary": "Résumé de l'argumentaire théorique, des hypothèses centrales et des données probantes mobilisées.",
        "keyFigures": ["Auteur C", "Auteur D"]
      }
    ],
    "readings": [
      {
        "level": "Facile",
        "title": "Titre exact de la ressource",
        "type": "Vulgarisation réflexive / Essai grand public",
        "author": "Nom de l'auteur ou de l'éditeur",
        "link": "https://lien-reel-ou-doi-ou-hashtag",
        "note": "Raison pédagogique d'aborder cette ressource en amorce."
      },
      {
        "level": "Moyen",
        "title": "Titre exact de la ressource",
        "type": "Article de synthèse / Manuel de référence",
        "author": "Nom de l'auteur",
        "link": "https://lien-reel-ou-doi-ou-hashtag",
        "note": "Apport conceptuel intermédiaire et mise en perspective."
      },
      {
        "level": "Difficile",
        "title": "Titre exact de la ressource",
        "type": "Article de recherche pair-à-pair / Modélisation",
        "author": "Nom de l'auteur",
        "link": "https://lien-reel-ou-doi-ou-hashtag",
        "note": "Formalisation formelle ou données empiriques clés."
      },
      {
        "level": "Expert",
        "title": "Titre exact de la référence",
        "type": "Traité théorique canonique / Méta-analyse",
        "author": "Nom de l'auteur",
        "link": "https://lien-reel-ou-doi-ou-hashtag",
        "note": "Ouvrage de référence exhaustif pour approfondissement maximal."
      }
    ]
  }
]
```

---

## 💬 Prompt d'Amorce Recommandé pour LLM

Copiez-collez ce prompt à votre modèle IA pour générer de nouvelles entrées :

```text
Agis en tant que didacticien et sociologue des sciences spécialisé dans l'analyse des controverses (méthode des Questions Socialement Vives - QSV).

Analyse le sujet suivant : [INSÉRER LE DOMAINE OU LE SUJET ICI]

Consignes :
1. Identifie la ligne de fracture épistémique ou méthodologique active au sein de la communauté scientifique.
2. Écarte formellement tout faux équilibre avec des pseudosciences ou du conspirationnisme (règle No False Balance).
3. Expose les deux thèses majeures selon le principe de charité épistémique (steelman).
4. Fournis 4 lectures réelles et vérifiables (Facile, Moyen, Difficile, Expert) avec liens DOI, revues ou URL exactes.
5. Produis strictement un tableau JSON valide conforme au schéma Épistémê, sans aucun texte introductif ni markdown autour.
```
