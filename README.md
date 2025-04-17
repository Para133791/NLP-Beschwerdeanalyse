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
├── notebooks/                # Explorative Analyse in Jupyter Notebooks  
│   ├── 1_Datenvorverarbeitung.ipynb  
│   ├── 2_Vektorisierung.ipynb  
│   └── 3_Themenextraktion.ipynb   
└── results/                  # Ergebnisse und Themencluster  
```

Einige Ordnerstrukturen sind nicht auf Anhieb erkennbar, diese werden im Verlauf vom ausführen des Codes, Schritt für Schritt hinzugefügt. 

- `notebooks/`: Jupyter Notebooks mit der schrittweisen Analyse
- `data/`: Rohdaten und vorverarbeitete Datensätze | werden lokal gespeichert aufgrund der Größe
- `results/`: Visualisierungen und Ergebnisse der Analyse

## Methodik
- **Datenvorverarbeitung**: Textreinigung, Entfernen von Stoppwörtern, Lemmatisierung
- **Vektorisierung**: TF-IDF und BoW
- **Themenextraktion**: Latent Semantic Analysis (LSA)

## Benötigte Bibliotheken

| Bibliothek     | Beschreibung                                                                 |
|----------------|------------------------------------------------------------------------------|
| pandas         | Datenanalyse- und Datenstruktur-Tool für tabellarische Daten.                |
| nltk           | Natural Language Toolkit für klassische Textverarbeitung und Linguistik.     |
| scikit-learn   | Bibliothek für maschinelles Lernen und statistische Modellierung.            |
| gensim         | Topic Modeling und semantische Modellierung mit Word2Vec, LDA.           |
| spacy          | Industrietaugliche NLP-Bibliothek mit Fokus auf Effizienz und Genauigkeit.   |
| matplotlib     | Grundlegende Bibliothek zum Erstellen von statischen Visualisierungen.       |
| seaborn        | Erweiterung von matplotlib für ansprechende statistische Visualisierungen.   |
| numpy          | Grundlage für numerische Berechnungen und Matrizenoperationen in Python.     |
| jupyterlab     | Web-basierte Entwicklungsumgebung für interaktives Coding und Analyse.       |
| notebook       | Klassisches Jupyter Notebook-Interface zur interaktiven Codeausführung.      |
| joblib         | Effizientes Serialisieren und Caching von Modellen und Arrays.               |
| symspellpy     | Schneller Rechtschreibkorrektur-Algorithmus basierend auf Symmetric Delete.  |
| wordcloud      | Erstellt Wortwolken zur Visualisierung der wichtigsten Begriffe in Daten.    |

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

![image](https://github.com/user-attachments/assets/db576346-8c53-4719-8ce0-6fa93cfa3864)


## Ergebnisse
Die Analyse identifiziert die Hauptthemen in den Beschwerdetexten und visualisiert deren Verteilung. Die detaillierten Ergebnisse sind **nach dem ausführen der Notebooks**, direkt im Notebook sichtbar bzw. die modifizierten Daten sowie Bilder in *results* zu finden.

Die finalen Ergebnisse der Analyse befinden sich im Ordner `results/`. Darunter:
- Visualisierungen der Themenverteilungen
- Auswertung häufiger Schlagwörter und Themencluster

## Lizenz
Dieses Projekt untersteht der MIT-Lizenz.
