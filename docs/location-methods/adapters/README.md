## Standard adapters (scaffold)

This directory is reserved for **standard-specific adapter modules** that align external standards (e.g., Alert-C, OpenLR, TPEG) to the methodology modules in `../`.

Adapters should prefer:\n- subclassing / equivalence axioms\n- annotation provenance and mapping notes\n- controlled enumerations where required\n\nAdapters should avoid duplicating shared primitives (coordinates, geometry, quality, external IDs).

