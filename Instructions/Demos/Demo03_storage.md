---
demo:
  title: 'Demo 03: Zugreifen auf Speicher für einen virtuellen Azure Linux-Computer'
  module: 'Guided Project: Deploy and administer Linux virtual machines'
---

# Demo 03: Zugreifen auf Speicher für einen virtuellen Azure Linux-Computer

## Leistungsnachweisaufgaben

+ Erstellen eines virtuellen Computers (CLI)
+ Hinzufügen von Datenträgern für virtuelle Computer und Konfigurieren von Partitionen 
+ Einbinden einer SMB-Azure-Dateifreigabe auf einer Linux-VM
+ Zuweisen einer verwalteten Identität auf einer Linux-VM 
+ Zuweisen von Azure-Rollen 
+ Datenübertragung von und zu einer Linux-VM mithilfe von AzCopy 

## Ressourcenanforderungen

Diese Ressourcen können vor oder während der Demonstration erstellt werden. 
+ Resource group
+ Linux VM.
+ Speicherkonto mit Dateifreigabe und Blob-Container.
+ Hochgeladene Dateien, die zum Testen verwendet werden sollen.
+ Verwaltete Identität. 

## Referenzschritte

Detaillierte Schritte finden Sie in diesen Links.

+ [Schnellstart: Erstellen eines virtuellen Linux-Computers mit der Azure CLI auf Azure](https://learn.microsoft.com/en-us/azure/virtual-machines/linux/quick-create-cli)
+ [Anfügen eines Datenträgers an einen virtuellen Linux-Computer](https://learn.microsoft.com/azure/virtual-machines/linux/attach-disk-portal)
+ [Erstellen einer SMB-Dateifreigabe](https://learn.microsoft.com/azure/storage/files/storage-how-to-create-file-share?tabs=azure-portal)
+ [Erste Schritte mit AzCopy](https://learn.microsoft.com/azure/storage/common/storage-use-azcopy-v10)


## Referenzfolien

Verwenden Sie diese Folien für zusätzlichen Kontext. 
+ Speicherkonten
+ Blobcontainer und Dateien
+ Dateien im Vergleich zu Blobs
+ Verwaltete Identitäten
+ Rollenbasierte Zugriffssteuerung

## Diskussionspunkte

**Erstellen eines virtuellen Computers mit CLI** – Referenz #1

>Sie können eine vorhandene VM (virtueller Computer) verwenden, anstatt eine neue zu erstellen.

1. Zugreifen auf die Cloud Shell.

1. Erstellen Sie den virtuellen Computer mit CLI. Weisen Sie darauf hin, dass dies die dritte Möglichkeit ist, die Studierenden zur Erstellung von VMs zur Verfügung steht.
   
**Hinzufügen eines Datenträgers zu einem virtuellen Linux-Computer** – Referenz #2

1. Überprüfen Sie, wie Sie mithilfe des Portals einem virtuellen Computer einen Datenträger hinzufügen. Schüler/Studenten verwenden CLI in der Übung.

1. Stellen Sie eine Verbindung zum virtuellen Computer her und verwenden Sie `lsblk`, um die Datenträger aufzulisten. Beachten Sie die Datenträgergröße und dass der Datenträger nicht eingebunden ist.

1. Bereiten Sie den Datenträger mit `parted` und `partprobe` vor. Verwenden Sie den Code im Referenzlink.

1. Verbinden Sie den Datenträger und verwenden Sie `df`, um den Bereitstellungspunkt aufzulisten. 

**Zugreifen auf eine SMB-Dateifreigabe vom virtuellen Computer** – Referenz #3 und Anweisungen für das Student Lab

1. Suchen Sie das Speicherkonto und besprechen Sie Dateifreigaben.

1. Weisen Sie dem virtuellen Computer eine verwaltete Identität zu. Die Identität sollte über Zugriff auf das Speicherkonto verfügen.

1. Kopieren Sie das Portalskript, um von einem virtuellen Linux-Computer aus auf die Dateifreigabe zuzugreifen.

1. Stellen Sie eine Verbindung mit dem virtuellen Computer her, und erstellen Sie eine Datei mit dem Skript. Sie können den vi-Editor verwenden.

1. Führen Sie das Skript aus, und stellen Sie die Dateifreigabe bereit. 

**Verwenden Sie AzCopy, um eine Blobdatei auf das Datenlaufwerk zu kopieren** – Anleitungen zu Referenz #4 und Student Lab.

1. Fügen Sie dem virtuellen Computer die Rolle „Mitwirkender an Storage-Blobdaten“ hinzu. Überprüfen Sie andere Blobrollen. 

1. Verbinden Sie sich mit dem virtuellen Computer und installieren Sie AzCopy. Überprüfen Sie andere Tools, die zum Übertragen von Dateien verwendet werden können. 

1. Verwenden Sie AzCopy, um eine Datei vom Blob Storage auf das Datenlaufwerk zu übertragen. Sie können eine Datei auch wieder in den Blob Storage übertragen.  
