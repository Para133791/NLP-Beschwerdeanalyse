# NLP-Beschwerdeanalyse
Datenanalyse Projekt von Beschwerden im Bereich US Consumer Finance Complaints von Kaggle (Uni Projekt)

## Projektbeschreibung
Diese Analyse verwendet den "Customer Complaints Database" vom Consumer Financial Protection Bureau (CFPB), um zu demonstrieren, wie unstrukturierte Beschwerde-Texte systematisch analysiert werden können. Das Projekt zeigt eine vollständige NLP-Pipeline von der Datenvorverarbeitung bis zur Themenextraktion.

## Projektstruktur
- `notebooks/`: Jupyter Notebooks mit der schrittweisen Analyse
- `data/`: Rohdaten und vorverarbeitete Datensätze
- `results/`: Visualisierungen und Ergebnisse der Analyse

## Methodik
- **Datenvorverarbeitung**: Textreinigung, Entfernen von Stoppwörtern, Lemmatisierung
- **Vektorisierung**: TF-IDF und Word2Vec
- **Themenextraktion**: Latent Semantic Analysis (LSA)

## Benötigte Bibliotheken
- pandas
- ntlk
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

