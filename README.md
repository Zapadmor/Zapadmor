# Zapadmor

Étudiant ingénieur en alternance. Je m'intéresse aux systèmes où la fiabilité
prime : perception par capteurs, chaînes logicielles reproductibles et testées.

## Domaines

- Perception : modèle de caméra, segmentation sémantique, détection d'objets, nuages de points Lidar
- Positionnement : GNSS (pseudodistances, moindres carrés)
- Données : Python, SQL, pipelines d'ingestion
- Ingénierie : tests automatisés, intégration continue, conteneurs

## Projet public

### [DynaStasis](https://github.com/Zapadmor/DynaStasis)

Tableau de bord hebdomadaire personnel, local et sans compte. Il agrège des
sources de données facultatives (sport, temps d'écran, finances) dans une base
SQLite et en tire un score configurable.

Ce que le dépôt permet de vérifier :

- Isolation des pannes : chaque source est synchronisée dans son propre processus,
  avec un délai maximal ; l'échec d'une source est consigné et n'arrête pas les autres.
- Traçabilité : journaux JSON, statut par source dans l'interface, migrations de
  base numérotées.
- Qualité : 223 tests, lint et format (ruff), détection de code mort (vulture),
  dépendances verrouillées, le tout exécuté en CI.
- Livraison : image Docker multi-étapes, utilisateur non-root, HEALTHCHECK, analyse
  Trivy en CI ; démo reproductible en une commande, avec des données fictives.

Limites : outil personnel mono-utilisateur, non certifié ; seuil de couverture
imposé en CI de 60 %.

Pile : Python 3.12, Streamlit, SQLite, Docker, GitHub Actions.

## Travaux non publiables

Une partie de mes travaux, industriels et académiques, est soumise à des
obligations de confidentialité et n'est pas publiée ici.

## Contact

zapadmor.research@proton.me
