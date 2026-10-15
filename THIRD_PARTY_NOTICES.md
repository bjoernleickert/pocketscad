# Third-party notices

Pocket SCAD is licensed under the GNU General Public License v3.0 or later (see `LICENSE`).
It includes or loads the following third-party components.

## three.js r160 (incl. OrbitControls, STLLoader)
- Files: `vendor/three/`
- License: MIT, see `licenses/three.js-MIT.txt`
- Source: https://github.com/mrdoob/three.js/tree/r160

## OpenSCAD (WebAssembly build)
- Files: `vendor/openscad/` (you add these, see README)
- License: GPL-2.0-or-later with CGAL exception (OpenSCAD); the WebAssembly build bundles
  CGAL (GPL-3.0-or-later / LGPL-3.0-or-later), Manifold (Apache-2.0), Boost (BSL-1.0),
  Eigen (MPL-2.0), GMP and MPFR (LGPL-3.0-or-later), GLib (LGPL-2.1-or-later),
  Cairo (LGPL-2.1 / MPL-1.1), FreeType (FTL / GPL-2.0), HarfBuzz (MIT), fontconfig (MIT-style),
  libxml2 (MIT), lib3mf (BSD-2-Clause), libzip (BSD-3-Clause), zlib (zlib), expat (MIT),
  double-conversion (BSD-3-Clause), libffi (MIT). As a whole: GPL-3.0-or-later.
  License texts: `LICENSE` (GPL-3.0), `licenses/GPL-2.0.txt`.
- Source: https://github.com/openscad/openscad-wasm, release tag: main @ dc2ff913b4193b1ebfef863da3f7e84f8fbc1e11
  The corresponding source is the openscad-wasm repository at that tag; its Makefile pins
  the exact versions of all dependencies listed above.
