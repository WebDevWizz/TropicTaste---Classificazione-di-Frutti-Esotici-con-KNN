# TropicTaste: Classificazione di Frutti Esotici con KNN

## Descrizione del progetto

TropicTaste Inc., azienda leader nella distribuzione di frutti esotici, ha l'obiettivo di ottimizzare il processo di classificazione dei frutti attraverso l’utilizzo del **Machine Learning**. Questo progetto mira a sviluppare un modello di **classificazione automatizzata** in grado di predire il tipo di frutto in base a sue caratteristiche fisiche e qualitative.

## Obiettivi

- 🔄 Automatizzare la classificazione dei frutti
- ⚙️ Aumentare l’efficienza e la precisione del processo
- 📉 Ridurre gli errori umani e i costi
- 🛒 Ottimizzare la gestione dell'inventario
- 😊 Migliorare la soddisfazione dei clienti

---

## 📁 Dataset

Il dataset è composto da misurazioni numeriche sui frutti e contiene le seguenti variabili:

| Variabile            | Descrizione                                                  |
|----------------------|--------------------------------------------------------------|
| `Frutto`             | Tipo di frutto (target da predire)                          |
| `Peso (g)`           | Peso del frutto in grammi                                   |
| `Diametro medio (mm)`| Diametro medio del frutto in millimetri                    |
| `Lunghezza media (mm)`| Lunghezza media del frutto in millimetri                  |
| `Durezza buccia (1-10)`| Scala da 1 a 10 della durezza della buccia               |
| `Dolcezza (1-10)`    | Scala da 1 a 10 della dolcezza del frutto                  |

🔗 **Link al dataset**: [fruits.csv](https://proai-datasets.s3.eu-west-3.amazonaws.com/fruits.csv)

---

## 🧪 Tecniche Utilizzate

- 📊 **Analisi Esplorativa**: visualizzazione distribuzioni, correlazioni, outlier.
- 🧹 **Preprocessing**: gestione valori mancanti, normalizzazione delle feature.
- 🧠 **Modello K-Nearest Neighbors (KNN)**: algoritmo supervisionato per classificazione.
- 🔍 **Ottimizzazione Hyperparametri**: ricerca del valore ottimale di `k`.
- 📈 **Valutazione**: accuracy, matrice di confusione, validazione incrociata.
- 📉 **Visualizzazioni**: grafici di supporto all’analisi e interpretazione dei risultati.

---

## ⚙️ Requisiti

Per eseguire il progetto, installa le seguenti librerie Python:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

### 🚀 Come eseguire il notebook
1. Clona il repository:
```bash
git clone https://github.com/tuo-username/tropic-taste-fruits-classification.git
cd tropic-taste-fruits-classification
```
2. Avvia Jupyter Notebook o VS Code e apri ESAME_ALGORITMI_ML.ipynb
3. Esegui il notebook passo passo per riprodurre l'intera analisi.

---

### 📊 Risultati e Insight

- ✅ Il modello **K-Nearest Neighbors (KNN)** ha raggiunto una **buona accuratezza predittiva**, dimostrando l’efficacia dell’approccio per questo tipo di dati.  
  Le performance sono comunque **migliorabili** con:
  - una selezione più avanzata delle feature,
  - oppure l’utilizzo di algoritmi alternativi (es. Random Forest, SVM).

- 🍬 L’analisi esplorativa ha evidenziato una **forte correlazione tra la dolcezza del frutto e il tipo di frutto**, indicando che questa è una delle feature più significative per la classificazione.

- ⚖️ L'applicazione di tecniche di **normalizzazione** e la **scelta ottimale del parametro `k`** ha permesso di raggiungere un **buon compromesso tra bias e varianza**, migliorando la capacità di generalizzazione del modello.
