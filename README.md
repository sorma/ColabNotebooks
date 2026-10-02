# Bank Marketing

Analisi del dataset **Bank Marketing** finalizzata a prevedere l'adesione di un cliente a una campagna per la sottoscrizione di un deposito a termine.

Il progetto esplora e prepara i dati, quindi confronta modelli di classificazione basati su Decision Tree e Support Vector Machine (SVM), insieme a semplici baseline.

## Contenuto

- [`Copia di Bank-Marketing.ipynb`](./Copia%20di%20Bank-Marketing.ipynb): notebook principale con analisi esplorativa, feature engineering, addestramento e valutazione dei modelli.
- `requirements.txt`: dipendenze Python necessarie.

Il dataset viene scaricato durante l'esecuzione tramite `kagglehub` dal dataset Kaggle [`janiobachmann/bank-marketing-dataset`](https://www.kaggle.com/datasets/janiobachmann/bank-marketing-dataset); non viene quindi versionato nella repository.

## Avvio locale

È consigliato Python 3.10 o successivo.

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install -r requirements.txt
jupyter lab
```

Aprire quindi `Copia di Bank-Marketing.ipynb` ed eseguire le celle in ordine.

## Google Colab

Il notebook è compatibile con Google Colab. Se una dipendenza non fosse già disponibile nell'ambiente, installarla in una cella con:

```python
%pip install -r requirements.txt
```

## Note sulla riproducibilità

- Lo split tra training e test e i principali modelli usano `random_state=42`.
- Il download tramite Kaggle può richiedere autenticazione secondo le condizioni e la configurazione corrente di Kaggle.
- La ricerca degli iperparametri SVM può richiedere diversi minuti e utilizza tutti i core disponibili (`n_jobs=-1`).
- Il notebook conserva gli output prodotti nell'esecuzione originale; per questo il file ha dimensioni maggiori rispetto a un notebook senza output.

## Licenza

Non è stata ancora specificata una licenza per il codice. Prima di rendere pubblica la repository, scegliere una licenza adatta e verificare separatamente i termini d'uso del dataset.
