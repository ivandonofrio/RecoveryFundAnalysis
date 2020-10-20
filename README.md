# Recovery Fund analysis con BERT e Transformer

Un metodo alternativo per codificare e ed effettuare cluster analysis di brevi testi grazie all'utilizzo dei **Transformer**. In particolare mostrerò come sfruttare un'implementazione di **BERT** pre-addestrata sulla lingua italiana per tradurre l'informazione semantica in forma vettoriale e utilizzare quest'ultima come input per algoritmi di clustering gerarchico.

A tale scopo farò riferimento a un case study nel quale ho applicato il metodo in questione sulla lista dei progetti proposti per il **Recovery Fund** dal Governo Italiano.

## Intuizioni e punti salienti

I concetti principali che riassumono questo lavoro sono i seguenti:

* BERT è in grado di generare un language model e di **codificare l'informazione semantica** grazie all'utilizzo del meccanismo di attenzione e dei Transformer.

* Utilizzare una architettura pre-addestrata di BERT sulla lingua italiana consente di effettuare una codifica numerica e vettoriale dei testi. Tale rappresentazione riassume l'informazione semantica contenuta in essi utilizzando la conoscenza pregressa derivante dal pre-addestramento della rete. Per tali ragioni è possibile definire BERT un encoder, in grado di codificare il testo in forma per altri task. 

* Una volta ottenuta una rappresentazione numerica del testo è possibile utilizzare strumenti matematici per manipolare tali vettori. Più specificamente, è possibile utilizzare algoritmi di **clustering** che utilizzano metriche per quantificare la similarità tra due vettori e, di conseguenza, due testi.

## Riprodurre l'esperimento

Il seguente [Python Notebook](https://colab.research.google.com/drive/1eN8WMNscb98PIAmFmfu2UFTxUrOD4jcn?usp=sharing) hostato su Google Colab consente di riprodurre l'esperimento ed, eventualmente, estenderlo a piacere in base alle necessità.

## Riferimenti

Il seguente [articolo](https://www.ivandonofrio.it/post/topic-extraction-e-clustering-con-bert) pubblicato sul mio blog personale racconta in maniera informale le metodologie utilizzate durante l'esperimento e altri dettagli non riportati esplicitamente in questa repository.