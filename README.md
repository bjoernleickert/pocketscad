# Pocket SCAD

**OpenSCAD in your pocket. Code, preview and export 3D models right in your browser.**

Pocket SCAD brings OpenSCAD to your browser and your phone. It runs the real OpenSCAD engine, compiled to WebAssembly, so your existing `.scad` files work as they do on the desktop.

Write code with a touch-friendly editor and a symbol bar for brackets and semicolons. Tweak your design with customizer sliders generated from your parameters, and check the result in an interactive 3D view with exact dimensions in millimeters. When it's ready, export STL or 3MF and send it straight to your slicer.

Everything happens on your device: no install, no account, and your models never leave your browser. Pocket SCAD is free and open source under the GPL-3.0-or-later. It is not affiliated with the OpenSCAD project.

## Setup checklist
1. **OpenSCAD engine:** add the official build to `vendor/openscad/` (see the README there).
   Until then the app falls back to the `openscad-wasm` package on jsDelivr/unpkg.
2. **Production:** `ALLOW_CDN_FALLBACK` in `index.html` is `false`, so the engine must be in `vendor/openscad/`. Set it to `true` only for testing without a local engine.
3. **Tip link and repository:** set `TIP_URL` (and, if the repo moves, `SOURCE_URL` / `SOURCE_BRANCH`) in the settings block at the top of the main script in `index.html`.
4. **Impressum:** enter your e-mail address in `impressum.html` (`user` and `domain` in the
   script at the bottom). An e-mail address is required by § 5 DDG.
5. **License notice:** enter the engine's release tag in `THIRD_PARTY_NOTICES.md`.

## Hosting on GitHub Pages
- Push this folder to a public repository, then Settings → Pages → deploy from branch `main`, folder `/`.
- Custom domain: verify the domain in your GitHub account settings first, then add it under
  Settings → Pages and enable "Enforce HTTPS". GitHub writes a `CNAME` file for you.

## Search engines
`impressum.html` carries `noindex` meta tags. It is intentionally **not** blocked in `robots.txt`,
because a blocked page can't be read and its URL may still show up in results.

## License
GPL-3.0-or-later. See `LICENSE` and `THIRD_PARTY_NOTICES.md`.
