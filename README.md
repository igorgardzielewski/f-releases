# f.

Gotowe paczki edytora **f.** (macOS, Apple Silicon). Kod źródłowy jest prywatny – tu są tylko wydania.

## Instalacja

```sh
curl -LO https://github.com/igorgardzielewski/f-releases/releases/latest/download/f-darwin-arm64.dmg
open f-darwin-arm64.dmg                      # przeciągnij f.app do Applications
xattr -dr com.apple.quarantine /Applications/f.app
```

Aplikacja nie jest notaryzowana przez Apple, dlatego potrzebne jest polecenie `xattr` – bez niego macOS zgłosi, że aplikacja jest uszkodzona.

Komenda `f` w terminalu:

```sh
mkdir -p ~/.local/bin && ln -sf /Applications/f.app/Contents/Resources/app/bin/code ~/.local/bin/f
```
