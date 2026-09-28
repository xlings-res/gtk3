# gtk3

xlings payload repacked from upstream binaries (conda-forge / Debian) by
[`.agents/tools/repack/repack.py`](https://github.com/openxlings/xim-pkgindex/tree/main/.agents/tools/repack).
Recipe: [`xim-pkgindex`](https://github.com/openxlings/xim-pkgindex) `pkgs/g/gtk3.lua`.

Every release asset carries `PROVENANCE.md` (upstream artefacts, sha256, the exact command) and a `.sha256` sidecar.

## Sources

| artefact | sha256 | origin |
|---|---|---|
| https://conda.anaconda.org/conda-forge/linux-64/gtk3-3.24.43-h0359ba6_0.conda | `493d416b436bf9902d246ae333f0e1ecfb7d8193f0acd0e5f30bb2405f06558b` | conda-forge gtk3 3.24.43 h0359ba6_0 (LGPL-2.0-or-later) |

## Command

```
.agents/tools/repack/repack.py \
    --name gtk3 \
    --version 3.24.43 \
    --arch x86_64 \
    --src https://conda.anaconda.org/conda-forge/linux-64/gtk3-3.24.43-h0359ba6_0.conda#493d416b436bf9902d246ae333f0e1ecfb7d8193f0acd0e5f30bb2405f06558b \
    --relocate 'lib/libgtk-3.so*' \
    --relocate 'lib/gtk-3.0/*' \
    --require lib/libgailutil-3.so.0 \
    --require lib/libgdk-3.so.0 \
    --require lib/libgtk-3.so.0
```

