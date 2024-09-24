---
demo:
  title: 'Demo 02: Überwachen eines virtuellen Azure Linux-Computers'
  module: 'Guided Project: Deploy and administer Linux virtual machines'
---

# Demo 02: Überwachen eines virtuellen Azure Linux-Computers

## Leistungsnachweisaufgaben

+ Erstellen Sie einen virtuellen Computer (Schnellstartvorlage).
+ Konfigurieren von VM Insights
+ Eine Warnung erstellen.  
+ Identifizieren von Leistungsproblemen 
+ Ändern der Größe eines virtuellen Computers 

## Ressourcenanforderungen

+ Virtueller Computer mit Linux (erstellt mit einer benutzerdefinierten Vorlage)

## Referenzfolien 

+ Azure Resource Manager-Vorlagen
+ Die wichtigsten Funktionen von Azure Monitor
+ Azure Monitor-Komponenten
+ Metriken und Protokolle

  
## Referenzschritte

Detaillierte Schritte finden Sie in diesen Links.

+ [Bereitstellen einer einfachen Ubuntu Linux-VM](https://learn.microsoft.com/azure/virtual-machines/linux/quick-create-template)
+ [Aktivieren von VM Insights für den Azure Monitor-Agent](https://learn.microsoft.com/azure/azure-monitor/vm/vminsights-enable-portal#enable-vm-insights-for-azure-monitor-agent) 
+ [Tutorial: Erstellen einer Metrikwarnung für eine Azure-Ressource](https://learn.microsoft.com/azure/azure-monitor/alerts/alerts-create-metric-alert-rule)


## Referenzfolien (optional)

Verwenden Sie diese Folien für zusätzlichen Kontext.



## Diskussionspunkte

1. Verwenden Sie **Bereitstellen einer benutzerdefinierten Vorlage** für einen einfachen Linux Ubuntu-Computer. Auf diese Weise werden die Studierenden die VM in der Übung erstellen. Besprechen Sie die Verwendung von Vorlagen. 

1. Aktivieren Sie VM Insights. Überprüfen Sie, wie Sie eine Datensammlungsregel verwenden und wie Sie einen Log Analytics-Arbeitsbereich auswählen. 

1. Erstellen Sie eine Warnung auf der Grundlage von Metriken. Erstellen Sie zum Beispiel eine neue Warnungsregel, die auf der prozentualen CPU-Auslastung basiert.

1. Besprechen Sie die Verwendung von Aktionsgruppen und das Zuweisen einer Aktionsgruppe zur Warnung. 

1. Überprüfen Sie, wie Sie eine Warnung überwachen, wenn sie ausgelöst wird.

1. Schließen Sie mit dem Exportieren der Ressourcenvorlage ab. 
