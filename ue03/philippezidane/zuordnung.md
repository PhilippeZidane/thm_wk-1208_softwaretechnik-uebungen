# Anforderung oder Lösung? — Terminplaner für die THM

GitHub-Benutzername: philippezidane

## Funktionale Anforderung (FA)

- Studierende können einen freien Sprechstundentermin bei einer Lehrperson buchen.
- Vor jeder Buchung fragt die Komponente „Buchung“ bei der Komponente „Kalender“ an, ob der Termin noch frei ist.
- Sagt eine Lehrperson eine Sprechstunde ab, erhalten alle, die gebucht haben, eine Nachricht.
- Ein bereits gebuchter Termin kann kein zweites Mal gebucht werden.

## Qualitätsanforderung (QA)

- Termine werden in einer PostgreSQL-Datenbank gespeichert.
- Personenbezogene Daten werden nach den Vorgaben der EU-DSGVO verarbeitet.
- Jeder gebuchte Termin lässt sich als iCal-Datei herunterladen.
- Die Buchungsseite ist mit einem Screenreader vollständig bedienbar.
- Die API nimmt Anfragen als REST-Aufrufe entgegen und antwortet in JSON.

## Randbedingung (RB)

- Die Anmeldung erfolgt ausschließlich über das Hochschulkonto.
- Eine Buchung ist für Studierende in höchstens drei Schritten abgeschlossen.
- Auch zu Beginn der Prüfungsanmeldung, wenn bis zu 2.000 Personen zugleich buchen, zeigt das System eine Seite in weniger als zwei Sekunden an.
- Das System wird im Rechenzentrum der THM betrieben.
- Die erste Ausbaustufe geht zum Sommersemester 2027 in Betrieb.

## Keine Anforderung — Lösung (WIE)

- Über die API kann ein KI-Agent freie Termine abfragen und im Namen einer Person buchen.
- Ein Sekretariat sieht alle Prüfungstermine seines Fachbereichs auf einen Blick.

## Bei welchen Karten waren Sie unsicher — und was haben Sie abgewogen?

- **Über die API kann ein KI-Agent freie Termine abfragen und im Namen einer Person buchen.** (Keine Anforderung — Lösung (WIE)): …

<!-- zuordnung ue03-anforderung-oder-loesung: k01=fa k02=qa k03=rb k04=rb k05=fa k06=rb k07=fa k08=fa k09=qa k10=rb k11=qa k12=qa k13=qa k14=wie k15=rb k16=wie | unsicher: k16 -->
