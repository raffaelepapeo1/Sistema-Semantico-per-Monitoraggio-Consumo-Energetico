
# Sistema Intelligente per l'Analisi dei Consumi Energetici

Questo progetto implementa un sistema di supporto basato su conoscenza (KBS) per l’analisi dei consumi energetici domestici. L’obiettivo è identificare automaticamente eventi critici di consumo combinando tecniche simboliche (ontologie OWL e ragionamento) e tecniche statistiche (machine learning supervisionato).

## Contenuti del progetto

- **Ontologia OWL DL**: rappresentazione semantica dei dispositivi, stanze, fasce orarie e consumi.
- **Reasoning con HermiT**: inferenza automatica di eventi critici tramite ragionamento simbolico.
- **Costruzione automatica di dataset**: dataset supervisionato generato dalla KB.
- **Modelli ML supervisionati**: Random Forest, SVM, Logistic Regression.
- **Valutazione predittiva**: accuracy, F1-score, AUC, matrici di confusione, feature importance.
- **Coerenza simbolico-subsymbolico**: verifica che i modelli ML apprendano schemi coerenti con le regole semantiche della KB.

## Struttura del repository

```
/ProgettoEnergia/
│
├── ontologia.owl                # Ontologia OWL del dominio energetico
├── reasoning.ipynb             # Notebook con ragionamento e generazione dataset
├── machine_learning.ipynb      # Notebook con addestramento modelli e valutazione
├── grafici/                    # Immagini di ROC, confusion matrix, feature importance
└── README.md                   # Questo file
```

## Requisiti

- Python >= 3.9
- Librerie:
  - `owlready2`
  - `scikit-learn`
  - `matplotlib`
  - `pandas`
  - `numpy`

## Esecuzione

1. Apri `reasoning.ipynb` per generare il dataset da ontologia.
2. Apri `machine_learning.ipynb` per addestrare e valutare i modelli.
3. I risultati delle valutazioni sono salvati in `grafici/`.

## Autore

Progetto realizzato per il corso di **Ingegneria della Conoscenza** – Università degli studi di Bari Aldo Moro.
