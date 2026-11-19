# Freie Software in Klangbar

Klangbar baut auf den folgenden Bausteinen auf. Jeder steht unter seiner eigenen Lizenz, und die bleibt gültig. Die Nutzungsbedingungen von Klangbar ([LIZENZ.md](LIZENZ.md)) schränken diese Rechte nicht ein. Danke an alle, die diese Projekte möglich machen.

| Baustein | Wofür | Lizenz | Quellcode |
|---|---|---|---|
| Python 3.12 | Laufzeitumgebung | PSF License | https://www.python.org/downloads/source/ |
| Qt 6 über PySide6 | Fenster, Wiedergabe, Grafik | LGPL v3 | https://code.qt.io · https://download.qt.io/official_releases/QtForPython/ |
| FFmpeg 7.1 (Build aus imageio-ffmpeg) | Umwandeln für den Avid- und WAV-Export | GPL v3 (der Build enthält GPL-Teile wie x264 und x265) | https://ffmpeg.org/download.html · https://github.com/imageio/imageio-ffmpeg |
| NumPy | Wellenform und Pegel | BSD-3-Clause | https://github.com/numpy/numpy |
| pyaaf2 | Avid-Bins (AAF) schreiben | MIT | https://github.com/markreidvfx/pyaaf2 |
| PyObjC | Milchglas-Effekt unter macOS | MIT | https://github.com/ronaldoussoren/pyobjc |
| PyInstaller (Bootloader) | macht aus allem eine App | GPL v2 mit Ausnahme für den Bootloader | https://github.com/pyinstaller/pyinstaller |
| Noto Sans Mono (Auszug, „Klangbar Marke“) | Schriftzug und App-Icon | SIL Open Font License 1.1 | https://github.com/notofonts/latin-greek-cyrillic |
| Unbounded | Schrift des früheren Logos (liegt der App noch bei) | SIL Open Font License 1.1 | https://github.com/googlefonts/unbounded |
| Universal Category System (UCS) | Liste der Sound-Kategorien | gemeinfrei | https://universalcategorysystem.com |

## Hinweise zu LGPL und GPL

**Qt (LGPL v3):** Klangbar bindet die Qt-Bibliotheken dynamisch ein. Sie liegen als eigene Dateien in `Klangbar.app/Contents/Frameworks/PySide6/Qt/lib` und lassen sich gegen andere, auch selbst gebaute, Fassungen derselben Qt-Version austauschen. Den vollständigen Quellcode von Qt und PySide6 gibt es unter den Links oben.

**FFmpeg (GPL v3):** FFmpeg liegt als eigenständiges Programm in der App (`Klangbar.app/Contents/Frameworks/ffmpeg`). Klangbar ruft es nur als separates Programm auf. Klangbar ist mit FFmpeg nicht verlinkt und steht deshalb nicht unter der GPL. Für FFmpeg selbst gilt die GPL: Du darfst es nutzen, verändern und weitergeben. Den Quellcode der verwendeten Fassung 7.1 findest du unter https://ffmpeg.org/releases/. Auf Anfrage über ein [Issue in diesem Repository](../../issues) schicke ich dir für mindestens drei Jahre nach der jeweiligen Version eine Kopie des Quellcodes und der Build-Einstellungen.

## Lizenztexte

- GNU LGPL v3: https://www.gnu.org/licenses/lgpl-3.0.html
- GNU GPL v3: https://www.gnu.org/licenses/gpl-3.0.html
- GNU GPL v2: https://www.gnu.org/licenses/old-licenses/gpl-2.0.html
- SIL Open Font License 1.1: https://openfontlicense.org
- PSF License: https://docs.python.org/3/license.html
- MIT und BSD-3-Clause: in den Repositories der jeweiligen Projekte
