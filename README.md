**NLP con Disaster Tweets** 🛰️🔥
Questo repository contiene un progetto di Natural Language Processing (NLP) focalizzato sulla classificazione di messaggi testuali provenienti da Twitter. L'obiettivo è determinare se un tweet annuncia un disastro reale (terremoti, incendi, alluvioni, ecc.) o se si tratta di un uso metaforico o non rilevante della parola.

Il progetto implementa una pipeline, dalla fase di esplorazione dei dati fino alla sottomissione dei risultati.

📋 **Panoramica del Progetto**
Il sistema è addestrato per risolvere il task della competizione Kaggle Natural Language Processing with Disaster Tweets.

**Tecniche Implementate:**
-*Integrazione Dataset:* Caricamento dei dati ufficiali e tecniche di Data Augmentation tramite l'unione con dataset esterni per migliorare la robustezza del modello.

-*Analisi Esplorativa (EDA):* Studio della distribuzione delle classi, lunghezza dei tweet, analisi delle keyword più frequenti e visualizzazione geografica delle location dichiarate.

-*Tokenizzazione avanzata:* Utilizzo del tokenizzatore cardiffnlp/twitter-roberta-base, ottimizzato specificamente per il linguaggio dei social media.

-*Cross-Validation:* Implementazione di un'architettura basata su Stratified K-Fold per garantire una valutazione stabile delle performance.

-*Ensembling:* Raccolta e combinazione delle predizioni di diversi fold per generare una submission finale ad alta accuratezza.

🛠️ **Tecnologie Utilizzate**
-Python

-Hugging Face Transformers (Modello: RoBERTa)

-PyTorch

-Pandas / NumPy (Manipolazione dati)

-Matplotlib / Seaborn (Data Visualization)

-Scikit-learn (Metriche e Cross-validation)

📂 **Struttura dei File**
Per eseguire correttamente il notebook, assicurati di avere i seguenti file nella cartella di lavoro:

-*train.csv:* Dataset di training ufficiale.

-*test.csv:* Dataset di test ufficiale.

-*socialmedia-disaster-tweets-DFE.csv:* Dataset esterno utilizzato per l'augmentation.

Bash
pip install transformers datasets evaluate contractions torch
Esegui il notebook:
Apri il file NLP_disaster_tweets_lucia_brando.ipynb in ambiente Jupyter o Google Colab.

📊 Risultati
Il modello sfrutta la potenza di Twitter-RoBERTa, un modello pre-addestrato su milioni di tweet, permettendo di catturare sfumature semantiche tipiche dello slang e della brevità di Twitter che i modelli tradizionali potrebbero ignorare.
