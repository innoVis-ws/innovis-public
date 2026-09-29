# UC Remote Privacy Policy

Last updated: September 30, 2026

## 1. Controller

The controller responsible for data processing in connection with UC Remote is:

- **innoVis Web Solutions**
- Represented by: Justin Jäger
- Steubenplatz 12
- 64293 Darmstadt
- Hesse, Germany
- Email: contact@unfolded.tools
- Web: [unfolded.tools](https://unfolded.tools)

UC Remote is an independently developed third-party application for Unfolded Circle Remote Two and Remote 3. The app is not operated by, supported by, affiliated with, or officially endorsed by Unfolded Circle ApS.

## 2. Core privacy principle

UC Remote is designed to operate primarily locally. It connects directly to a Remote Two or Remote 3 configured by the user, normally over the local network.

During normal control use, Remote activities, entities, commands, media information, and resources are not routed through a server operated by innoVis Web Solutions. The native app does not require an account with the app provider.

The app contains no advertising integrated by the app provider and no analytics, advertising, or tracking SDKs.

## 3. Data stored locally on the device

To provide the functions requested by the user, UC Remote stores information locally on the device. This may include in particular:

- the name and network address of configured Remotes
- the selected authentication method
- a Web Configurator PIN or Core API key where entered by the user
- app preferences such as language, startup view, interface options, haptics, orientation, and motion settings
- dashboard and activity presentation settings
- keyboard configuration
- activity stream configuration and related presentation settings
- the most recently selected settings section and other local UI state
- locally cached Remote resources such as icons, backgrounds, TV channel logos, sounds, artwork, or stream previews

This information is stored in app, browser, or WebView storage such as IndexedDB, Local Storage, shared app-group storage, or native preferences as required by the relevant feature. Local storage alone does not transmit this information to the app provider.

Cached Remote resources may remain on the device until replaced, manually cleared, the corresponding app data is removed, or the app is uninstalled.

## 4. iCloud configuration synchronization on Apple devices

On supported iOS and iPadOS devices, UC Remote uses Apple's **iCloud Key-Value Storage** to synchronize selected app configuration between devices signed in to the same iCloud account when iCloud is available for the app.

The synchronized configuration can include:

- interface and device preferences
- dashboard layout and dashboard page preferences
- activity-page presentation preferences
- keyboard configuration
- activity stream configuration and related display preferences
- profile-group collapse state and similar UI preferences

Remote-scoped preference keys are associated with the configured Remote using its normalized Remote URL so that equivalent Remote configurations can be matched across devices even when the app assigns different local identifiers.

The iCloud synchronization payload **does not include the saved Remote registry or Remote authentication credentials**. In particular, Web Configurator PINs, Core API keys, and other credentials used to authenticate to a Remote are not placed in the iCloud configuration payload by UC Remote. A Remote therefore still needs to be paired or configured on another device before Remote-specific synchronized preferences can be applied there.

Activity stream configuration can contain URLs or other user-entered configuration values. Users should not place secrets in stream URLs or other synchronized preference fields unless they are comfortable with those values being stored in their personal iCloud account.

iCloud is operated by Apple. The synchronized data is stored and transmitted through the user's Apple/iCloud account infrastructure; innoVis Web Solutions does not operate the iCloud service and does not receive a copy of the synchronized configuration through the app. Apple's processing is governed by Apple's applicable privacy information and iCloud terms.

More information is available in [Apple's Privacy Policy](https://www.apple.com/legal/privacy/).

## 5. Communication with the Unfolded Circle Remote

UC Remote can discover compatible Remotes on the local network using mDNS. After setup, it communicates directly with the selected Remote using HTTP or HTTPS and WebSocket or WebSocket Secure.

Depending on the functions used, Remote configuration, activities, entities, media and resource information, and control commands requested by the user may be exchanged between the device and the Remote. Stored Remote credentials are used to authenticate to the configured Remote.

For local or private network addresses, the app may permit unencrypted HTTP. In that case, transport within the local network is not encrypted. For non-local destinations, the native app requires HTTPS.

This direct Remote communication is not relayed through infrastructure operated by innoVis Web Solutions.

## 6. Native system features

Depending on the platform and enabled settings, UC Remote may use system features such as haptics, screen-orientation controls, widgets, Live Activities, background refresh, and local activity notifications.

Remote state needed for these features is processed by the app on the device and, where required by Apple platform features, in the app's shared local App Group container. The app provider does not operate a proprietary push-notification or Remote-state relay service for these functions.

Permissions can be managed through the operating-system settings of the relevant device.

## 7. Diagnostics and support

UC Remote can expose local diagnostic information and an app log to help troubleshoot the local connection and app state. Diagnostic export is initiated by the user. The app does not automatically upload the exported diagnostics to the app provider.

If the user voluntarily sends exported diagnostics, screenshots, logs, or other information to support, that material is processed for the purpose of handling the support request and may contain information selected or included by the user.

## 8. Legal, privacy, and license publications loaded from GitHub

When the user opens the Legal, Privacy, or Licenses publication in the app, the current Markdown document is retrieved from the public `innoVis-ws/innovis-public` repository through `raw.githubusercontent.com`.

This request establishes a technical connection to GitHub. GitHub may receive and process information such as the IP address, request time, requested URL, and technical information about the device or app. innoVis Web Solutions does not receive this connection data directly from the in-app request.

More information about GitHub's processing is available in the [GitHub Privacy Statement](https://docs.github.com/site-policy/privacy-policies/github-general-privacy-statement).

If the user opens a “View source on GitHub” link, the GitHub website is additionally opened in the default browser or corresponding system view.

## 9. Legal bases

Where innoVis Web Solutions actually receives or processes personal data, the applicable legal basis depends on the relevant operation. Processing may in particular be based on Article 6(1)(b) GDPR where necessary to perform a service requested by the user within a contractual relationship, or Article 6(1)(f) GDPR based on the legitimate interest in providing the app securely, reliably, and transparently.

Most Remote data is processed locally between the user's device and the user's Remote. iCloud configuration synchronization is performed through the user's Apple account infrastructure and is not operated by innoVis Web Solutions.

## 10. Retention

During normal use, innoVis Web Solutions does not maintain a central copy of the user's configured Remote credentials, Remote activities, Remote entities, or iCloud-synchronized app configuration.

Data stored locally generally remains until changed or removed by the user, the app's data is cleared, or the app is uninstalled. iCloud-synchronized configuration is subject to the user's iCloud account, device, and Apple retention/deletion mechanisms.

For data processed by GitHub when a publication is retrieved, GitHub's own retention and deletion rules apply.

## 11. Recipients and international transfers

Direct LAN Remote communication is between the user's device and Remote and is not sent to the app provider.

For iCloud synchronization, Apple is the provider of the cloud infrastructure. When Legal, Privacy, or Licenses publications are retrieved, GitHub is the external provider handling that request. Apple and GitHub may process data outside the European Union or European Economic Area subject to their respective legal safeguards and privacy terms.

## 12. Data subject rights

Where the requirements of the GDPR are met, data subjects may in particular have rights of access, rectification, erasure, restriction of processing, data portability, and objection, as well as the right to withdraw consent with effect for the future where processing is based on consent.

Privacy requests can be sent to contact@unfolded.tools.

Data subjects also have the right to lodge a complaint with a competent data protection supervisory authority.

## 13. Changes

This privacy policy may be updated if app functions, data flows, services used, or legal requirements change. The current version is available from the Privacy button in UC Remote and from this public repository.
