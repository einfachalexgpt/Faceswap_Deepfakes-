# **deepfakes_faceswap**

<p align="center">
  <a href="https://faceswap.dev"><img src="https://i.imgur.com/zHvjHnb.png" alt="FaceSwap Logo"></a>
<br />FaceSwap ist ein Tool, das Deep Learning verwendet, um Gesichter in Bildern und Videos zu erkennen und auszutauschen.
</p>

<p align="center">
<img src="https://i.imgur.com/nWHFLDf.jpg" alt="FaceSwap Beispiel"></p>

<p align="center">
<a href="https://www.patreon.com/bePatron?u=23238350"><img src="https://c5.patreon.com/external/logo/become_a_patron_button.png" alt="Patreon Support"></a>
&nbsp;&nbsp;&nbsp;&nbsp;<a href="https://discord.gg/FC54sYg"><img src="https://i.imgur.com/gIpztkv.png" alt="Discord"></a>
</p>

<p align="center">
  <a href="https://www.dailymotion.com/video/x810mot"><img src="https://user-images.githubusercontent.com/36920800/178301720-b69841bb-a1ca-4c20-91db-a2a10f5692ca.png" alt="Emma Stone/Scarlett Johansson FaceSwap"></a>
<br />Emma Stone/Scarlett Johansson FaceSwap mit dem Phaze-A Modell
</p>

<p align="center">
  <a href="https://www.youtube.com/watch?v=r1jng79a5xc"><img src="https://img.youtube.com/vi/r1jng79a5xc/0.jpg" alt="Jennifer Lawrence/Steve Buscemi FaceSwap"></a>
<br />Jennifer Lawrence/Steve Buscemi FaceSwap mit dem Villain Modell
</p>

