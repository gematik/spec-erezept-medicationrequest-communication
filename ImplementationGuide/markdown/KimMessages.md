
# Inhalt

- [Inhalt](#inhalt)
  - [Verwendung von KIM](#verwendung-von-kim)
  - [KIM Dienstkennungen](#kim-dienstkennungen)
  - [KIM Datenübertragung](#kim-datenübertragung)
  - [KIM Rezeptanforderung](#kim-rezeptanforderung)

## Verwendung von KIM

Die Übertragung der Daten bzw. der Anfrage erfolgt via KIM. Dabei sind vier Nachrichtentypen zu unterscheiden:

- Übermittlung der Rezeptanforderung (Anforderung)
- Übermittlung der Verordnung zu einer Rezeptanforderung  (Antwort)
- Übermittlung der Abgabeinformationen zu einer Rezeptanforderung (Abgabeinformationen)
- Stornierung/Ablehnung einer Rezeptanforderung (Stornierung)

## KIM Dienstkennungen

Dienstkennungen in KIM-Nachrichten kennzeichnen den transportierten Inhalt für das Empfangssystem. Diese erlauben damit eine Dunkelverarbeitung bei Nachrichtenempfang und ggfs. die vollautomatisierte Erstellung und den Versand einer Antwortnachricht.

|Anwendung                          |E-Rezept|
|:--------                          |:--------------------------------------|
|Verantwortlich                     |gematik                                |
|Anwendungsbeschreibung             |Rezeptanforderungsverfahren zur Übertragung relevanter Informationen zur Anforderung, Übertragung von Verschreibungen und resultierenden Abgabeinformationen|
|Dienstkennung & Kurzbeschreibung|**E-Rezept;Rezeptanforderung;V1.0** <br /> Nachrichten-Typ: Anfragedaten zur Anforderung einer E-Rezeptes<br /> Verwendung: Pflegeeinrichtungen, Vertragsärzte, Vertragszahnärzte, Krankenhäuser, Apotheken <br /><br /> **E-Rezept;Rezeptanforderung_Rezeptuebermittlung;V1.0** <br /> Nachrichten-Typ: Auf eine Rezeptanforderung beruhende elektronische Verordnung<br /> Verwendung: Pflegeeinrichtungen, Vertragsärzte, Vertragszahnärzte, Krankenhäuser, Apotheken <br /> <br /> **E-Rezept;Verordnung_Dispensierung;V1.0** <br /> Nachrichten-Typ: Abgabeinformationen zu einer Abgabe ausgelöst durch eine Verordnung und eine Abgabe<br /> Verwendung: Pflegeeinrichtungen, Apotheken <br /> <br /> **E-Rezept;Rezeptanforderung_Storno;V1.0** <br /> Nachrichten-Typ: Stornierung einer Rezeptanforderung<br /> Verwendung: Pflegeeinrichtungen, Vertragsärzte, Vertragszahnärzte, Krankenhäuser, Apotheken <br /> <br /> **E-Rezept;Rezeptanforderung_Ablehnung;V1.0** <br /> Nachrichten-Typ: Ablehnung einer Rezeptanforderung<br /> Verwendung: Pflegeeinrichtungen, Vertragsärzte, Vertragszahnärzte, Krankenhäuser, Apotheken|

## KIM Datenübertragung

Die FHIR-Datensätze in Anfrage- und Antwortnachrichten werden ausschließlich als Anhang in der KIM Nachricht übertragen.
