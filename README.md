# SSIAP Helper

## 1. Présentation du projet

SSIAP Helper est une application d'assistance intelligente destinée aux agents de sécurité incendie.

L'objectif est d'accompagner les agents lors du traitement d'une alarme incendie ou intrusion, en s'appuyant sur les documents, plans et procédures validées du site.

L'application utilise l'intelligence artificielle multimodale pour analyser une photo d'alarme et identifier les informations affichées.

Elle propose ensuite un accompagnement étape par étape, avec confirmation de l'utilisateur avant de poursuivre.

**SSIAP Helper est un outil d'assistance. Il ne remplace pas les procédures officielles, les décisions des agents habilités ou les dispositifs de sécurité.**

## 2. Fonctionnalités prévues

- Analyse des photos d'alarmes par un modèle multimodal.
- Identification des alarmes incendie et intrusion.
- Recherche documentaire dans les PDF et plans du site (RAG).
- Consultation des procédures d'intervention validées.
- Accompagnement étape par étape.
- Gestion des confirmations et difficultés rencontrées.
- Interface Streamlit dans un premier temps.
- Intégration WhatsApp dans une version ultérieure.

## 3. Stack technique

| Technologie | Utilisation |
|---|---|
| Python 3.12 | Développement |
| PyCharm | Environnement de développement |
| LangChain | Intégration des modèles IA |
| LangGraph | Orchestration des workflows |
| OpenAI | Analyse multimodale |
| ChromaDB | Recherche vectorielle |
| PyMuPDF | Traitement des PDF |
| Pydantic | Validation des données |
| Streamlit | Interface utilisateur |
| Git / GitHub | Versionnement |

## 4. Architecture du projet

```text
ssiap_helper/
├── src/
│   ├── agents/       # Agents IA spécialisés
│   ├── graph/        # Orchestration LangGraph
│   ├── rag/          # Recherche documentaire
│   ├── prompts/      # Prompts des modèles
│   ├── schemas/      # Modèles de données
│   ├── services/     # Logique métier
│   └── interfaces/   # Streamlit et WhatsApp
├── data/             # Documents locaux du site
├── tests/            # Tests du projet
└── README.md         # Documentation
```

## 5. Avancement

- [x] Création du projet PyCharm.
- [x] Configuration de Python 3.12.
- [x] Création de l'environnement virtuel `.venv`.
- [x] Création de l'arborescence.
- [ ] Initialisation Git et connexion GitHub.
- [ ] Installation des dépendances.
- [ ] Premier appel au modèle multimodal.
- [ ] Création du système RAG.
- [ ] Création du workflow LangGraph.
- [ ] Développement de l'interface Streamlit.
- [ ] Tests et validation.

## 6. Sécurité et confidentialité

Les documents du site, plans de sécurité, procédures sensibles et clés API ne doivent pas être publiés dans le dépôt Git.

Les procédures utilisées pour guider une intervention doivent être approuvées par les responsables compétents. En cas d'information incertaine, l'application doit demander une vérification humaine et ne pas inventer de consignes.

L'utilisation opérationnelle nécessitera une validation de sécurité et de fiabilité préalable.