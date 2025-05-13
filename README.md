# 🦖 DinoCorp – Dinosaurier-Park-Management-Simulation (Java)

Dieses Java-Projekt bildet das Backend einer Dinosaurier-Management-Simulation ab. Ziel ist die modellhafte Umsetzung einer Infrastruktur zur Erzeugung, Speicherung und Verwaltung virtueller Dinosaurier innerhalb eines Dino-Freizeitparks.

## 🌍 Domäne

Das Projekt spielt in der Welt eines Freizeitparks mit lebenden Dinosauriern. Als Teil eines Simulationssystems werden verschiedene Spezies von Dinosauriern erzeugt und in einer Datenstruktur gespeichert, die schnellen Zugriff auf einzelne Tiere erlaubt. Die Basis bildet ein binärer Suchbaum, über den alle registrierten Saurier verwaltet werden.

## ⚙️ Funktionalität

- **Dynamisch gebundener binärer Suchbaum** zur Verwaltung der Dinosaurierpopulation
- **Erzeugung von Sauriern** über speziesabhängige **Fabriken**, die über ein einfaches Skript aktiviert werden
- Unterstützung mehrerer Spezies durch **Factory Method** und **Abstract Factory Pattern**
- **Skripting-System** zur Steuerung des Erzeugungsprozesses:
  - `#TREX` aktiviert z. B. eine Brutstätte für Tyrannosaurus Rex
  - `"Daisy!8"` erzeugt z. B. einen Dino namens *Daisy* mit DNA-Code `8` in der aktiven Fabrik
- Speicherung aller erzeugten Dinos im Suchbaum für spätere Verarbeitung

## 🚀 Beispiel

```plaintext
#TREX
Mom!200
Tick!456
Trick!123
Track!7
#EDMONTOSAURUS
Donald!1
Daisy!8
