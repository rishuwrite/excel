# RISHU TOOLS

Personal Excel productivity toolkit built as an Office.js Excel task pane add-in.

## Current build
- **119 feature definitions**
- Search + category filtering
- Selection analyzer
- Home-ribbon `Open RISHU TOOLS` command
- HTTPS localhost development server with Microsoft Office development certificates
- Build + validation + Node test suite

## Run locally
1. Install Node.js.
2. In the repository root run `npm install`.
3. Run `npm start`.
4. The server hosts `https://localhost:3000`.
5. In Excel, sideload `manifest.xml` through **Home → Add-ins → More Settings / Advanced / Upload My Add-in** (the exact wording depends on your Excel build).

If Windows asks you to trust the development certificate, allow it. Microsoft documents that self-signed certificates can be used for local Office Add-in development/testing, and Office add-in web content should use HTTPS. The project uses Microsoft's `office-addin-dev-certs` package for this.

## Build
`npm run validate` → `npm test` → `npm run build`

The `dist/` folder is the deployable web-app output. The manifest remains at the repository root for sideloading.
