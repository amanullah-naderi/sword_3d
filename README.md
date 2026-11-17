# Das Feuer der Finsternis – Das leuchtende Drachenschwert in der Gruselhölle

Ein 3D-Projekt im Rahmen des Moduls **Medienproduktion 3D** (Sommersemester 2024) an der **Fachhochschule Erfurt**.

---

## Projektübersicht & Konzept

Das Projekt inszeniert eine düstere, mystische Welt mit einem leuchtenden Drachenschwert im Zentrum. 
* **Szenerie & Architektur:** Das Schwert ruht auf einem stufenartig aufgebauten, benebelten Podest, das von einem Steinzaun ummauert ist. Umgeben wird das Zentrum von 4 großen Türmen, 5 kleinen leuchtenden Burgen (verbunden über Wege) sowie einer äußeren Steinmauer.
* **Atmosphäre:** Ein bedrohlicher roter Himmel, dunkle Farbgebung und gezielte Lichtakzente schaffen eine düstere, filmreife Kulisse.
* **Animation & Story:** Das Schwert „erwacht“ zum Leben, beginnt intensiv zu leuchten und löst durch seine Energie eine physikalische Kettenreaktion aus, bei der die umliegenden Steine und Mauern auseinanderplatzen.

---

## Verwendete Techniken & Workflow (Blender)

Das gesamte Projekt wurde in **Blender** umgesetzt und deckt die gesamte 3D-Pipeline ab:

* **Modeling:** 
  * Aufbau des Schwertes aus Grundformen (*Cube* für die Klinge; *Cylinder* für Parierstange, Heft und Knauf).
  * Einsatz von Modifikatoren wie *Subdivision Surface*, *Mirror* und *Simple Deform* für saubere Symmetrie und detaillierte Formen.
* **Physics & Animation:**
  * Gestaltung der Umgebung (*Plane* als Fundament, *Circle* für die Umgebung, modellierte Steinblöcke).
  * Einsatz von **Rigid Body Simulationen** (*Active* & *Passive*), um das Zerbersten der Steine rund um das Schwert-Podest realistisch zu animieren.
* **UV Editing:**
  * Sauberes Unwrapping mit **UDIM Tiles** (`1001`, `1002`), um hochauflösende Texturen verzerrungsfrei auf Klinge und Griff zu projizieren.
* **Shading & Lighting:**
  * Node-basiertes Material-Setup (*Principled BSDF*, *Texture Coordinate*, *Mapping*).
  * Einsatz von Emission-Shadern für das magische Leuchten des Schwertes sowie atmosphärischem World-Shading (roter Himmel).
* **Texture Paint:**
  * Handbemalte Details und Oberflächenstrukturen direkt auf dem 3D-Modell (inklusive individueller Signatur/Gravuren).

---

## Projektstruktur

```text
sword_3d/
├── Sword.blend                  # Haupt-Blender-Datei mit Modell, Szene, Rigging/Physics & Shadern
├── Textures/                    # Verwendete Texturen und Bild-Maps
│   ├── Black.jpg
│   └── Symbol.png
└── docs/                        # Projektdokumentation & Präsentation
    ├── 3D-Konzept.pdf           # Konzeptskizzen, Szenenaufbau und Ideenfindung
    └── 3D-Presentation.key      # Projektpräsentation (Modeling, Shading, UV & Animation)
