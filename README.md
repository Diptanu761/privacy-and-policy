Privacy Policy for Foxisync Extension

Last Updated: August 2, 2025

This Privacy Policy describes how the Foxisync Chrome Extension ("the Extension") operates regarding your data. Foxisync is designed to enhance your web browsing experience through custom sound effects and visual themes.

1. Data Collection

Foxisync is committed to your privacy. The Extension does NOT collect, store, or transmit any of the following types of user data:

Personally Identifiable Information (PII): We do not collect your name, email address, physical address, phone number, age, date of birth, or any other information that could directly identify you.

Health Information: We do not collect any data related to your health, medical history, symptoms, diagnoses, or procedures.

Financial and Payment Information: We do not collect any data related to your financial transactions, credit card numbers, bank account details, credit ratings, or payment history. Foxisync is a free extension and does not process payments.

Authentication Information: We do not collect passwords, credentials, security questions, or personal identification numbers (PINs). Foxisync does not require any user accounts or logins.

Personal Communications: We do not access or collect the content of your emails, texts, chat messages, or any other personal communications.

Location Information: We do not collect data about your geographical region, IP address, GPS coordinates, or any other information about your physical location.

Web History: We do not collect, store, or transmit a persistent list of web pages you have visited, nor associated data such as page titles or timestamps. Our interaction with tabs is ephemeral and solely for the purpose of triggering immediate sound effects or theme synchronization.

User Activity (Logged): While the Extension responds to user actions like clicks, mouse movements, scrolls, and keystrokes to trigger sound effects, it does NOT collect, monitor, or log these activities for storage or transmission. These events are processed in real-time to provide auditory feedback only.

Website Content: We do not collect or transmit the text, images, sounds, videos, or hyperlinks from the content of the websites you visit. Our content scripts interact with the Document Object Model (DOM) to detect user actions for sound effects but do not extract or store the actual content of the page.

2. Local Storage Usage

Foxisync utilizes your browser's local storage (chrome.storage.local) exclusively to save your personal preferences and the Extension's operational state. This data is stored directly on your local device and is NOT accessed, shared, or transmitted by us to any external servers or third parties. The data stored includes:

Volume Settings: Your customized volume levels for various sound effects (e.g., general volume, tab open, tab close, click, scroll).

Selected Theme: Your chosen visual and audio theme to ensure it loads automatically when you open a new tab or restart your browser.

Sound Paths Configuration: The specific file paths for sound effects associated with your active theme.

Music Playback State: Whether the background music on your new tab page is currently playing or paused.

This local data retention is solely for the purpose of providing a consistent and personalized user experience.

3. Permissions Used and Justification

Foxisync requests only the minimum necessary permissions required to deliver its advertised features. Each permission is used strictly for the purposes described below:

tabs: This permission is essential for detecting and responding to browser tab events (e.g., chrome.tabs.onCreated, chrome.tabs.onRemoved, chrome.tabs.onMoved, chrome.tabs.onUpdated for mute/unmute status). It allows the Extension to play corresponding sound effects for these actions and to query/send messages to existing tabs for theme synchronization. No sensitive tab content or browsing history is accessed or stored.

downloads: Used to listen for chrome.downloads.onCreated and chrome.downloads.onChanged events. This enables the Extension to play distinct sound effects when a download starts, completes, or is interrupted. No download content or personal download history is accessed or modified.

bookmarks: Utilized to listen for chrome.bookmarks.onCreated events. This allows the Extension to play a specific sound effect when a new bookmark is successfully added by the user. No existing bookmark data is accessed, modified, or stored.

offscreen: This permission is crucial for enabling continuous background audio playback in Manifest V3. It allows the Extension to create a small, invisible offscreen.html document. This document hosts an audio element that plays a silent, looping sound, ensuring the offscreen context remains active and can reliably play sound effects triggered by the service worker. No user data is processed or stored by the offscreen document.

storage: As detailed in Section 2, this permission is used exclusively for saving and retrieving user preferences (volume settings, selected theme, sound paths, music state) locally on the user's device.

scripting: This permission is used with chrome.scripting.executeScript to dynamically inject content.js into web pages (http://*/*, https://*/*). This is necessary for content.js to detect in-page user interactions (like clicks and scrolls) and trigger associated sound effects. Content scripts run in an isolated world, preventing interference with the web page and limiting data access to event detection for sound purposes.

host_permissions (<all_urls>): This broad permission is required to allow scripting to inject content.js into any standard web page for universal in-page sound effects. It also enables chrome.tabs.query and chrome.tabs.sendMessage to reach all active tabs for theme synchronization. This permission does NOT grant access to sensitive user data or browsing history; its use is strictly confined to the functionalities described.

4. Third-Party Services

Foxisync utilizes publicly available Content Delivery Networks (CDNs) for certain styling and icon libraries (e.g., Google Fonts, Boxicons). These CDNs are used solely for loading static assets (fonts, icons) and do not involve the collection or transmission of user data by Foxisync. The Tailwind CSS library is included locally within the extension package.

5. Changes to This Privacy Policy

We may update this Privacy Policy from time to time to reflect changes in our practices or for other operational, legal, or regulatory reasons. We will notify you of any changes by posting the new Privacy Policy on this page. You are advised to review this Privacy Policy periodically for any changes.

6. Contact Us

If you have any questions about this Privacy Policy or Foxisync's data practices, please contact us at:

[Your Contact Email Address, e.g., foxisync.support@example.com]
