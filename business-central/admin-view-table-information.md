---
title: Visualizzare Informazioni tabella
description: Informazioni su come visualizzare le informazioni sulle tabelle di database in Business Central.
author: jswymer
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.form: 8700
ms.date: 08/23/2022
ms.author: jswymer
---

# <a name="viewing-table-information" />Visualizzazione di Informazioni tabella

La pagina **8700 Informazioni sulla tabella** fornisce informazioni sul numero di record in tutte le tabelle di sistema e aziendali in [!INCLUDE[prod_short](includes/prod_short.md)] e quanti dati contiene ciascuna tabella.

Queste informazioni sono utili per la risoluzione dei problemi di prestazioni, perché consente di vedere la distribuzione delle dimensioni dei dati tra le tabelle.

## <a name="viewing-table-information" />Visualizzazione di Informazioni tabella

Per aprire questa pagina, seleziona l'icona ![Cerca pagina o report](media/ui-search/search_small.png "Icona Cerca pagina o report") immetti **Informazioni tabella**, quindi scegli il collegamento correlato.

La tabella seguente descrive le informazioni fornite per ciascuna tabella:

|Colonna|Descrizione|
|------|-----------|
|Nome società|Nome della società, se presente, a cui appartiene la tabella.|
|Nome tabella|Nome della tabella.|
|Nr. tabella|L'ID della tabella.|
|Nr. di record|Il numero totale di record archiviati nella tabella.|
|Dim. record|La dimensione media del record in KB/record. Il valore viene calcolato utilizzando la seguente formula: 1024 (Dimensione)/(N. di record). |
|Dimensioni (KB)|Quantità totale di spazio occupato dalla tabella nel database. Il valore è la somma dei valori nei campi Dimensione dati e Dimensione indice.|
|Dimensioni dati (KB)|Quantità di spazio occupato dai dati della tabella nel database.|
|Dimensioni indice (KB)|Quantità di spazio occupato dagli indici (chiavi) della tabella nel database.|
|Compressione|Il tipo di compressione, **Riga**, **Pagina**, o **Nessuno** che viene applicato alla tabella nel database. Per ulteriori informazioni, vedi [Compressione dei dati](/sql/relational-databases/data-compression/data-compression?).|

> [!NOTE]
> Se elimini i dati in una tabella, [!INCLUDE[prod_short](includes/prod_short.md)] avvia diversi processi dietro le quinte per assicurarsi che tutto venga eliminato nel database. I valori nella pagina Informazioni tabella non verranno aggiornati fino al completamento di tali processi, operazione che può richiedere del tempo. La quantità di tempo che dovrai aspettare può variare a seconda delle dimensioni del tuo database.

## <a name="see-also" />Vedi anche

[Controllo di pagine](across-inspect-page.md)  
[Articoli sulle prestazioni per gli sviluppatori](/dynamics365/business-central/dev-itpro/performance/performance-developer)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
