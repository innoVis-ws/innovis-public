# Rechtliche Informationen

Stand: 19. September 2026

## Impressum

### Anbieter und Verantwortlicher

- **innoVis Web Solutions**
- Vertreten durch: Justin Jäger
- Steubenplatz 12
- 64293 Darmstadt
- Hessen, Deutschland
- E-Mail: contact@unfolded.tools
- Web: [unfolded.tools](https://unfolded.tools)
- GitHub: [github.com/jstnjx](https://github.com/jstnjx)

UC Remote ist eine unabhängig entwickelte Drittanbieter-App für Unfolded Circle Remote Two und Remote 3. Die App wird weder von Unfolded Circle ApS betrieben noch von Unfolded Circle ApS unterstützt, ist nicht mit Unfolded Circle ApS verbunden und wird nicht offiziell gebilligt.

Produktnamen, Marken und Logos Dritter sind Eigentum der jeweiligen Rechteinhaber. Ihre Nennung dient ausschließlich der Identifikation, Interoperabilität und Beschreibung der unterstützten Geräte und Dienste.

### Kontakt

Für rechtliche Hinweise, Datenschutzanfragen, Support und sonstige Anfragen: contact@unfolded.tools

---

## Datenschutzerklärung

### 1. Verantwortlicher

Verantwortlich für die Datenverarbeitung im Zusammenhang mit UC Remote ist:

- **innoVis Web Solutions**
- Vertreten durch: Justin Jäger
- Steubenplatz 12
- 64293 Darmstadt
- Hessen, Deutschland
- E-Mail: contact@unfolded.tools

### 2. Grundprinzip der App

Die native UC-Remote-App für iOS, iPadOS und Android arbeitet primär lokal. Sie verbindet sich direkt über das lokale Netzwerk mit einer vom Nutzer konfigurierten Unfolded Circle Remote Two oder Remote 3.

Remote-Aktivitäten, Entitäten, Befehle und Ressourcen werden bei der normalen Nutzung nicht über einen Server des App-Anbieters geleitet. Für die native App ist kein Benutzerkonto beim App-Anbieter erforderlich.

Die App enthält keine vom App-Anbieter eingebundene Werbung und keine Analyse-, Werbe- oder Tracking-SDKs.

### 3. Lokal auf dem Gerät gespeicherte Daten

Damit die vom Nutzer gewünschten Funktionen bereitgestellt werden können, speichert die App Informationen lokal auf dem verwendeten Gerät. Dazu können insbesondere gehören:

- Name und lokale Netzwerkadresse eingerichteter Remotes
- gewählte Authentifizierungsmethode
- Web-Configurator-PIN oder Core-API-Schlüssel, soweit vom Nutzer hinterlegt
- App-Einstellungen wie Sprache, Startansicht, Darstellung, Haptik und Ausrichtung
- Einstellungen für Aktivitäten und optionale Aktivitäts-Streams
- die zuletzt verwendete Einstellungsansicht
- lokal zwischengespeicherte Remote-Ressourcen wie Icons, Hintergründe, Senderlogos oder Sounds

Diese Daten werden in lokalem Browser-/WebView-Speicher wie IndexedDB und Local Storage abgelegt. Sie werden durch diese Speicherung nicht an den App-Anbieter übertragen.

Der Ressourcen-Cache behandelt gespeicherte Remote-Ressourcen nach 30 Tagen als veraltet. Daten können technisch bis zum Überschreiben, manuellen Löschen der entsprechenden Einstellungen/App-Daten oder bis zur Deinstallation der App auf dem Gerät verbleiben.

Die lokale Speicherung und der Zugriff auf diese Informationen erfolgen, soweit anwendbar, zur Bereitstellung der ausdrücklich gewünschten App-Funktionen. Für unbedingt erforderliche Speicherzugriffe gilt insbesondere § 25 Abs. 2 Nr. 2 TDDDG.

### 4. Kommunikation mit der Unfolded Circle Remote

Die App kann im lokalen Netzwerk nach kompatiblen Remotes per mDNS suchen. Nach der Einrichtung kommuniziert sie direkt mit der ausgewählten Remote über HTTP oder HTTPS sowie WebSocket oder WebSocket Secure.

Dabei können die vom Nutzer angeforderte Remote-Konfiguration, Aktivitäten, Entitäten, Medien- und Ressourceninformationen sowie Steuerbefehle zwischen dem Gerät und der Remote übertragen werden. Hinterlegte Zugangsdaten werden ausschließlich zur Authentifizierung gegenüber der konfigurierten Remote verwendet.

Bei lokalen oder privaten Netzwerkadressen erlaubt die App auch unverschlüsseltes HTTP. In diesem Fall ist die Übertragung innerhalb des lokalen Netzwerks nicht transportverschlüsselt. Für nicht lokale Ziele verlangt die native App HTTPS.

Diese direkte LAN-Kommunikation wird nicht über Infrastruktur des App-Anbieters vermittelt.

### 5. Native Systemfunktionen

Je nach Plattform und aktivierten Einstellungen kann UC Remote Gerätefunktionen wie Haptik, Bildschirmausrichtung, iPadOS Live Activities, Hintergrundaktualisierung und lokale Aktivitätsbenachrichtigungen verwenden.

Die hierfür benötigten Remote-Zustände werden von der App auf dem Gerät verarbeitet. Der App-Anbieter betreibt hierfür keinen eigenen Push-Benachrichtigungsdienst und erhält durch diese Funktionen keine Remote-Aktivitätsdaten.

Berechtigungen können über die Systemeinstellungen des jeweiligen Geräts verwaltet werden.

### 6. Abruf dieser rechtlichen Informationen über GitHub

Die rechtlichen Informationen werden erst beim Öffnen von „Rechtliches“ aus dem öffentlichen Repository `innoVis-ws/innovis-public` über `raw.githubusercontent.com` geladen.

Bei diesem Abruf wird technisch eine Verbindung zu GitHub hergestellt. Dabei können insbesondere IP-Adresse, Zeitpunkt des Abrufs, angeforderte URL sowie technische Angaben des Geräts oder der App an GitHub übermittelt und von GitHub verarbeitet werden. Der App-Anbieter erhält diese Verbindungsdaten nicht direkt.

Weitere Informationen zur Datenverarbeitung durch GitHub enthält die [GitHub-Datenschutzerklärung](https://docs.github.com/site-policy/privacy-policies/github-general-privacy-statement).

Wenn der Nutzer den Link „Quelle auf GitHub anzeigen“ öffnet, wird zusätzlich die GitHub-Webseite im Standardbrowser oder einer entsprechenden Systemansicht aufgerufen.

### 7. Rechtsgrundlagen

Soweit der App-Anbieter personenbezogene Daten tatsächlich erhält oder verarbeitet, erfolgt die Verarbeitung abhängig vom jeweiligen Vorgang insbesondere auf Grundlage von Art. 6 Abs. 1 lit. b DSGVO, sofern sie zur Erfüllung einer vom Nutzer angeforderten Leistung im Rahmen eines Vertragsverhältnisses erforderlich ist, oder Art. 6 Abs. 1 lit. f DSGVO aufgrund des berechtigten Interesses, die App sicher, funktionsfähig und nachvollziehbar bereitzustellen.

Die überwiegende Verarbeitung von Remote- und Einstellungsdaten findet jedoch ausschließlich lokal zwischen dem Gerät des Nutzers und dessen Remote statt und wird dem App-Anbieter nicht offengelegt.

### 8. Speicherdauer

Der App-Anbieter speichert bei der normalen Nutzung der nativen App keine zentrale Kopie der lokal konfigurierten Remote-Zugangsdaten, Remote-Aktivitäten oder Remote-Entitäten.

Auf dem Gerät gespeicherte Daten bleiben grundsätzlich erhalten, bis sie durch den Nutzer geändert oder entfernt, App-Daten gelöscht oder die App deinstalliert werden. Kurzlebige Laufzeitdaten können bereits beim Beenden der App oder der jeweiligen Ansicht entfallen.

Für Daten, die GitHub beim Abruf der rechtlichen Informationen verarbeitet, gelten die Speicher- und Löschregeln von GitHub.

### 9. Empfänger und Drittlandübermittlung

Bei der normalen direkten LAN-Nutzung werden Remote-Daten nicht an den App-Anbieter oder einen vom App-Anbieter beauftragten Cloud-Dienst übertragen.

Beim Abruf der rechtlichen Informationen ist GitHub der externe Empfänger der dabei entstehenden technischen Verbindungsdaten. GitHub kann Daten auch außerhalb der Europäischen Union beziehungsweise des Europäischen Wirtschaftsraums verarbeiten. Einzelheiten ergeben sich aus den Datenschutzinformationen von GitHub.

### 10. Rechte betroffener Personen

Soweit die Voraussetzungen der DSGVO vorliegen, bestehen insbesondere Rechte auf Auskunft, Berichtigung, Löschung, Einschränkung der Verarbeitung, Datenübertragbarkeit und Widerspruch sowie das Recht, eine erteilte Einwilligung mit Wirkung für die Zukunft zu widerrufen.

Datenschutzanfragen können an contact@unfolded.tools gerichtet werden.

Darüber hinaus besteht das Recht, sich bei einer zuständigen Datenschutzaufsichtsbehörde zu beschweren.

### 11. Änderungen

Diese Datenschutzerklärung kann angepasst werden, wenn sich Funktionen, Datenflüsse, eingesetzte Dienste oder rechtliche Anforderungen ändern. Die jeweils aktuelle Fassung wird über den in der App eingebauten Rechtliches-Dialog aus diesem öffentlichen Repository geladen.
