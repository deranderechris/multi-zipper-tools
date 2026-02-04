#MULTI-ZIPPER TOOLS
Vier Batch-Tools zum automatischen Packen von Projekten (Release, Source, Full ZIP)

Dieses Paket enthält vier eigenständige Batch-Dateien, die Python-Projekte zuverlässig packen, sichern und als Release bereitstellen. Alle Tools funktionieren ohne zusätzliche Software – Windows + PowerShell reichen aus.

Alle .bat-Dateien müssen direkt im Projektordner liegen.

---------------------------------------------------------
1) zip_project.bat
---------------------------------------------------------

Funktion:
Erstellt ein vollständiges ZIP-Archiv des gesamten Projekts.

Packt ein:
- Alle Dateien
- Alle Unterordner
- Assets, Icons, Configs usw.

Ergebnis:
projektname.zip

Zweck:
- Komplettsicherung
- Weitergabe an Entwickler
- Archivierung

---------------------------------------------------------
2) zip_release_and_source.bat
---------------------------------------------------------

Funktion:
Erstellt zwei getrennte ZIP-Pakete:

Release.zip  -> EXE, ICON, wichtige Dateien (für Endnutzer)
Source.zip   -> kompletter Quellcode (für Entwickler)

Ergebnis:
projektname_Release.zip
projektname_Source.zip

Zweck:
- Saubere Trennung von Release und Source
- Ideal für GitHub-Releases
- Weitergabe an Tester und Entwickler

---------------------------------------------------------
3) zip_release.bat
---------------------------------------------------------

Funktion:
Erstellt ein reines Release-Paket ohne Source-Code.

Packt ein:
- EXE
- ICON
- wichtige Dateien (README, LICENSE, Configs)

Ergebnis:
projektname_Release.zip

Zweck:
- Endnutzer-Downloads
- Kleine, saubere Release-Pakete

---------------------------------------------------------
4) build_and_zip_release.bat
---------------------------------------------------------

Funktion:
Vollautomatischer One-Click-Release-Builder.

Ablauf:
1. Baut automatisch eine EXE aus dem Projekt
2. Erstellt einen release/-Ordner
3. Kopiert EXE + ICON + wichtige Dateien hinein
4. Erstellt zwei ZIP-Pakete:
   - Release.zip
   - Source.zip

Ergebnis:
release\ (fertige Dateien)
projektname_Release.zip
projektname_Source.zip

Zweck:
- Vollautomatisierte Release-Erstellung
- Ideal für GitHub-Releases
- Spart Zeit bei wiederholten Builds

---------------------------------------------------------
Hinweise
---------------------------------------------------------

- Alle .bat-Dateien müssen im Projektordner liegen
- ZIP-Dateien werden automatisch überschrieben
- PowerShell wird zum Packen verwendet
- Keine zusätzlichen Programme erforderlich
- Funktioniert auf jedem Windows-System
 multi-zipper-tools
Vier Batch-Tools zum automatischen Packen von Projekten (Release, Source, Full ZIP)
