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

## 🧱 Architektur

- Interfaces zur Spezifikation der Saurier und Datenstruktur
- Baumstruktur besteht aus `EmptyTreeNode` und `NonEmptyTreeNode`
- Implementierte Saurierarten: z. B. **Tyrannosaurus Rex**, **Edmontosaurus**
- Fabriken: `TRexFactory`, `EdSFactory`
- Einstiegspunkt: `Application.java` (hier werden Szenarien ausgeführt)

## 🚀 Beispiel

```plaintext
#TREX
Dino1!42
Dino2!11
#EDS
Dino3!6
