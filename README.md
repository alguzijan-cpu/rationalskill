# Rationalität AN – Analyse-Modus für LLMs

Ein Custom-Instruction-/Skill-Prompt für Claude (und mit Anpassung auch andere LLMs), der ein strenges, strukturiertes Analyseschema für Entscheidungen und Argumente aktiviert: systematische Pro/Cons-Abwägung, explizite Beweislastzuweisung, Konfidenzausweisung und aktive Erkennung logischer Fehler – auch in der eigenen Argumentation.

## Warum dieser Skill

Die meisten "Anti-Sykophanz"-Prompts (siehe z. B. [Knotts 12 Custom Instructions](https://www.knott.cam/12-custom-instructions-for-chatgpt-claude-other-llms/)) fordern pauschal "widersprich mir, wenn ich falsch liege" oder "biete Gegenperspektiven". Das Problem: ohne Abbruchkriterium führt das leicht zu erzwungenem, pedantischem Widerspruch, auch wenn der Nutzer bereits recht hat.

Dieser Skill wurde genau dafür gehärtet – über mehrere Iterationen anhand echter Gesprächsverläufe:

- **v1**: Grundschema (Kernfrage, Pros/Cons, Fehleraufdeckung, Fazit)
- **v2**: Ergänzt um empirische Entscheidbarkeit, Beweislastzuweisung, Konfidenzskala
- **v2.1** (aktuell): Vier gezielte Korrekturen gegen beobachtetes Fehlverhalten:
  1. Beweislastregel auf Nutzen-/Maßnahmenbewertungen beschränkt (statt Universalhebel)
  2. Konzession explizit als legitimer Endpunkt definiert – "kein Fehler gefunden" ist kein Ausweichen
  3. Trennung zwischen fazitrelevanter Korrektur und rein kosmetischer Präzisierung
  4. Kennzeichnung von Mehrheits- vs. Minderheitspositionen bei Gegenperspektiven, um false balance zu vermeiden

## Verwendung

In den Custom Instructions / als Skill hinterlegen. Aktivierung durch Phrasen wie:
`"Rationalität AN"`, `"rationaler Modus"`, `"denk rational"`

Deaktivierung durch: `"Rationalität AUS"`, `"normaler Modus"`

Der Modus bleibt über mehrere Nachrichten hinweg aktiv, bis er explizit beendet wird.

## Beispiel

Siehe `SKILL.md`, Abschnitt "Beispiel-Antwort-Skelett", für das vollständige Ausgabeformat.

## Lizenz

MIT – frei nutzbar, veränderbar, weiterverbreitbar.

## Bekannte Grenzen

- Nur auf Deutsch getestet und formuliert; Übersetzung ins Englische erfordert eigene Anpassung der Trigger-Phrasen
- Konfidenzskala ist bewusst qualitativ (hoch/mittel/niedrig) statt numerisch – numerische Konfidenzwerte erzeugen bei LLMs erfahrungsgemäß Scheinpräzision (schwankende Werte bei identischer Wiederholung)
- Der Skill ersetzt keine fachliche/medizinische/rechtliche Beratung – er strukturiert Argumentation, prüft aber keine Fakten gegen externe Quellen
