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
- Visualisierung relevanter Ergebnisse

## Projektstruktur

```
NLP-Beschwerdeanalyse/
├── README.md                 # Projektbeschreibung  
├── data/                     # Datensätze (z. B. consumer_complaints.csv)
├── models/                   # Gespeicherte Modelle und Vektoren
├── notebooks/                # Jupyter Notebooks  
│   ├── 1_Datenvorverarbeitung.ipynb  
│   ├── 2_Vektorisierung.ipynb  
│   └── 3_Themenextraktion.ipynb   
└── results/                  # Ergebnisse, Plots und Themencluster  
```

Einige Ordnerstrukturen sind nicht auf Anhieb erkennbar, diese werden im Verlauf vom ausführen des Codes, Schritt für Schritt hinzugefügt. 

- `notebooks/`: Jupyter Notebooks mit der schrittweisen Analyse
- `data/`: Rohdaten und vorverarbeitete Datensätze | werden lokal gespeichert aufgrund der Größe
- `results/`: Visualisierungen und Ergebnisse der Analyse
- `models/`: verarbeitete NLP Modelle | werden lokal gespeichert aufgrund der Größe

## Beschreibung der Module

1. **Datenvorverarbeitung**: 
   - Bereinigung der Rohtexte (Kleinschreibung, Entfernen von Sonderzeichen)
   - Tokenisierung, Entfernen von Stoppwörtern und Lemmatisierung
   - Speicherung der vorverarbeiteten Texte für weitere Analysen

2. **Vektorisierung**: 
   - TF-IDF: Gewichtung relevanter Begriffe basierend auf Häufigkeit und Seltenheit
   - Bag-of-Words: Worthäufigkeiten für LDA-Themenmodellierung
   - Word2Vec: Erzeugung semantisch reicher Worteinbettungen
   - Erstellung von Dokumentenvektoren für weiteres Clustering

3. **Themenextraktion**:
   - LDA (Latent Dirichlet Allocation): Identifikation von Themen mittels Bag-of-Words
   - LSA/SVD: Dimensionsreduktion und Themenextraktion aus TF-IDF
   - K-Means-Clustering: Gruppierung ähnlicher Beschwerden basierend auf Word2Vec
   - Visualisierung und Interpretation der extrahierten Themen

## Benötigte Bibliotheken
**Datenverarbeitung und NLP:**
- **pandas**: Datenverarbeitung und -manipulation
- **numpy**: Numerische Berechnungen und Arrays
- **nltk**: Tokenisierung, Stopwörter, Lemmatisierung
- **spacy**: Fortgeschrittene NLP-Funktionen und Sprachmodelle
- **re**: Reguläre Ausdrücke für Textbereinigung

**Maschinelles Lernen und Vektorisierung:**
- **scikit-learn**: TF-IDF, Vektorisierung, Clustering
- **gensim**: Word2Vec und Topic-Modellierung

**Visualisierung und Ausgabe:**
- **matplotlib**: Erstellung von Diagrammen und Visualisierungen
- **seaborn**: Erweiterte statistische Visualisierungen

**Hilfswerkzeuge:**
- **joblib**: Sichere Modellspeicherung und -ladung
- **json**: Speicherung von strukturierten Daten

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

# Nur bei Bedarf
# Unter VSCode auf Mac musste ich mit:
python -m ipykernel install --user --name nlp_projekt --display-name "Python (nlp_projekt)"

# den Kernel speichern und ihn dann zu finden, danach folgende Schritte durchführen:
```
1.	Starte VS Code neu
2.	Öffne dein .ipynb-Notebook
3.	Oben rechts auf den Kernel-Namen klicken
4.	Wähle: “Python (nlp_projekt)”



## Ergebnisse
Die Analyse identifiziert die Hauptthemen in den Beschwerdetexten und visualisiert deren Verteilung. Die detaillierten Ergebnisse sind **nach dem ausführen der Notebooks**, direkt im Notebook sichtbar bzw. die modifizierten Daten sowie Bilder in *results* zu finden.

Die finalen Ergebnisse der Analyse befinden sich im Ordner `results/`. Darunter:
- Visualisierungen der Themenverteilungen
- Interaktive LDA-Visualisierung via pyLDAvis
- Auswertung häufiger Schlagwörter und Themencluster

## Lizenz
Dieses Projekt untersteht der MIT-Lizenz.
