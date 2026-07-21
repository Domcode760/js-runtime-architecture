# js-runtime-architecture
Visuelle Deep-Dive-Architektur am Praxisbeispiel meiner Bankwebsite: Wie JavaScript von UTF-8-Dateibytes über V8-Kompilierung zu libuv-HTTP-Requests wird. [WIP]

# JS Runtime Architecture: Under the Hood [WIP]

Ein visuelles Deep-Dive-Projekt, das den genauen Weg von JavaScript-Quellcode von der Festplatte bis zur Ausführung in der Engine dokumentiert. 

Dieses Repository dient als begleitendes Projekt für meine **Bewerbung um eine Ausbildung zum Fachinformatiker für Anwendungsentwicklung**. 

---

## 🎯 Der Praxis-Kontext: Mein Bankwebsite-Projekt
Der eigentliche Antrieb für diese Architektur-Analyse ist ein konkretes Projekt, das ich aktuell entwickle: **Eine funktionale Bankwebsite (Full-Stack).** 

Um ein sicheres und performantes Banking-System zu bauen, reicht es nicht, nur Code zu schreiben – man muss verstehen, wie die Maschine dahinter arbeitet. Das finale Ziel dieses Diagramms ist es, den kompletten Lebenszyklus eines **HTTP-Requests** (z. B. einer Kontostandsabfrage oder Überweisung) visuell zu tracken:
1. **Frontend:** Der Klick des Nutzers im Browser.
2. **Netzwerk:** Der Transport der Datenpakete zum Server.
3. **Backend (Node.js/V8):** Wie der Server den Request annimmt, im Dateisystem/der Datenbank verarbeitet (via `libuv`) und die Server-Logik im V8 Call Stack ausführt.

---

## 📍 Aktueller Status: Work in Progress (WIP)
Das Diagramm befindet sich aktuell in der aktiven Entwicklung. Ich bereinige momentan redundante Phasen in der Kompilierungs-Pipeline (V8 AST) und bereite die Integration des HTTP-Request-Flows vor.
