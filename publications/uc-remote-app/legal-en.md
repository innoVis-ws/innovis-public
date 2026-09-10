# Legal Information

Last updated: September 10, 2026

## Imprint

### Provider and responsible person

- **Justin Jäger (jstnjx)**
- Germany
- Email: contact@unfolded.tools
- Web: [unfolded.tools](https://unfolded.tools)
- GitHub: [github.com/jstnjx](https://github.com/jstnjx)

UC Remote is an independent open-source project for Unfolded Circle Remote Two and Remote 3. The project is not operated by, supported by, or officially endorsed by Unfolded Circle ApS.

Third-party product names, trademarks, and logos remain the property of their respective owners. They are referenced solely for identification, interoperability, and description of supported devices and services.

### Contact

For legal notices, privacy requests, support, and other inquiries: contact@unfolded.tools

---

## Privacy Policy

### 1. Controller

The person responsible for data processing in connection with UC Remote is:

- **Justin Jäger (jstnjx)**
- Germany
- Email: contact@unfolded.tools

### 2. Core privacy principle

The native UC Remote app for iOS, iPadOS, and Android is designed to operate primarily locally. It connects directly over the local network to an Unfolded Circle Remote Two or Remote 3 configured by the user.

During normal use, Remote activities, entities, commands, and resources are not routed through a server operated by the project operator. The native app does not require an account with the project operator.

The app contains no advertising integrated by the project operator and no analytics, advertising, or tracking SDKs.

### 3. Data stored locally on the device

To provide the functions requested by the user, the app stores information locally on the device. This may include in particular:

- the name and local network address of configured Remotes
- the selected authentication method
- the Web Configurator PIN or Core API key, where entered by the user
- app preferences such as language, startup view, appearance, haptics, and orientation
- settings for activities and optional activity streams
- the most recently selected settings section
- locally cached Remote resources such as icons, backgrounds, TV channel logos, or sounds

This data is stored in local browser or WebView storage such as IndexedDB and Local Storage. Storing it locally does not by itself transmit it to the project operator.

The resource cache treats stored Remote resources as stale after 30 days. Data may technically remain on the device until overwritten, corresponding settings or app data are manually cleared, or the app is uninstalled.

Where applicable, local storage and access to this information take place to provide functionality explicitly requested by the user. For storage or access that is strictly necessary for the requested digital service, Section 25(2)(2) TDDDG applies in particular.

### 4. Communication with the Unfolded Circle Remote

The app can discover compatible Remotes on the local network using mDNS. After setup, it communicates directly with the selected Remote using HTTP or HTTPS and WebSocket or WebSocket Secure.

Depending on the functions used, Remote configuration, activities, entities, media and resource information, and control commands requested by the user may be exchanged between the device and the Remote. Stored credentials are used only to authenticate to the configured Remote.

For local or private network addresses, the app also permits unencrypted HTTP. In that case, transport within the local network is not encrypted. For non-local destinations, the native app requires HTTPS.

This direct LAN communication is not relayed through infrastructure operated by the project operator.

### 5. Native system features

Depending on the platform and enabled settings, UC Remote may use device features such as haptics, screen orientation controls, iPadOS Live Activities, background refresh, and local activity notifications.

Remote state required for these features is processed by the app on the device. The project operator does not operate a proprietary push-notification service for these features and does not receive Remote activity data through them.

Permissions can be managed through the operating-system settings of the relevant device.

### 6. Loading this legal information from GitHub

The legal information is loaded only when the user opens “Legal”. It is retrieved from the public `innoVis-ws/innovis-public` repository through `raw.githubusercontent.com`.

This request establishes a technical connection to GitHub. GitHub may receive and process information such as the IP address, request time, requested URL, and technical information about the device or app. The project operator does not receive this connection data directly.

More information about GitHub's processing is available in the [GitHub Privacy Statement](https://docs.github.com/site-policy/privacy-policies/github-general-privacy-statement).

If the user opens the “View source on GitHub” link, the GitHub website is additionally opened in the default browser or corresponding system view.

### 7. Legal bases

Where the project operator actually receives or processes personal data, the legal basis depends on the relevant operation. Processing may in particular be based on Article 6(1)(b) GDPR where it is necessary to perform a service requested by the user within a contractual relationship, or Article 6(1)(f) GDPR based on the legitimate interest in providing the app securely, reliably, and transparently.

Most processing of Remote and settings data, however, takes place exclusively locally between the user's device and the user's Remote and is not disclosed to the project operator.

### 8. Retention

During normal use of the native app, the project operator does not store a central copy of locally configured Remote credentials, Remote activities, or Remote entities.

Data stored on the device generally remains there until changed or removed by the user, the app's data is cleared, or the app is uninstalled. Short-lived runtime data may be discarded earlier when the app or relevant view is closed.

For data processed by GitHub when the legal information is retrieved, GitHub's own retention and deletion rules apply.

### 9. Recipients and international transfers

During normal direct-LAN use, Remote data is not transmitted to the project operator or to a cloud service commissioned by the project operator.

When the legal information is retrieved, GitHub is the external recipient of the resulting technical connection data. GitHub may also process data outside the European Union or European Economic Area. Details are provided in GitHub's privacy information.

### 10. Data subject rights

Where the requirements of the GDPR are met, data subjects may in particular have rights of access, rectification, erasure, restriction of processing, data portability, and objection, as well as the right to withdraw consent with effect for the future where processing is based on consent.

Privacy requests can be sent to contact@unfolded.tools.

Data subjects also have the right to lodge a complaint with a competent data protection supervisory authority.

### 11. Changes

This privacy policy may be updated if app functions, data flows, services used, or legal requirements change. The current version is loaded by the app's built-in Legal dialog from this public repository.
