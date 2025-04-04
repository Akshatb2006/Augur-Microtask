# 🛠 Microtask 4 — Documentation Contribution

This microtask involves identifying and addressing documentation issues in the CHAOSS Augur repository. I found a broken link pointing to the Augur live demo, raised a GitHub issue, and proposed a fix.

---

## 📌 Problem Identified

The `CONTRIBUTING.md` file in the Augur repository contained a broken link to the **Live Augur Demo**. Attempting to access the link resulted in a `Connection Refused` error.

### 🔗 Broken Link
```md
[Live Augur demo](http://augur.osshealth.io)
```
---
### 🔍 Steps to Reproduce
Navigate to the CONTRIBUTING.md file in the CHAOSS Augur GitHub repository.

Click the Live Augur demo link.

Observe that the site does not load, showing a connection error.

---

### ✅ Expected Behavior
The link should navigate to a working instance of the Augur demo dashboard.

---

### ❌ Actual Behavior
The site failed to load, showing an error like This site can’t be reached.

---

### 📝 Fix Implemented
Removed or commented out the broken link with a note (until a working demo URL is available)
---

### 🧵 Issue Raised
https://github.com/chaoss/augur/issues/3065
