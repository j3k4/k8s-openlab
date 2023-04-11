# k8s openlab

Das repo ist zu trainingszwecken erstell worden, um sich mit Kubernetes und einiges Applikationen und damit verbundenen Services sich auseinander zu setzen.

Die Kubernetes-Instanz wird auf Nodes ausgeführt, die in einer DMZ liegern, wodurch die Verwedungs-Möglichkeiten eingeschränkt sind.

## Infos zur Umgebung

Der Cluster läuft auf drei Nodes (1x Master, 2x Worker).

**Node Infos:**
- CPU: 8GHz
- RAM: 8GB
- Storage: 30GB
- OS: RedHat
- K8s: RKE2

## Idee

Die Idee ist es ein Cluster aufzubauen mit allen nötigen Applicationen um darauf dann weiter Applikationen testen zu können.

Die folgenden Services sind als Base Applikationen gedach:

| Apps | Beschreiebung |
| --- | --- |
| Longhorn | Verteilen von Daten von den einzelen Applikationen und als Standart Persistant Class |
| Prometheus | Sammeln von Daten und Metriken von dem Cluster und deren Services |
| Grafana | Grafisch aufbereitete Darstellung von Daten und Metriken |
| ArgoCD | Automatisierte Syncronisation mit diesem Repo |

