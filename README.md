# NLP-Beschwerdeanalyse
Datenanalyse Projekt von Beschwerden im Bereich US Consumer Finance Complaints von Kaggle (Uni Projekt)

## Dataset
Download Link: https://www.kaggle.com/datasets/kaggle/us-consumer-finance-complaints
Das Datenset muss heruntergeladen werden sowie die ".csv" Datei in den Ordner "data" gelegt werden, bevor die notebooks genutzt werden können.

## Projektbeschreibung
Diese Analyse verwendet den "Customer Complaints Database" vom Consumer Financial Protection Bureau (CFPB), um zu demonstrieren, wie unstrukturierte Beschwerde-Texte systematisch analysiert werden können. Das Projekt zeigt eine vollständige NLP-Pipeline von der Datenvorverarbeitung bis zur Themenextraktion.

## Projektziele

- Extraktion von häufigen Beschwerdethemen aus einem englischsprachigen Datensatz
- Anwendung der NLP-Techniken
- Erstellung wiederverwendbarer Code-Module für Preprocessing und Analyse
- Visualisierung relevanter Ergebnisse

## Projektstruktur

NLP-Beschwerdeanalyse/
├── README.md                 # Projektbeschreibung
├── konzept.pdf               # Dein Konzeptdokument
├── data/                     # Datensätze
├── notebooks/                # Jupyter Notebooks
│   ├── 1_Datenvorverarbeitung.ipynb
│   ├── 2_Vektorisierung.ipynb
│   └── 3_Themenextraktion.ipynb
├── src/                      # Python-Skripte
│   ├── preprocessing.py
│   ├── vectorization.py
│   └── topic_extraction.py
└── results/                  # Ergebnisse und Visualisierungen

- `notebooks/`: Jupyter Notebooks mit der schrittweisen Analyse
- `data/`: Rohdaten und vorverarbeitete Datensätze
- `results/`: Visualisierungen und Ergebnisse der Analyse

## Methodik
- **Datenvorverarbeitung**: Textreinigung, Entfernen von Stoppwörtern, Lemmatisierung
- **Vektorisierung**: TF-IDF und Word2Vec
- **Themenextraktion**: Latent Semantic Analysis (LSA)

## Benötigte Bibliotheken
- pandas
- nltk
- scikit-learn
- gensim
- spacy
- matplotlib
- seaborn
- numpy

## Ergebnisse
Die Analyse identifiziert die Hauptthemen in den Beschwerdetexten und visualisiert deren Verteilung. Die detaillierten Ergebnisse sind in den Notebooks und im Results-Ordner zu finden.

## Autor
Adrian Gashi

## Lizenz
Dieses Projekt untersteht der MIT-Lizenz.
