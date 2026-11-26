<!--
@license
Copyright (c) <YOUR_COPYRIGHT_HOLDER>

Use of this source code is governed by terms that can be
found in the LICENSE file in the root of this package.
-->

# Themen-Leitfaden

TODO: Ein oder zwei Sätze dazu, was diese DNA-Schicht bereitstellt.

## Was konfiguriert ist <a id="what-is-configured"></a>

- TODO: Liste auf, was die Dateien in `dna/` einrichten
- In Vorlagen verfügbare Variablen: `<YOUR_COPYRIGHT_HOLDER>`, `<YOUR_COMPANY>`
  (Werte in `dna/_vars.json`)

## Eine Datei hinzufügen <a id="add-a-file"></a>

- Lege sie in `dna/` ab. Ein führendes `dot-` wird im nutzenden Repo zu
  einem `.` (`dna/dot-foo/bar.json` → `.foo/bar.json`)
- Führe `dart test` aus, um die DNA zu instanziieren und
  `dna/_generated.json` zu aktualisieren

## In einem nutzenden Repo überschreiben <a id="override-in-a-consuming-repo"></a>

- Eine Datei mit gleichem Pfad in einer späteren Schicht ersetzt diese
  vollständig
- Eine `<name>.overrides.json` führt stattdessen zusammen: Objekte werden
  tief zusammengeführt, `"key!"` ersetzt ohne Zusammenführen, `"key+"`
  hängt an ein Array an — die vollständige Syntax steht in der README von
  helix
