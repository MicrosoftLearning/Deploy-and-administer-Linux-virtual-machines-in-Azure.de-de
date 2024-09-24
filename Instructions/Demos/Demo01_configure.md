---
demo:
  title: 'Demo 01: Konfigurieren eines virtuellen Azure Linux-Computers'
  module: 'Guided Project: Deploy and administer Linux virtual machines'
---

# Demo 01: Konfigurieren eines virtuellen Azure Linux-Computers

## Leistungsnachweisaufgaben

Verwenden Sie diese Demonstration, um diese Leistungsnachweisaufgaben zu überprüfen:
+ Erstellen einer virtuellen Linux-Maschine (Portal)
+ Konfigurieren eines Linux-VMs
+ Herstellen einer SSH-Verbindung mit einer Linux-VM  
+ Aktualisieren von Linux-VM-Betriebssystemen
+ Installieren und Ausführen einer Workloadabhängigkeit

## Ressourcenanforderungen

Diese Ressource kann vor oder während der Demonstration erstellt werden. 

+ Ressourcengruppe. 

## Referenzfolien (optional)

+ Plan für virtuelle Maschinen
+ Unterstützte Linux-Distributionen
+ VM-Größen
+ Azure-Ressourcen-Organisation
+ Azure-Administratortools

## Referenzschritte

Detaillierte Schritte finden Sie in diesen Links.

+ [Bereitstellen eines virtuellen Linux-Computers über das Azure-Portal](https://learn.microsoft.com/training/modules/provision-linux-virtual-machine-in-azure/2-provision-linux-virtual-machine-using-the-azure-portal)
+ [Schnellstart: Erstellen einer Linux-VM](https://learn.microsoft.com/azure/virtual-machines/linux/quick-create-portal?tabs=ubuntu)

## Diskussionspunkte

**Erstellen und Konfigurieren des virtuellen Computers**

1. Verwenden Sie das Portal, um eine Linux-VM zu erstellen. Besprechen Sie, wie in späteren Übungen die CLI- und Schnellstartvorlagen zum Erstellen von virtuellen Computern verwendet werden. 

1. Verwenden Sie den Link zum Portal, um die Linux **Bilder**-Auswahl zu überprüfen.  Identifizieren Sie die neueste Ubuntu-Verteilung.

1. Verwenden Sie den Link zum Portal, um die Auswahl der **Größe** zu überprüfen.  Erläutern Sie, wie Sie die CPU- und Arbeitsspeichereinstellungen skalieren können.

1. Besprechen Sie die Auswirkungen der Größenänderung. Die Größenänderung erfolgt in einer späteren Übung. 

1. Besprechen Sie die verschiedenen Möglichkeiten, sich mit einem virtuellen Computer unter Linux zu verbinden (öffentlicher SSH-Schlüssel und Kennwort).
   
1. Besprechen Sie die Bedeutung eingehender **Portregeln**. Insbesondere Port 22 für SSH und Port 80 für Nginx. 

1. Verwenden Sie die Registerkarte **Datenträger**, um darzustellen, wie ein Datenträger hinzugefügt werden würde. Das Hinzufügen eines Datenträgers erfolgt in einer späteren Übung. 
 
1. Verwenden Sie die Seite **Erweitert**, um darzustellen, wo eine Cloud-init-Datei bereitgestellt werden könnte.

1. In späteren Übungen verwenden Sie außerdem Vorlagen und die CLI, um virtuelle Computer zu installieren. 

**Zugreifen auf den virtuellen Computer und Installieren von Nginx**

1. Stellen Sie den virtuellen Computer bereit. Besprechen Sie die Validierungsphase und das Überwachen von Benachrichtigungen.

1. Öffnen Sie ein CMD-Fenster, und greifen Sie mit SSH auf den virtuellen Computer zu. Besprechen Sie das Format des SSH-Befehls und den Speicherort der Schlüsseldatei. 

1. Installieren Sie Nginx, und stellen Sie sicher, dass die Startseite angezeigt wird. 
