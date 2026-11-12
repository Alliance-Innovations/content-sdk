---
'@sitecore-content-sdk/nextjs': patch
---

Fix `RichText` internal links hijacking Cmd/Ctrl/Shift/Alt and non-primary clicks. These clicks, as well as clicks on links with a `download` attribute or a non-`_self` target, now fall through to default browser behavior (open in new tab/window, download) instead of triggering client-side navigation in the current tab.
