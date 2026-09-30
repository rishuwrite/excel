# Architecture

RISHU TOOLS uses an Office.js Task Pane architecture. `manifest.xml` registers the add-in. `taskpane.html` hosts the UI. `src/app.js` manages selection context and feature execution. `src/features.js` is the feature registry. `scripts/` contains build, validation, and local-server tooling.

Feature handlers are selection-aware and prefer bulk range operations. Unsupported desktop-only functionality must use a reliable alternative and be documented.