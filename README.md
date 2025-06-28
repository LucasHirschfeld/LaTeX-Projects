# LaTeX Projects Repository

Dieses Repository enthält meine LaTeX-Dokumente und Projekte.

## Struktur

- `documents/` - Hauptdokumente
- `templates/` - Wiederverwendbare LaTeX-Vorlagen
- `figures/` - Bilder und Grafiken
- `bibliography/` - Literaturverzeichnisse und Zitationsdateien

## Automatischer Build

Dieses Repository nutzt GitHub Actions, um LaTeX-Dokumente automatisch zu kompilieren. Bei jedem Push werden die PDFs erstellt und als Artifacts bereitgestellt.

## Lokale Entwicklung

### Voraussetzungen
- LaTeX-Distribution (MacTeX, TeX Live, MiKTeX)
- VS Code mit LaTeX Workshop Extension

### Kompilierung
```bash
# Für einzelne Dokumente
lualatex document.tex

# Mit Biber für Bibliographien
lualatex document.tex
biber document
lualatex document.tex
lualatex document.tex
```

## Verwendete Tools
- **LuaLaTeX** - Primärer LaTeX-Compiler
- **Biber** - Bibliographie-Verarbeitung
- **GitHub Actions** - Automatische PDF-Generierung
