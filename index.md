# Unqork Colorizer Privacy Policy
 
Last updated: November 18, 2026.

Unqork Colorizer has no data-collection server, analytics, telemetry, advertising, or network client. No application APIs are called. Nothing is transmitted by the extension.

The extension reads the rendered DOM of sites you explicitly allow to identify component cards and group structure. It adds temporary visual annotations and CSS. It does not access application framework state, authentication tokens, cookies, module APIs, or configuration objects. It does not trigger Save or Publish.

Persistent local data consists of your enabled preference, selected colors, and optional imported classification metadata. Metadata contains component keys, optional component IDs, normalized types, and ancestor keys. The entire URL is hashed to scope each import; the URL itself is not saved as part of the import. Raw exported HTML, configuration values and unrelated export properties are not retained. Imports are optional and remain in `chrome.storage.local`, not sync storage.

Permissions:

| Permission | Purpose |
| --- | --- |
| `storage` | Persist local settings and optional classification metadata. |
| `activeTab` | Identify the tab where you open the popup to offer access to its hostname. |
| `scripting` | Register/inject the bundled isolated-world colorizer on allowed sites. |
| Optional `https://*/*` | Permit the user to approve their own organization's exact HTTPS hostname. No hosts are granted at installation. |

Use the popup to remove access to the current site or clear its metadata. Use the options page to delete all imported metadata. Removing site access does not delete saved preferences or metadata, so regranting the same host can resume your preferences. Uninstalling the extension removes its Chrome local storage. Refresh an open page if residual styling remains after Chrome removes the extension.

The extension does not include third-party runtime libraries. Development dependencies are only used to test and package it. This privacy statement applies to this source release; distributors are responsible for keeping it accurate if they modify the extension.

## Questions

For privacy questions, open an issue at https://github.com/manojkd111/unqork-colorizer-privacy/issues. Do not include confidential module or customer data in public issues.

