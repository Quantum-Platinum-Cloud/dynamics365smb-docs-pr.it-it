---
title: 'Come esportare i report di transazioni IVA [IT]'
description: 'Il seguente argomento spiega come esportare i report di transazioni IVA. Dopo la creazione di un report, è possibile rilasciarlo e quindi esportarlo per le autorità.'
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: null
ms.date: 06/18/2021
ms.author: edupont
---
# <a name="export-vat-transactions-reports-in-the-italian-version" />Esportare i report di transazioni IVA nella versione italiana
Dopo la creazione di un report, è possibile rilasciarlo e quindi esportarlo per le autorità. Per modificare il report, assicurarsi che la casella di controllo Modifica report inviati sia attivata nella pagina Setup report IVA. Se non lo è, per modificare il report quando si desidera correggere un errore, sarà necessario creare un nuovo report, aggiungere il report con l'errore al numero di report originale e quindi creare un report correttivo. Per ulteriori informazioni, vedere [Correggere i report di transazioni IVA](how-to-correct-vat-transactions-reports.md).  

È possibile modificare le righe e i campi solo quando lo stato del documento è Aperto. Quando lo stato è Rilasciato, solo il numero di carico è modificabile. Quando lo stato è Inviato, tutti i campi sono bloccati.  

## <a name="to-export-and-submit-a-vat-transaction-report" />Per esportare e inviare un report di transazioni IVA

1.  Scegli l'icona a forma di ![lampadina che consente di aprire la funzionalità delle informazioni.](../../media/ui-search/search_small.png "Informazioni sull'operazione che si desidera eseguire") immetti **Report IVA**, quindi scegli il collegamento correlato.  
2.  selezionare un report esistente o crearne uno nuovo.  

    - Selezionare il report IVA pertinente dall'elenco, quindi scegliere l'azione **Modifica**.  
    - Scegliere l'azione **Nuovo** e creare un nuovo report. Per ulteriori informazioni, vedere [Creare report elettronici di transazioni IVA](how-to-create-electronic-vat-transactions-reports.md).  

3.  Esaminare i dettagli della transazione. Per evitare che una riga venga dichiarata all'autorità fiscale, nella riga, deselezionare la casella di controllo **Elementi inclusi in report**. Per visualizzare i movimenti IVA su cui la riga è basata, scegliere il pulsante di drill-down nel campo **Importo**.

    > [!NOTE]  
    >  È possibile creare un report vuoto, ovvero un report senza righe, nel caso in cui non vi siano transazioni.  

4.  Scegliere l'azione **Rilascia**. Nel campo **Stato** viene visualizzato Rilasciato.  

    [!INCLUDE[prod_short](../../includes/prod_short.md)] verifica che il report IVA è valido e pronto per l'invio. Se la convalida ha esito negativo, gli errori vengono visualizzati nella pagina **Log errori report IVA** per consentire di apportare le modifiche appropriate.  

    Un report IVA rilasciato non può essere modificato. Se si deve modificare il report dopo averlo rilasciato, è necessario innanzitutto riaprirlo. Scegliere l'azione **Riapri**.  

5.  Scegliere l'azione **Esporta**. Il processo batch **Esporta transazioni IVA** viene aperto.  
6.  Selezionare la casella di controllo **Esportazione dettagliata**, in base alle proprie esigenze. Il campo determina se esportare i dati in formato dettagliato o aggregato. Se aggregato, le righe vengono ulteriormente raggruppate per numero di partita VAT o codice fiscale.  
7.  Scegliere il pulsante **OK**.

    Il report IVA viene esportato come file .CCF. È ora possibile inviare il report alle autorità fiscali utilizzando lo strumento dall'agenzia delle entrate italiana. Utilizzare le indicazioni fornite dall'autorità. Per ulteriori informazioni, vedere l'[agenzia delle entrate italiana](https://go.microsoft.com/fwlink/?LinkID=206524).  

    Una volta ricevuta una risposta dalle autorità fiscali, è necessario aggiornare il report IVA.  

8.  Nella Scheda dettaglio **Generale** nel campo **Nr. ricevuta ufficio fiscale** specificare il numero di carico ricevuto dalle autorità fiscali. Nel campo **Numero protocollo di invio - seconda parte**, specificare il numero di documento che si riceve.  
9. Scegliere l'azione **Contrassegna come inviato** per completare il report. Il valore del campo **Stato** diventa Inviato.  

    > [!NOTE]  
    >  È possibile modificare un report con lo stato Inviato solo se è stata selezionata la casella di controllo **Modifica report inviati** nella pagina **Setup report IVA**.  

## <a name="see-also" />Vedere anche
[Correggere i report di transazioni IVA](how-to-correct-vat-transactions-reports.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
