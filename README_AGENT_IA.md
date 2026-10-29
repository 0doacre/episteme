# Guide Opérationnel pour Agents IA & LLM

Ce document définit les règles méthodologiques strictes, la grille des **niveaux de preuve (HAS)**, le schéma JSON complet et le prompt d'amorce permettant à un agent d'intelligence artificielle de documenter en profondeur un sujet et d'enrichir le corpus d'**Épistémê**.

---

## 🎯 Règles Méthodologiques Impératives

1. **Règle d'or : Validité Épistémique & Filtre Anti-Faux Équilibre (No False Balance)**
   - Ne traitez **JAMAIS** un consensus scientifique résolu ou une contestation idéologique/conspirationniste comme une controverse scientifique active.
   - 🚫 *Interdits formels :* Climatoscepticisme vs GIEC, Vaccins vs Autisme, Terre plate, Créationnisme vs Évolution, Révisionnisme historique.
   - ✅ *Controverses valides :* Théories de la conscience en neurosciences computationnelles, Méthodes d'enseignement et théorie de la charge cognitive, Gravité quantique à boucles vs Cordes, Origine de l'architecture cognitive humaine (modularité vs plasticité), Microéconomie néoclassique vs Économie comportementale.
2. **Niveaux de Preuve Méthodologique (Standard HAS / Evidence-Based Science)**
   - Chaque thèse et ressource documentaire doit être explicitement évaluée selon la grille de la Haute Autorité de Santé (HAS) :
     - **Grade A (Niveau 1) — Preuve Scientifique Établie :** Méta-analyses d'essais contrôlés randomisés (ECR) de forte puissance, revues systématiques, études de cohortes massives répliquées.
     - **Grade B (Niveau 2) — Présomption Scientifique :** Essais comparatifs randomisés sur échantillons restreints, quasi-expériences bien menées, mesures biomédicales directes.
     - **Grade C (Niveau 3) — Faible Niveau de Preuve :** Études corrélationnelles observationnelles, études cas-témoins, données de laboratoire sur échantillons spécifiques (ex. WEIRD).
     - **Grade D (Niveau 4) — Modèle Théorique Déductif / Accord d'Experts :** Formalisations mathématiques sans données empiriques directes (ex. échelle de Planck), séries de cas, consensus informel d'experts.
