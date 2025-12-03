Sentimentanalyse von Amazon-Rezensionen (IU Projektarbeit NLP)

Dieses Repository enthält den vollständigen Code sowie alle relevanten Ergebnisse der Projektarbeit „Sentimentanalyse von Produktrezensionen“ im Rahmen des Moduls DLBAIPNLP01_D an der IU Internationalen Hochschule.

Ziel des Projekts ist die Entwicklung eines Modells, das Amazon-Rezensionen anhand ihres Textinhalts automatisch einer Sternebewertung (1–5) zuordnet.

Inhalt des Projekts

Das Repository umfasst:

Jupyter Notebook (notebook.ipynb) Vollständiger Workflow:

Laden & Vorbereiten der Daten

Bereinigung

TF-IDF-Vektorisierung

Training des Klassifikators

Bewertungs- und Verwirrungsmatrix

Ordner results/ Enthält:

sentiment_model.joblib (trainiertes Modell)

tfidf_vectorizer.joblib (TF-IDF-Vektorisierer)

accuracy.txt (Modellgenauigkeit)

confusion_matrix_rating.png (normierte Matrix)

Ordnerdaten/ Aus rechtlichen Gründen sind keine Original-Amazon-Daten enthalten. Stattdessen liegt eine Datei README.txt, die dies erklärt.

Wie führe ich das Projekt aus? 1️ Repository klonen git clone https://github.com/ciliooo/sentiment-nlp-project cd sentiment-nlp-project

2️Virtuelle Umgebung erstellen python -m venv venv

3️Virtuelle Umgebung aktivieren

Windows:

venv\Scripts\activate

4 Abhängigkeiten installieren pip install -r require.txt

5️ Notebook starten Jupiter Notebook

Ergebnisse

Modell: Logistische Regression (multinomial)

Vektorisierung: TF-IDF (max_features=50.000, Unigram + Bigram)

Genauigkeit: 73,45 %

Confusion-Matrix: → siehe results/confusion_matrix.png

Das Modell erkennt besonders gut:

1-Stern-Bewertung

5-Sterne-Bewertung

Mittlere Bewertungen (2–4 Sterne) sind sprachlich unterschiedlich zu unterscheiden.

Datenhinweis

Sie können über folgende Quelle heruntergeladen werden:

McAuley Lab (2023): https://amazon-reviews-2023.github.io/

Lizenz & Nutzung

Dieses Projekt wurde im Rahmen einer IU-Projektarbeit erstellt. Die Nutzung des Codes ist für Lernzwecke erlaubt.
