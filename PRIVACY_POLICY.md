# Privacy Policy for 镜像传输参数生成器 (Image Transfer Parameter Generator)
_Last updated: March 10, 2026_
## Overview
镜像传输参数生成器 ("the Extension") is a Chrome browser extension designed for internal use. This privacy policy describes how the Extension handles data.
## Data Collection
**The Extension does not collect, transmit, or store any personal data on external servers.**
All data processing occurs locally within the user's browser.
## Data Storage
The Extension uses Chrome's `storage.local` API to persist the following user preferences locally on the user's device:
- Namespace input
- Repository name
- Image name prefix
- Selected service list
- Generated parameter results
This data is stored **only on the user's local device** and is never transmitted to any external server or third party.
## Host Access
The Extension operates exclusively on `https://devops.zatech.com`. It injects a content script on this domain solely to:
- Read container image information from the service list page
- Proxy API requests to the platform using the user's existing authenticated session (cookie-based token)
No data extracted from this domain is transmitted outside of the user's local browser environment.
## Permissions
| Permission | Purpose |
|---|---|
| `activeTab` | Read the current tab's URL to extract cluster and namespace information |
| `storage` | Save and restore user preferences and service list across sessions |
| `tabs` | Enable communication between the popup and the content script |
| Host permission (`devops.zatech.com`) | Inject content script and proxy API requests on the target DevOps platform |
## Third-party Sharing
The Extension does **not** share any data with third parties.
## Remote Code
The Extension does **not** use any remote code. All JavaScript is bundled within the extension package.
## Changes to This Policy
If this policy is updated, the updated version will be reflected in this repository with a new "Last updated" date.
## Contact
If you have any questions about this privacy policy, please contact: jun.wang@leadinx.co.jp
```