3. **Densité Didactique & Auto-Suffisance de l'Apprenant**
   - L'utilisateur doit pouvoir **comprendre les mécanismes intimes du débat sans aller lire les articles** :
     - Définir les 3 à 5 concepts clés (*Glossaire*) et expliquer *pourquoi chaque terme est capital*.
     - Poser le *Socle Commun* (ce sur quoi tout le monde est d'accord) pour éviter les procès d'intention.
     - Découper le désaccord en 3 ou 4 *axes de clivage précis* avec arguments et objections réciproques.
     - Citer 2 à 3 *expériences empiriques réelles* avec le protocole, le résultat observé et l'impact.
     - Traiter 3 *questions tranchantes / idées reçues (FAQ)*.
4. **Principe de Charité Épistémique (Steelman)**
   - Exposer chaque position sous sa forme la plus solide, la plus noble et la plus rigoureuse possible.

---

## 📋 Schéma JSON Strict

```json
[
  {
    "id": "identifiant-unique-kebab-case",
    "domain": "Discipline académique (ex. Neurosciences & IA)",
    "title": "Titre explicite de la controverse",
    "subtitle": "Question didactique centrale résumant l'enjeu",
    "definition": "Définition approfondie de la fracture épistémique (pourquoi le débat existe et ce qui se joue).",
    "guardrail": "Exclusion explicite des dérives pseudoscientifiques ou idéologiques (filtre No False Balance).",
    "glossary": [
      {
        "term": "Terme ou concept clé",
        "definition": "Définition concise et claire sans jargon inutile.",
        "whyItMatters": "Explication de pourquoi cette notion est indispensable pour comprendre le débat."
      }
    ],
    "agreements": [
      {
        "point": "Point de consensus scientifique non négociable",
        "explanation": "Explication factuelle partagée par l'ensemble des chercheurs des deux camps."
      }
    ],
    "divergences": [
      {
        "axis": "Intitulé de la ligne de fracture (ex. Substrat, Méthode, Rôle de l'erreur)",
        "thesis1Stance": "Position argumentée de la Thèse 01",
        "thesis2Stance": "Position argumentée de la Thèse 02",
        "analysis": "Analyse didactique expliquant la racine théorique ou méthodologique du désaccord."
      }
    ],
    "empiricalTests": [
      {
        "experimentName": "Nom de l'étude ou expérience princeps",
        "yearOrContext": "Année ou contexte institutionnel",
        "protocol": "Protocole expérimental mis en œuvre.",
        "finding": "Données et résultats observés.",
        "impactOnDebate": "Conséquence directe sur la confrontation des deux théories."
      }
    ],
    "qa": [
      {
        "question": "Question naïve ou idée reçue fréquente ?",
        "answer": "Réponse étayée, pédagogique et nuancée démontant les confusions."
      }
    ],
    "positions": [
      {
        "name": "Intitulé du Courant A",
        "summary": "Résumé de l'architecture théorique.",
        "evidenceLevel": {
          "grade": "Grade A | Grade B | Grade C | Grade D",
          "levelText": "Niveau 1 — Preuve établie | Niveau 2 — Présomption | Niveau 3 — Faible | Niveau 4 — Modèle théorique",
          "justification": "Justification méthodologique selon les critères HAS."
        },
        "keyArguments": [
          "Argument fort 1",
          "Argument fort 2"
        ],
        "counterCritique": "Objection technique adressée au camp adverse.",
        "keyFigures": ["Auteur A", "Auteur B"]
      },
      {
        "name": "Intitulé du Courant B",
        "summary": "Résumé de l'architecture théorique.",
        "evidenceLevel": {
          "grade": "Grade A | Grade B | Grade C | Grade D",
          "levelText": "Niveau 1 — Preuve établie | Niveau 2 — Présomption | Niveau 3 — Faible | Niveau 4 — Modèle théorique",
          "justification": "Justification méthodologique selon les critères HAS."
        },
        "keyArguments": [
          "Argument fort 1",
          "Argument fort 2"
        ],
        "counterCritique": "Objection technique adressée au camp adverse.",
        "keyFigures": ["Auteur C", "Auteur D"]
      }
    ],
    "readings": [
      {
        "level": "Facile | Moyen | Difficile | Expert",
        "evidenceGrade": "Grade A | Grade B | Grade C | Grade D",
        "evidenceLevel": "Niveau 1 | Niveau 2 | Niveau 3 | Niveau 4",
        "title": "Titre exact de la ressource",
        "type": "Type d'écrit",
        "author": "Auteur(s)",
        "link": "https://url-reelle-ou-doi",
        "note": "Raison pédagogique d'aborder ce texte."
      }
    ]
  }
]
```

---

## 💬 Prompt d'Amorce Recommandé pour LLM

```text
Agis en tant que didacticien des sciences et expert en épistémologie appliquée (méthodologie des Questions Socialement Vives - QSV et standard HAS).

Analyse le sujet suivant : [INSÉRER LE SUJET OU LA QUESTION SCIENTIFIQUE]

Consignes strictes :
1. DENSITÉ MAXIMALE : Ne te contente pas d'un résumé superficiel. L'apprenant doit TOUT comprendre directement dans l'interface sans aller lire les articles.
2. NIVEAUX DE PREUVE HAS : Évalue scrupuleusement chaque thèse et lecture selon la grille HAS (Grade A / B / C / D).
3. LEXIQUE : Définis 4 à 5 termes clés indispensables et explique pour chacun 'pourquoi c'est capital'.
4. CONSENSUS & DIVERGENCES : Dégage le socle commun partagé et 3 axes de désaccord tranchés avec l'analyse didactique.
5. EXPÉRIENCES : Documente 2 expériences scientifiques réelles avec protocole, résultats et impact.
6. FAQ : Réponds à 3 questions percutantes déconstruisant les idées reçues.
7. FORMAT : Retourne exclusivement un tableau JSON valide strictement conforme au schéma Épistémê.
```
