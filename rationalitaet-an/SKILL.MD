# Entscheidungsraster (Version 4.0)

## Gehärtetes Entscheidungsprotokoll

### 0. Meta-Regeln
1. **Status quo ist immer eine Option.**  
   X und Y sind nur Alternativen zum Status quo, nicht das ganze Entscheidungsuniversum.
2. **Sein und Sollen strikt trennen.**  
   Empirische Behauptungen brauchen Evidenz. Normative Prämissen brauchen explizite Wertbegründung.
3. **Keine Evidenz ohne Evidenzklasse.**  
   „Fakt“, „Plausibilität“, „Wahrscheinlichkeit“ reichen nicht. Jede Behauptung bekommt E0–E6.
4. **Unsicherheit wird klassifiziert, nicht verbalisiert.**  
   Nicht „mittel“, sondern U1–U4 plus Begründung.
5. **Beweislast ist asymmetrisch, aber begründet.**  
   Wer den Status quo ändert oder irreversible Risiken behauptet, trägt höhere Last.
6. **Entscheidungsregel vor dem Fazit festlegen.**  
   Erwartungsnutzen, Maximin, Minimax-Regret oder Vorsorgeprinzip. Nicht nachträglich wählen.
7. **Keine Gesamtnote ohne Gewichtung.**  
   Kriterien A, B, C … brauchen Gewichte und Schwellen.
8. **Jede normative Prämisse wird sichtbar gemacht.**  
   Normativ ≠ beliebig. Prüfbar auf Konsistenz, Universalisierbarkeit, Folgen und Wertkonflikte.

**Modus:** S = Kurzcheck (10 Zeilen) | M = Standard | L = Vollprüfung (+ Red Team, EVI, Audit)

---

### 1. Kernfrage
**Soll X, Y oder Status quo gewählt werden?**

Pflichtangaben:
- Entscheider: …
- Zeithorizont: …
- Betroffene: …
- Reversibilität: reversibel / schwer reversibel / irreversibel
- Entscheidungsregel: …

---

### 2. Kriterienkatalog
| Kriterium | Typ | Messgröße | Zielrichtung | Gewicht | Mindestevidenz | Reversibilität |
|---|---|---|---|---|---|---|
| A | empirisch | … | ↑/↓ | 0,4 | E3 | mittel |
| B | normativ | … | ↑/↓ | 0,6 | normativ konsistent | hoch |
| C | Risiko | … | ↓ | … | E4 | irreversibel |

**Regel:**  
Normative Kriterien sind nicht empirisch testbar, aber auf Konsistenz, Folgen, Universalisierbarkeit und Konfliktfreiheit prüfbar. Fehlt diese Prüfung, ist B nicht „normativ“, sondern bloß Behauptung.

---

### 3. Evidenz- und Unsicherheitsklassen
| Klasse | Bedeutung |
|---|---|
| E0 | reine Behauptung |
| E1 | Plausibilität |
| E2 | Mechanismus |
| E3 | Beobachtung / Korrelation |
| E4 | Quasi-experimentell |
| E5 | Experimentell / RCT |
| E6 | Systematische Synthese / Meta-Analyse |

| Klasse | Unsicherheit |
|---|---|
| U1 | niedrig |
| U2 | mittel |
| U3 | hoch |
| U4 | unbekannt / strukturell nicht messbar |

**Harte Schwellen:**
- Positive Effekte: mindestens **E3**.
- Eingriffe in irreversible Systeme: mindestens **E5** oder klare Vorsorge-Regel.
- Normative Kriterien: mindestens **explizite Wertprämisse + Konsistenzprüfung**.

---

### 4. Beweislastmatrix
| Behauptung | Träger | Schwelle | Status | Konsequenz bei Nichterfüllung |
|---|---|---|---|---|
| X hat positiven Effekt auf A | X | E3 | offen | X gilt als unbelegt, nicht als falsch |
| Y hat Nachteil auf A | Y | E3 | erfüllt | Y wird abgewertet |
| B ist vorrangig | wer B setzt | normative Begründung | offen | B darf nicht als „rational“ gelten |
| X ist alternativlos | X | E5 + Ausschluss Y | offen | falsches Dilemma |

**Wichtig:**  
Fehlende Evidenz ist **kein Beweis der Falschheit**. Sie senkt eine Option nur dann, wenn die Entscheidungsregel Evidenzschwellen vorsieht.

---

### 5. Annahmenregister
| Annahme | Typ | prüfbar | belegt | Falsifikator | Impact bei Falschheit |
|---|---|---|---|---|---|
| A | empirisch | ja | nein | … | hoch |
| B | normativ | konsistenzprüfbar | teilweise | … | mittel |
| C | empirisch | nein | nein | … | unbekannt |

**Regel:**  
Jede Annahme braucht einen Falsifikator. Ohne Falsifikator ist sie immunisiert und darf nicht als Entscheidungsgrundlage dienen.

