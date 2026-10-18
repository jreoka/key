# key

PGP public key for **Cross Nastasi <jreoka1@gmail.com>**

| URL | What you get |
| --- | --- |
| <https://key.dill.moe> | Raw key, no markup — safe for `curl ... \| gpg --import` |
| <https://key.dill.moe/key.html> | Same key, formatted for reading in a browser |
| <https://key.dill.moe/cross.pub> | Raw key file, `text/plain` |

Fingerprint:

```
A2B9 B79B F56D 16EB B5BD  1D4E CA77 2969 CBD5 2177
```

Import:

```sh
curl -fsSL https://key.dill.moe | gpg --import
```

`index.html` contains the armored key and nothing else, which is why `curl` on the
bare domain returns only the key. GitHub Pages serves every `index.html` as
`text/html`, so a browser collapses the whitespace — use `/key.html` to read it.
