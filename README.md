# Portfolio Studio

`index.html` is a browser-based portfolio setup wizard and editor. New portfolios start in the guided wizard, with clickable steps and a focused live preview; finishing the wizard opens the full editor. Existing portfolios open directly in the editor. Edit profile details through the wizard, and add, edit, remove, or drag to reorder standalone containers. The profile, timezone, and interest sections retain their standard positions. `ThemplateExample.html` is the original portfolio example. Serve this folder from a web server (for example, GitHub Pages) to use the included badge gallery; opening the editor as a `file://` URL may prevent local assets from loading.

Published portfolios include styled date hints, an animated profile-picture carousel, an optional cropped profile banner matching the example, and an analogue/digital local clock when timezone display is enabled. Local-time text shows hours and minutes; the analogue clock's second hand continues to move.

## Publishing

Create a repository on your own GitHub account before connecting. For a new portfolio, leave it empty except for an optional README. The editor publishes a generated `index.html`; uploaded images are resized and compressed to WebP before being embedded. The page has a 900 KB publishing limit, so portfolios with many images may still need fewer images. Optional Pages automation needs the additional `Pages: read and write` permission. Otherwise, enable Pages manually in repository settings.

Use a Fine-grained personal access token restricted to that one repository, expiring within 24 hours, with only `Metadata: read-only` and `Contents: read and write` (plus Pages read/write only if enabling Pages from the editor). The token is held in page memory and is not saved to browser storage. GitHub does not expose a token's expiry, repository allow-list, or complete permission set to this browser editor, so it cannot enforce those settings; users must verify them before pasting the token and revoke it after publishing.

Edit mode accepts only an unchanged, canonical `index.html` created by Portfolio Studio. It refuses to overwrite an unrecognized or modified file. Use the editor's consent prompt to review the GitHub Terms of Service, code of conduct, and publishing confirmation before proceeding.
