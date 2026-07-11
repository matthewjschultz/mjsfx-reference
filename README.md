# mjsfx-reference

The canonical reference files for [MJSFX](https://mjsfx.app), the macOS designer for 8-bit game
sound effects.

| Folder | Contents |
|---|---|
| `controllers/` | The bundled `.mjsfxcontroller` configs, byte-identical to the copies inside the shipping app |
| `sounds/` | Example `.mjsfx` sounds used by the format documentation |

Every file format is documented at [mjsfx.app/reference](https://mjsfx.app/reference), complete
enough to write a file from scratch.

## This repo is written by a pipeline

Nothing here is edited by hand. The files are published from the MJSFX source tree by
`publish-mjsfx-reference.sh` (which runs `FormatDocs --reference-repo`): controller configs come
from the same bundled resources the app ships, and example sounds are extracted from the
documentation's own specimen blocks, so this repo cannot drift from the app or its docs. Issues
and pull requests about the files belong with the app, not here.