---

### 6. Pro/Contra-Matrix (gehärtet)
| Option | Kriterium | Richtung | Evidenz | Unsicherheit | Normatives Gewicht | Reversibilität | Netto |
|---|---|---|---|---|---|---|---|
| X | A | + | E2 | U3 | mittel | mittel | schwach + |
| X | B | − | normativ | U2 | hoch | hoch | stark − |
| Y | A | − | E4 | U2 | mittel | mittel | mittel − |
| Y | B | + | normativ | U2 | hoch | hoch | stark + |

**Regel:**  
„Pro“ und „Contra“ werden nicht saldiert, bevor Gewicht, Evidenz und Reversibilität getrennt ausgewiesen sind.

---

### 7. Entscheidungsregel
**Regelauswahl:**
- Erwartungsnutzen → belastbare Wahrscheinlichkeiten
- Maximin → hohe Unsicherheit + irreversible Schäden
- Minimax-Regret → Irrtumskosten vergleichen
- Vorsorge → plausibel + irreversibel + evidenzarm
- Lexikographisch → ein Kriterium hat absoluten Vorrang

Wähle explizit eine Regel:

- **Erwartungsnutzen:**  
  \( U(X) = \sum w_i \cdot u_i(X) - \lambda \cdot R(X) \)  
  nur bei belastbaren Wahrscheinlichkeiten.

- **Maximin / Minimax-Regret:**  
  bei hoher Unsicherheit und irreversiblen Risiken.

- **Vorsorgeprinzip:**  
  wenn Schaden plausibel, irreversibel und Evidenz strukturell dünn ist.

- **Lexikographische Ordnung:**  
  wenn ein normatives Kriterium absoluten Vorrang hat.

**Ohne diese Regel ist „rational“ rhetorisch, nicht analytisch.**

---

### 8. Sensitivitätsanalyse
Pflichtfragen:
1. Welche Gewichtsänderung kippt X gegen Y?
2. Welche Evidenzstufe müsste X erreichen, um zu gewinnen?
3. Wie viele Annahmen müssen falsch sein, damit Y kippt?
4. Was ist der teuerste Irrtum: X wählen und falsch liegen oder Y wählen und falsch liegen?
5. Gibt es einen robusten Kern jenseits aller Unsicherheit?
6. **EVI:** Lohnt weitere Information? Was würde sie kippen?
7. **Bias-Check:** Status-quo, Confirmation, Sunk Cost, Anchoring, Authority.

---

### 9. Fehlercodes
| Code | Fehler |
|---|---|
| F1 | Appeal to Tradition / Popularity |
| F2 | Argumentum ad Ignorantiam |
| F3 | falsches Dilemma |
| F4 | naturalistischer Fehlschluss |
| F5 | Nirwana-Fallacy |
| F6 | Slippery Slope |
| F7 | Zirkelschluss |
| F8 | Strohmann |
| F9 | Whataboutism |

**Regel:**  
Jeder Fehlercode muss im Fazit neutralisiert werden. Sonst bleibt er als offene Schwachstelle markiert.

---

### 9b. Red Team
- Stärkstes Gegenargument:
- Steelman der Gegenposition:
- Welche Annahme muss falsch sein, damit die Präferenz kippt?

---

### 10. Fazit-Formel
**Unter Entscheidungsregel R, Gewichten \(w\), Evidenzstand E und Unsicherheit U ist Y gegenüber X vorläufig zu bevorzugen, weil …**

**Die Präferenz kippt, wenn:**
- X Evidenzstufe E… erreicht,
- B anders gewichtet wird,
- Risiko R(X) unter Schwelle … fällt,
- Annahme … falsch ist.

**Offene Unbekannte:**
- …
- …
- …

**Nächster Schritt / Update:** …

**Präzisere These:**
> „Unter der Annahme, dass B mit 0,6 und A mit 0,4 gewichtet wird, ist Y vorläufig rational, weil Xs positiver Effekt auf A unbelegt ist und Ys Nachteil auf A weniger irreversibel erscheint. Die These kippt, wenn X einen Effekt auf A oberhalb der Schwelle d nachweist oder wenn Ys Nachteil irreversibel ist.“

---

### 11. Qualitätsgate
- [ ] Status quo geprüft
- [ ] Sein/Sollen getrennt
- [ ] Evidenzklassen vergeben
- [ ] Beweislast begründet
- [ ] Gewichte explizit
- [ ] Entscheidungsregel begründet
- [ ] Normative Prämissen geprüft
- [ ] Red Team durchgeführt
- [ ] Falsifikatoren genannt
- [ ] Fazit konditional

---

**Kurz:**  
Das Raster ist gehärtet, wenn es drei Dinge erzwingt: **Evidenzklasse, Beweislast, Entscheidungsregel.** Ohne diese drei ist jedes „rational“ zu stark.
