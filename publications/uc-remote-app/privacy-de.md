# Datenschutzerklärung für UC Remote

Stand: 30. September 2026

## 1. Verantwortlicher

Verantwortlich für die Datenverarbeitung im Zusammenhang mit UC Remote ist:

- **innoVis Web Solutions**
- Vertreten durch: Justin Jäger
- Steubenplatz 12
- 64293 Darmstadt
- Hessen, Deutschland
- E-Mail: contact@unfolded.tools
- Web: [unfolded.tools](https://unfolded.tools)

UC Remote ist eine unabhängig entwickelte Drittanbieter-App für Unfolded Circle Remote Two und Remote 3. Die App wird weder von Unfolded Circle ApS betrieben noch unterstützt, ist nicht mit Unfolded Circle ApS verbunden und wird nicht offiziell gebilligt.

## 2. Grundprinzip der App

UC Remote ist darauf ausgelegt, primär lokal zu arbeiten. Die App verbindet sich direkt mit einer vom Nutzer konfigurierten Remote Two oder Remote 3, üblicherweise über das lokale Netzwerk.

Bei der normalen Steuerung werden Remote-Aktivitäten, Entitäten, Befehle, Medieninformationen und Ressourcen nicht über einen Server von innoVis Web Solutions geleitet. Für die native App ist kein Benutzerkonto beim App-Anbieter erforderlich.

Die App enthält keine vom App-Anbieter eingebundene Werbung und keine Analyse-, Werbe- oder Tracking-SDKs.

## 3. Lokal auf dem Gerät gespeicherte Daten

Damit die vom Nutzer gewünschten Funktionen bereitgestellt werden können, speichert UC Remote Informationen lokal auf dem Gerät. Dazu können insbesondere gehören:

- Name und Netzwerkadresse eingerichteter Remotes
- gewählte Authentifizierungsmethode
- Web-Configurator-PIN oder Core-API-Schlüssel, soweit vom Nutzer hinterlegt
- App-Einstellungen wie Sprache, Startansicht, Interface-Optionen, Haptik, Ausrichtung und Bewegungseinstellungen
- Dashboard- und Aktivitätsdarstellung
- Tastaturkonfiguration
- Konfiguration von Aktivitäts-Streams und zugehörige Darstellungsoptionen
- zuletzt ausgewählter Einstellungsbereich und weiterer lokaler UI-Zustand
- lokal zwischengespeicherte Remote-Ressourcen wie Icons, Hintergründe, Senderlogos, Sounds, Cover oder Stream-Vorschaubilder

Diese Informationen werden je nach Funktion in App-, Browser- oder WebView-Speichern wie IndexedDB, Local Storage, gemeinsamem App-Group-Speicher oder nativen Einstellungen gespeichert. Durch die lokale Speicherung allein werden diese Informationen nicht an den App-Anbieter übertragen.

Zwischengespeicherte Remote-Ressourcen können auf dem Gerät verbleiben, bis sie ersetzt, manuell gelöscht, die entsprechenden App-Daten entfernt oder die App deinstalliert wird.

## 4. iCloud-Konfigurationssynchronisierung auf Apple-Geräten

Auf unterstützten iOS- und iPadOS-Geräten verwendet UC Remote **Apple iCloud Key-Value Storage**, um ausgewählte App-Konfigurationen zwischen Geräten zu synchronisieren, die mit demselben iCloud-Account angemeldet sind, sofern iCloud für die App verfügbar ist.

Synchronisiert werden können insbesondere:

- Interface- und Geräteeinstellungen
- Dashboard-Layouts und Dashboard-Seiteneinstellungen
- Darstellungsoptionen für Aktivitätsseiten
- Tastaturkonfiguration
- Konfiguration von Aktivitäts-Streams und zugehörige Darstellungsoptionen
- eingeklappte Profilgruppen und vergleichbare UI-Einstellungen

Remote-bezogene Einstellungsschlüssel werden über die normalisierte Remote-URL der konfigurierten Remote zugeordnet. Dadurch können entsprechende Remote-Konfigurationen auf mehreren Geräten erkannt werden, auch wenn die App lokal unterschiedliche interne Kennungen vergibt.

Der iCloud-Synchronisierungspayload **enthält weder die gespeicherte Remote-Liste noch Zugangsdaten zur Remote**. Insbesondere werden Web-Configurator-PINs, Core-API-Schlüssel und andere zur Authentifizierung gegenüber einer Remote verwendete Zugangsdaten von UC Remote nicht in den iCloud-Konfigurationspayload aufgenommen. Eine Remote muss deshalb auf einem weiteren Gerät weiterhin separat gekoppelt oder eingerichtet sein, bevor Remote-spezifische synchronisierte Einstellungen dort angewendet werden können.

Die Konfiguration von Aktivitäts-Streams kann URLs oder andere vom Nutzer eingegebene Einstellungswerte enthalten. Nutzer sollten keine geheimen Zugangsdaten in Stream-URLs oder anderen synchronisierten Einstellungsfeldern hinterlegen, sofern diese Werte nicht in ihrem persönlichen iCloud-Account gespeichert werden sollen.

iCloud wird von Apple betrieben. Die synchronisierten Daten werden über die Apple-/iCloud-Infrastruktur des Nutzers gespeichert und übertragen. innoVis Web Solutions betreibt den iCloud-Dienst nicht und erhält über die App keine Kopie dieser synchronisierten Konfiguration. Für die Datenverarbeitung durch Apple gelten die jeweils anwendbaren Datenschutzinformationen und iCloud-Bedingungen von Apple.

Weitere Informationen enthält die [Datenschutzrichtlinie von Apple](https://www.apple.com/legal/privacy/).

## 5. Kommunikation mit der Unfolded Circle Remote

UC Remote kann kompatible Remotes im lokalen Netzwerk per mDNS erkennen. Nach der Einrichtung kommuniziert die App direkt mit der ausgewählten Remote über HTTP oder HTTPS sowie WebSocket oder WebSocket Secure.

Abhängig von den verwendeten Funktionen können Remote-Konfiguration, Aktivitäten, Entitäten, Medien- und Ressourceninformationen sowie vom Nutzer ausgelöste Steuerbefehle zwischen Gerät und Remote übertragen werden. Hinterlegte Remote-Zugangsdaten werden zur Authentifizierung gegenüber der konfigurierten Remote verwendet.

Bei lokalen oder privaten Netzwerkadressen kann die App auch unverschlüsseltes HTTP zulassen. In diesem Fall ist die Übertragung innerhalb des lokalen Netzwerks nicht transportverschlüsselt. Für nicht lokale Ziele verlangt die native App HTTPS.

Diese direkte Kommunikation mit der Remote wird nicht über Infrastruktur von innoVis Web Solutions vermittelt.

## 6. Native Systemfunktionen

Je nach Plattform und aktivierten Einstellungen kann UC Remote Systemfunktionen wie Haptik, Steuerung der Bildschirmausrichtung, Widgets, Live Activities, Hintergrundaktualisierung und lokale Aktivitätsbenachrichtigungen verwenden.

Für diese Funktionen erforderliche Remote-Zustände werden von der App auf dem Gerät und, soweit für Apple-Plattformfunktionen erforderlich, im gemeinsamen lokalen App-Group-Container verarbeitet. Der App-Anbieter betreibt dafür keinen eigenen Push-Benachrichtigungs- oder Remote-State-Relay-Dienst.

Berechtigungen können über die Systemeinstellungen des jeweiligen Geräts verwaltet werden.

## 7. Diagnose und Support

UC Remote kann lokale Diagnoseinformationen und ein App-Protokoll zur Fehleranalyse der lokalen Verbindung und des App-Zustands anzeigen. Ein Diagnoseexport wird vom Nutzer ausdrücklich ausgelöst. Die App lädt exportierte Diagnosedaten nicht automatisch zum App-Anbieter hoch.

Wenn der Nutzer exportierte Diagnosedaten, Screenshots, Protokolle oder andere Informationen freiwillig an den Support übermittelt, werden diese zur Bearbeitung der Supportanfrage verarbeitet und können vom Nutzer ausgewählte oder enthaltene Informationen umfassen.

## 8. Abruf von Rechtliches-, Datenschutz- und Lizenzinformationen über GitHub

Wenn der Nutzer in der App die Bereiche Rechtliches, Datenschutz oder Lizenzen öffnet, wird das jeweils aktuelle Markdown-Dokument aus dem öffentlichen Repository `innoVis-ws/innovis-public` über `raw.githubusercontent.com` abgerufen.

Bei diesem Abruf wird technisch eine Verbindung zu GitHub hergestellt. Dabei kann GitHub Informationen wie IP-Adresse, Zeitpunkt des Abrufs, angeforderte URL sowie technische Angaben zum Gerät oder zur App erhalten und verarbeiten. innoVis Web Solutions erhält diese Verbindungsdaten durch den In-App-Abruf nicht direkt.

Weitere Informationen enthält die [GitHub-Datenschutzerklärung](https://docs.github.com/site-policy/privacy-policies/github-general-privacy-statement).

Wenn der Nutzer einen Link „Quelle auf GitHub anzeigen“ öffnet, wird zusätzlich die GitHub-Webseite im Standardbrowser oder einer entsprechenden Systemansicht geöffnet.

## 9. Rechtsgrundlagen

Soweit innoVis Web Solutions personenbezogene Daten tatsächlich erhält oder verarbeitet, hängt die anwendbare Rechtsgrundlage vom jeweiligen Vorgang ab. Die Verarbeitung kann insbesondere auf Art. 6 Abs. 1 lit. b DSGVO beruhen, soweit sie zur Erfüllung einer vom Nutzer angeforderten Leistung im Rahmen eines Vertragsverhältnisses erforderlich ist, oder auf Art. 6 Abs. 1 lit. f DSGVO aufgrund des berechtigten Interesses, die App sicher, zuverlässig und transparent bereitzustellen.

Der überwiegende Teil der Remote-Daten wird lokal zwischen dem Gerät des Nutzers und dessen Remote verarbeitet. Die iCloud-Konfigurationssynchronisierung erfolgt über die Apple-Account-Infrastruktur des Nutzers und wird nicht von innoVis Web Solutions betrieben.

## 10. Speicherdauer

Bei normaler Nutzung führt innoVis Web Solutions keine zentrale Kopie der konfigurierten Remote-Zugangsdaten, Remote-Aktivitäten, Remote-Entitäten oder der über iCloud synchronisierten App-Konfiguration.

Lokal gespeicherte Daten bleiben grundsätzlich erhalten, bis sie vom Nutzer geändert oder entfernt, App-Daten gelöscht oder die App deinstalliert werden. Für über iCloud synchronisierte Konfiguration gelten die iCloud-Account-, Geräte- sowie Speicher- und Löschmechanismen von Apple.

Für Daten, die GitHub beim Abruf einer Veröffentlichung verarbeitet, gelten die Speicher- und Löschregeln von GitHub.

## 11. Empfänger und Drittlandübermittlung

Die direkte LAN-Kommunikation mit der Remote findet zwischen dem Gerät des Nutzers und der Remote statt und wird nicht an den App-Anbieter übertragen.

Für die iCloud-Synchronisierung stellt Apple die Cloud-Infrastruktur bereit. Beim Abruf der Veröffentlichungen Rechtliches, Datenschutz oder Lizenzen verarbeitet GitHub die entsprechende Anfrage. Apple und GitHub können Daten außerhalb der Europäischen Union beziehungsweise des Europäischen Wirtschaftsraums verarbeiten; hierfür gelten die jeweiligen rechtlichen Schutzmechanismen und Datenschutzbedingungen der Anbieter.

## 12. Rechte betroffener Personen

Soweit die Voraussetzungen der DSGVO vorliegen, bestehen insbesondere Rechte auf Auskunft, Berichtigung, Löschung, Einschränkung der Verarbeitung, Datenübertragbarkeit und Widerspruch sowie das Recht, eine Einwilligung mit Wirkung für die Zukunft zu widerrufen, soweit die Verarbeitung auf einer Einwilligung beruht.

Datenschutzanfragen können an contact@unfolded.tools gerichtet werden.

Darüber hinaus besteht das Recht, sich bei einer zuständigen Datenschutzaufsichtsbehörde zu beschweren.

## 13. Änderungen

Diese Datenschutzerklärung kann angepasst werden, wenn sich Funktionen, Datenflüsse, eingesetzte Dienste oder rechtliche Anforderungen ändern. Die aktuelle Fassung ist über den Datenschutz-Button in UC Remote und in diesem öffentlichen Repository verfügbar.
