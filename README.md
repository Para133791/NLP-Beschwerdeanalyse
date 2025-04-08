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

```
NLP-Beschwerdeanalyse/
├── README.md                 # Projektbeschreibung  
├── konzept.pdf               # Konzeptdokument mit Zielsetzung und Methodik  
├── data/                     # Datensätze (z. B. consumer_complaints.csv)  
├── notebooks/                # Explorative Analyse in Jupyter Notebooks  
│   ├── 1_Datenvorverarbeitung.ipynb  
│   ├── 2_Vektorisierung.ipynb  
│   └── 3_Themenextraktion.ipynb  
├── src/                      # Wiederverwendbare Python-Module  
│   ├── preprocessing.py      # Funktionen zur Textbereinigung  
│   ├── vectorization.py      # Vektorisierungsmethoden (z. B. TF-IDF)  
│   └── topic_extraction.py   # LDA-Topic-Modellierung und Visualisierung  
└── results/                  # Ergebnisse, Plots und Themencluster  
```

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
- tqdm

## Repository klonen

```bash
git clone https://github.com/Para133791/NLP-Beschwerdeanalyse.git
cd NLP-Beschwerdeanalyse
```

## Conda-Umgebung erstellen (optional):

```bash
conda create -n nlp_projekt python=3.11
conda activate nlp_projekt
pip install -r requirements.txt
```

## Ergebnisse
Die Analyse identifiziert die Hauptthemen in den Beschwerdetexten und visualisiert deren Verteilung. Die detaillierten Ergebnisse sind in den Notebooks und im Results-Ordner zu finden.

Die finalen Ergebnisse der Analyse befinden sich im Ordner `results/`. Darunter:
- Visualisierungen der Themenverteilungen
- Interaktive LDA-Visualisierung via pyLDAvis
- Auswertung häufiger Schlagwörter und Themencluster

## Lizenz
Dieses Projekt untersteht der MIT-Lizenz.