![Build Status](https://github.com/deepfakes/faceswap/actions/workflows/pytest.yml/badge.svg) [![Documentation Status](https://readthedocs.org/projects/faceswap/badge/?version=latest)](https://faceswap.readthedocs.io/en/latest/?badge=latest)

**Bevor du beginnst, lies bitte [INSTALL.md](INSTALL.md).**

- [deepfakes_faceswap](#deepfakes_faceswap)
- [Manifesto](#manifesto)
  - [FaceSwap hat ethische Anwendungsbereiche.](#faceswap-hat-ethische-anwendungsbereiche)
- [Setup und Ausführung des Projekts](#setup-und-ausführung-des-projekts)
- [Überblick](#überblick)
  - [Extract](#extract)
  - [Train](#train)
  - [Convert](#convert)
  - [GUI](#gui)
- [Allgemeine Hinweise:](#allgemeine-hinweise)
- [Hilfe! Ich brauche Unterstützung!](#hilfe-ich-brauche-unterstützung)
  - [Discord-Server](#discord-server)
  - [FaceSwap-Forum](#faceswap-forum)
- [Spenden](#spenden)
  - [Patreon](#patreon)
  - [Einmalige Spenden](#einmalige-spenden)
    - [@torzdf](#torzdf)
    - [@andenixa](#andenixa)
- [Wie kann man beitragen?](#wie-kann-man-beitragen)
  - [Für generative Modell-Interessierte](#für-generative-modell-interessierte)
  - [Für Entwickler](#für-entwickler)
  - [Für fortgeschrittene Anwender](#für-fortgeschrittene-anwender)
  - [Für Endanwender](#für-endanwender)
  - [Für Kritiker](#für-kritiker)
- [Über github.com/deepfakes](#über-githubcomdeepfakes)
  - [Was ist dieses Repo?](#was-ist-dieses-repo)
  - [Warum dieses Repo?](#warum-dieses-repo)
  - [Warum heißt es 'deepfakes', wenn es nicht von /u/deepfakes ist?](#warum-heißt-es-deepfakes-wenn-es-nicht-von-udeepfakes-ist)
  - [Was, wenn /u/deepfakes das stört?](#was-wenn-udeepfakes-das-stört)
- [Über maschinelles Lernen](#über-maschinelles-lernen)
  - [Wie erkennt oder formt ein Computer Gesichter? Was ist maschinelles Lernen? Was ist ein neuronales Netzwerk?](#wie-erkennt-oder-formt-ein-computer-gesichter-was-ist-maschinelles-lernen-was-ist-ein-neuronales-netzwerk)

# 📜 Manifesto

## FaceSwap hat ethische Anwendungsbereiche.

Als FaceSwapping erstmals entwickelt wurde, war es eine bahnbrechende Technologie, ein großer Schritt in der KI-Entwicklung. Leider wurde es von einigen für unangemessene Zwecke verwendet. Trotz dieser problematischen Anwendungen war es der erste KI-Code, den jeder herunterladen und durch Experimentieren ohne tiefgehende mathematische oder theoretische Kenntnisse nutzen konnte.

Heutzutage wird FaceSwap von Entwicklern genutzt, um KI-Techniken zu erforschen und zu experimentieren. Auch wenn die Software missbraucht werden kann, liegt der Fokus der Entwickler auf ethischen Anwendungsbereichen wie Filmen, sozialen Kommentaren und Experimenten.

- FaceSwap ist **nicht** für unangemessene Inhalte.
- FaceSwap ist **nicht** zum heimlichen Ändern von Gesichtern ohne Zustimmung.
- FaceSwap ist **nicht** für illegale oder unethische Zwecke.

# 🛠️ Setup und Ausführung des Projekts

FaceSwap ist ein Python-Programm, das auf Windows, Linux und macOS läuft. Für die beste Leistung wird eine moderne GPU mit CUDA-Unterstützung empfohlen.

Weitere Anweisungen findest du in [INSTALL.md](INSTALL.md).

# 🗂️ Überblick

Das Projekt umfasst mehrere Hauptschritte:
- **Bilder und Videos sammeln**
- **Extract**: Gesichter aus Fotos extrahieren
- **Train**: Ein Modell auf den extrahierten Gesichtern trainieren
- **Convert**: Neue Gesichter in die Quellbilder einfügen

Schau dir [USAGE.md](USAGE.md) für detaillierte Anweisungen an.

## Extract
Verwende `python faceswap.py extract`, um Gesichter aus Bildern zu extrahieren.

## Train
Verwende `python faceswap.py train`, um ein Modell zu trainieren.

## Convert
Verwende `python faceswap.py convert`, um Gesichter zu konvertieren.

## GUI
Du kannst alternativ die GUI verwenden, indem du `python faceswap.py gui` ausführst.

# 📝 Allgemeine Hinweise:

Alle Skripte haben `-h`/`--help` Optionen, um Argumente anzuzeigen. Es gibt auch ein Video-Konvertierungstool, das über `python tools.py effmpeg -h` aufgerufen werden kann.

# ❓ Hilfe! Ich brauche Unterstützung!

## Discord-Server
Der beste Ort, um Unterstützung zu erhalten, ist der [FaceSwap Discord-Server](https://discord.gg/FC54sYg).

## FaceSwap-Forum
Alternativ kannst du Fragen im [FaceSwap-Forum](https://faceswap.dev/forum) stellen.

# 💰 Spenden

Die Entwickler investieren viel Zeit in die Verbesserung von FaceSwap. Wenn dir das Programm gefällt, ziehe bitte eine Spende in Betracht.

## Patreon
Unterstütze uns über unsere [Patreon-Seite](https://www.patreon.com/bePatron?u=23238350).

## Einmalige Spenden

### @torzdf
**Bitcoin:** bc1qpm22suz59ylzk0j7qk5e4c7cnkjmve2rmtrnc6  
**Ethereum:** 0xd3e954dC241B87C4E8E1A801ada485DC1d530F01  
**Paypal:** [Spenden](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=JZ8PP3YE9J62L)

### @andenixa
**Paypal:** [Spenden](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=NRVLQYGS6NWTU)

# 👨‍💻 Wie kann man beitragen?

## Für generative Modell-Interessierte
- Diskutiere im 'faceswap-model'-Bereich Alternativen zum aktuellen Algorithmus.

## Für Entwickler
- Forke das Repo und experimentiere damit.
- Schau dir Issues mit dem 'dev'-Tag an.

## Für fortgeschrittene Anwender
- Klone das Repo und spiele damit herum.
- Unterstütze andere im [FaceSwap-Forum](https://faceswap.dev/forum).

## Für Endanwender
- Lade den Code herunter und experimentiere.
- Sei geduldig, diese Technologie ist noch neu!

# 🤖 Über github.com/deepfakes

## Was ist dieses Repo?
Es ist ein Community-Repository für aktive Benutzer.

## Warum dieses Repo?
Das joshua-wu-Repo scheint inaktiv zu sein, daher wurde dieses geschaffen.

# 💡 Über maschinelles Lernen

## Wie funktioniert maschinelles Lernen und was ist ein neuronales Netzwerk?
Es ist kompliziert. Hier ist ein hilfreiches Video:
[![Wie Maschinen lernen](https://img.youtube.com/vi/R9OHn5ZF4Uo/0.jpg)](https://www.youtube.com/watch?v=R

9OHn5ZF4Uo)

Mehr Details hier:
[![Neuronale Netzwerke erklärt](https://img.youtube.com/vi/aircAruvnKk/0.jpg)](https://www.youtube.com/watch?v=aircAruvnKk)
