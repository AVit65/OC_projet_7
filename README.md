**CreditRiskScore**

La société Prêt à Dépenser est une société financière  qui propose des crédits à la consommation. 
Dans une logique de gestion du risque, l’entreprise souhaite mettre en place un outil de scoring de crédits capable d’estimer 
la probabilité qu’un client rembourse son emprunt. Cet outil permettra de classer automatiquement les demandes en deux catégories : 
les demandes de prêts peu risquées qui seront acceptées ou les demandes de prêts risquées qui seront refusées. Pour déveloper ce modèle 
de classification, la société fournit un large pannel de données provenant de différentes sources et inclus des informations comportementales 
et des données issues d'autres institutions financières.

**Architecture du repository**

```
OC_projet_7/
│
├── README.md                        # Documentation générale du projet  
├── requirements.txt                 # Package Python nécessaire au déploiement de l'API 
├── .gitignore                       # Fichiers à ignorer si Git est utilisé 
│
├── .github/workflows       
│   ├── deployed.yml/                # Workflow de déploiement de l'API 
│   ├── test.yml/                    # Workflow de test de l'API 
│
├── Data/                             # Données 
│   ├── App_test_final.csv/           # Table de caractéristiques client utilisée dans la modélisation  
│   └── pipeline_to_deployed.joblib/  # Pipeline de modélisation entrainée   
│
├── notebooks/                        # Notebooks d'exploration et de modélisation
│
├── API/                              # Code source principal
│   ├── __init__.py
│   ├── app.py/                       # Code de l'API
│
├── Test/                 
    ├── __init__.py
    ├── test_api.py/                  # Tests unitaires et d'intégration


```

