<!--
author:   Sebastian Zug & André Dietrich

email:    LiaScript@web.de

version:  0.0.1

language: de

narrator: Deutsch Female

comment:  Try to write a short comment about
          your course, multiline is also okay.

-->

[![LiaScript](https://raw.githubusercontent.com/LiaScript/LiaScript/master/badges/course.svg)](https://LiaScript.github.io/course/?https://raw.githubusercontent.com/LiaPlayground/LiaScript_Tutorial_Kiel/main/D-LiaScript_Tutorial.md)

# Entwicklung von OER mit LiaScript und GitHub


**Allgemeine Ziele:**

* __100%__
  [Markdown](https://en.wikipedia.org/wiki/Markdown)-[Syntax](https://de.wikipedia.org/wiki/Syntax)
* __90%__
  [LiaScript](https://LiaScript.github.io)
* __20%__
  kennenlernen von [Versionmanagement](https://de.wikipedia.org/wiki/Versionsverwaltung) und kollaborativem Arbeiten mit [git](https://de.wikipedia.org/wiki/Git) und [GitHub](https://github.com)

---

**Zeitplan**

* __Vorstellung:__
  Infos zu uns, Forschungsziele, Projekte, etc.

* __Vorstellung/ Erwartungen der Teilnehmer__

  - Was erwarten Sie von der heutigen Veranstaltung, Welchen Hintergrund habe Sie?
  - Eintragung in ein Etherpad Dokument
  - Kurze Besprechung der Inhalte und der Arbeitsmethodik bei dessen Erstellung
  - synchrones kollaboratives Arbeiten --> Herausforderung Synchronisation

* __Motivation OER:__

  - Ziele, Zentrale Aussage zu den Anforderungen: Verteiltheit der Editierung
  - (Lösung mit Git), einfache Editierung interaktiver Inhalte (Lösung mit LiaScript)
  - Ableitung des folgenden Ablaufes - Phase 1: Github EInführung, Phase 2: LiaScript

* __Phase 1 - Einführung GitHub__

  - Mechanismen zur Synchronisation von Dokumenten, Abläufe in GitHub

* __Übung Github__

  - Alle Teilnehmer arbeiten an einer README.md Datei eines Projektes
  - Erklärung der Unterschiede zum Etherpad
  - Explizite Formatierung mit Markdown, Nachvollziehbarkeit der Veränderungen,
  - Einbettung in Entwicklungsumgebung


## Quellen

* __Projekt-Website:__ https://LiaScript.github.io
* __Open-Source:__ https://github.com/liascript
* __YouTube:__ https://www.youtube.com/channel/UCyiTe2GkW_u05HSdvUblGYg
* __Wieteres:__

  - Dokumentation: https://github.com/LiaScript/docs
  - Bücher: https://github.com/topics/liascript-course
  - Templates: https://github.com/topics/liascript-template
  - Talks & ...: https://github.com/LiaPlayground
  - Blog: https://aizac.herokuapp.com

* __Editor:__

  - Atom: https://atom.io

    - Liascript-Preview: https://atom.io/packages/liascript-preview
    - Liascript-Snippets: https://atom.io/packages/liascript-snippets

  - VSCode: https://code.visualstudio.com/Download

    - LiaScript-Preview: https://marketplace.visualstudio.com/items?itemName=LiaScript.liascript-preview
    - LiaScript-Snippets: https://marketplace.visualstudio.com/items?itemName=LiaScript.liascript-snippets

* __Development-Server:__ https://www.npmjs.com/package/@liascript/devserver

* __Exporter:__ https://www.npmjs.com/package/@liascript/exporter

## Git & GitHub

Quellen:

- Pro Git book (2te Ausgabe) - _Ben Straub_
- online (deutsche Ausgabe): https://git-scm.com/book/de/v2


### Fachsprache & Fachchinesisch

     {{1}}
* ___git___

  - dezentrales Versionsmanagement System, entwickelt von [Linus Torvalds](https://de.wikipedia.org/wiki/Linus_Torvalds)
  - speichert die gesamte Historie eines Projektes
  - ermöglicht kooperatives Arbeiten mehrer Autoren
  - Download: https://git-scm.com/downloads

     {{2}}
* ___GitHub___

  - Platform für die Versionsverwaltung
  - Erweitert git um: __Reviews__, __Projekt-Management__, __Bug-Reports__, etc.
  - online: https://github.com
  - Wikipedia: https://de.wikipedia.org/wiki/GitHub

     {{3}}
* ___repository___ (___repo___)

  - das eigentliche Projekt
  - enthält alle Versionen und Entwicklungs-Zweige (branches)

     {{4}}
* ___fork^*^___

  - Kopie eines fremden ___Repositories___
  - Ziel: eigene Weiterentwicklung oder Zuarbeit

  ---

  <!-- style="max-width: 60rem" -->
  ``` ascii
  GitHub

  .----------------------.        fork        .---------------------.
  |                      |------------------->|                     |
  |   Main Repository    |                    | Personal Repository |
  |                      |<-------------------|                     |
  '----------------------'    pull request    '---------------------'
  ```

     {{5}}
* ___clone___

  - lokale Kopie eines ___Repositories___

  ---

  <!-- style="max-width: 60rem" -->
  ``` ascii
  GitHub

  .----------------------.        fork        .---------------------.
  |                      +------------------->|                     |
  |   Main Repository    |                    | Personal Repository |
  |                      |<-------------------+                     |
  '----------------------'    pull request    '--+------------------'
                                                 | clone          ^
  ---------------------------------------------- |           push |
  Local Machine                                  | pull           |
                                                 v                |
  .---------------------------------------------------------------+-.
  |                                                                 |
  |                            local files                          |
  |                                                                 |
  '-----------------------------------------------------------------'
  ```

     {{6}}
* ___pull___

  - Heruntladen/herunterziehen der Versionen aus einem entfernten ___repo___
  - (meist auf GitHub)

     {{7}}
* ___push___

  - Hochladen der lokalen Versionen zu einem entfernten ___repo___
  - (meinst auf GitHub)

     {{8}}
* ___pull request^*^___

  - Höfliche Anfrage der Übernahme von Änderungen

     {{9}}
* ___branch___

  - Verschiedene Entwicklungs-Zweige
  - Namensgebung: (beliebig aber ...)

    - `main`: Projekt (__Nur funktionierende Versionen__)
    - `develop`: Hauptentwicklungszweig
    - `test`: Test-Zweig für unsere Arbeit nicht nötig
    - `feat/Irgendwas`: kleine Erweiterungen


  <!-- style="max-width: 60rem" -->
  ``` ascii
  GitHub

  .----------------------.        fork        .---------------------.
  |                      +------------------->|                     |
  |   Main Repository    |                    | Personal Repository |
  |                      |<-------------------+                     |
  '----------------------'    pull request    '--+------------------'
                                                 | clone          ^
  ---------------------------------------------- |           push |
  Local Machine                                  | pull           |
                                                 v                |
  .---------------------------------------------------------------+-.
  |                                                                 |
  |  (main) *---*---*-----*----------------------------*-----*      |
  |              \       /                            /             |
  |  (develop)    o-----o--------o-----o--------o----o              |
  |                      \      /       \      /                    |
  |                       #----#         #----#                     |
  |                      (feat-1)       (feat-2)                    |
  '-----------------------------------------------------------------'
  ```

     {{10}}
* ___commit___

   - Hinzufügen einer neuen Version


     {{11}}
* ___checkout___

  - "auschecken" oder springen zu einem Zweiges oder einer Version

     {{12}}
* ___merge___

  - Übernehmen der Änderungen aus einem ___branch___ in einen anderen


### Setup Entwicklungsumgebung

1. Download und Installation von Atom: https://atom.io
2. Installation von PlugIns:

   - [LiaScript-Preview](https://atom.io/packages/liascript-preview)
   - [LiaScript-Snippets](https://atom.io/packages/liascript-snippets)
   - [Markdown-Table-Editor](https://github.com/susisu/atom-markdown-table-editor)

---

1. Download und Installation von VSCode: https://code.visualstudio.com/Download
2. Installation von PlugIns:

   - [LiaScript-Preview](https://marketplace.visualstudio.com/items?itemName=LiaScript.liascript-preview)
   - [LiaScript-Snippets](https://marketplace.visualstudio.com/items?itemName=LiaScript.liascript-snippets)

    {{1}}
> # Wichtige Tastenkombination:
>
> * Fuzzy Suche: <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>P</kbd>
> * Speichern: <kbd>Shift</kbd> + <kbd>S</kbd>
> * Verschieben von Zeilen: <kbd>Ctrl</kbd> + <kbd>ᐃ/ᐁ</kbd>
> * __LiaScript__:
>
>   - Snippets: <kbd>l</kbd> <kbd>i</kbd> <kbd>a</kbd>
>   - Programmiersprachen: <kbd>h</kbd> <kbd>i</kbd> <kbd>l</kbd> <kbd>i</kbd>
>   - Stimmen: <kbd>v</kbd> <kbd>o</kbd> <kbd>i</kbd> <kbd>c</kbd> <kbd>e</kbd>

## Teilen von Kursen via ...

**`https://LiaScript.github.io/course/?YOUR_COURSE_URL`**


    {{1}}
* [GitHub](https://github.com)
* [GitLab](https://gitlab.com)

    {{2}}
* [DropBox](https://DropBox.com)
* [nextCloud](https://nextCloud.com)

    {{3}}
* [Brave Browser](https://brave.com) via [IPFS](https://ipfs.io)
* [Beaker Browser](https://beakerbrowser.com) via [Hyper](https://hypercore-protocol.org)

  !?[Beaker-Browser demo](https://beakerbrowser.com/beaker-site-demo.mp4)<!-- autoplay="true" -->

* [Onion-Share](https://onionshare.org)

    {{4}}
* freier Webspace
* [CodiLia](https://github.com/liaScript/codilia)


## Markdown Tutorial

### Philosophy

> ~~__Markdown is intended to be as easy-to-read and easy-to-write as is feasible.__~~
>
> Readability, however, is emphasized above all else. A Markdown-formatted document ~~__should be publishable as-is__~~, as plain text, without looking like it’s been marked up with tags or formatting instructions. While Markdown’s syntax has been influenced by several existing text-to-HTML filters — including Setext, atx, Textile, reStructuredText, Grutatext, and EtText — the single ~~__biggest source of inspiration__~~ for Markdown’s syntax is the format of ~~__plain text email__~~.
>
>To this end, Markdown’s syntax is comprised entirely of punctuation characters, which ~~__punctuation characters have been carefully chosen so as to look like what they mean__~~. E.g., asterisks around a word actually look like \*emphasis\*. Markdown ~~__lists look like, well, lists__~~. Even ~~__blockquotes look like quoted passages of text__~~, assuming you’ve ever used email.
>
> -- by [John Gruber](https://daringfireball.net/projects/markdown/syntax#philosophy)

### Dialekte

### Grundlagen

> Blöcke werden "optisch" durch Leerzeilen voneinander getrennt

#### 1. Absätze und Formatierungen

#### 2. Listen

#### 3. Blockquotes

#### 4. Tabellen

#### 5. Verweise

#### 6. Bilder

#### 7. Trennlinien

#### 8. Code

#### 9. HTML

Übersicht über alle HTML-Tags: https://www.w3schools.com/TAgs/default.asp

##### `<details>` & `<summary>`

<details style="background: #EEE">

<summary>**Honest Textbook ads (click to enlarge)**</summary>

https://www.youtube.com/watch?v=lhSjYT7pWkw

</details>

##### `<lia-keep>`

## LiaScript Tutorial

### Multimedia

Verweis -> !Bild --> ?Audio --> !?Video --> ??Unbekannt

#### Bilder und Texte


#### Formatierung

<!-- style="color: red; font-size: 4rem; max-width: 400px" -->
Blöcke<!-- style="background: green" --> und einzelne Elemente<!-- style="border: 3px dashed blue" --> können unterschiedlich formatiert werden!

> Merke: Kommentare __vor__ dem Block und __hinter__ dem Element.
>
> Siehe auch: [W3Schools](https://www.w3schools.com/Css/css_colors.asp)

##### Nützliche Stile

* Schriftfarbe:
  `color: red` oder `color: #FF0000` oder `color: rgb(1,0,0)`
* Schriftgröße:
  `font-size: 4rem` oder `font-size: 3cm` oder `font-size: 20px`
* Maximale Höhe & Breite:
  `max-height: 300px` `max-widht: 300px`
* Minimale Höhe & Breite:
  `min-height: 300px` `min-widht: 300px`
* Tatsächliche Höhe & Breite:
  `width: 300px` oder `width: 50%` oder `ẁidth: 50vw`
* Ränder:
  `border: 2px solid black` oder `border: 2px dashed black`
* Abstände:
  `padding: 3px` oder `padding-top: ..` oder `padding-left`
  oder `margin: 3px` oder `margin-top: ..` oder `margin-left`

##### Kontrolle der Übersetzung

> Mithilfe von `class="translate"` oder `class="notranslate"` können Element markiert werden, die übersetzt bzw. nicht übersetzt werden sollen.

---

**Beispiel:**

```` markdown
<!-- class="notranslate" -->
Alle Code-Elemente werden automatisch mit der Klasse `notranslate` markiert.

<!-- class="translate" -->
``` javascript
console.log("Hello World")
```
````

### Metainformationen

### Präsentationsformate

Buch/Präsentation/Folien

``` markdown
    --{{0}}--
Ich bin ein Kommentar, der laut vorgelesen werden kann.

    --{{1}}--
Es ist möglich, Kommentare mit Animation zu verbinden.

      {{1}}
?[audio](https://bigsoundbank.com/UPLOAD/mp3/1068.mp3)


    --{{2}}--
Blöcke können auch wieder verschwinden.

     {{2-3}}
| Tabellen |      sind      | cool  |
|:-------- |:--------------:|:----- |
| rechts   |   zentriert    | links |
| :-)      | $ f(x) = x^2 $ | <-->  |

liatab

    --{{3 Ukrainan Female}}--
Первоначально создан в 2004 году Джоном Грубером (англ. John Gruber) и Аароном
Шварцем.
Многие идеи языка были позаимствованы из существующих соглашений по
разметке текста в электронных письмах...


    {{3}}
Oder die Sprache kann geändert werden. Tippe "voice" um
eine Auswahl der unterstützen Sprachen zu erhalten
```

#### Inline Animationen

Hallo {2}{Welt, } dies ein Absatz mit internen Animationen {1-2}{**die auch wieder verschwinden können**}.

#### Sprachen Lernen `|>` oder `!>`

#### Versteckte Kommentare

    --{{1}}--
Dieser Text ist besonders wichtiges Zitat.

      {{1}}
> “Live as if you were to die tomorrow.
> Learn as if you were to live forever.”
>
> -- Mahatma Gandhi

<!-- --{{1}}--
Lebe so als ob du morgen sterben würdest.
Lerne so als ob du für immer Leben würdest.
Von Mahatma Ghandi.
-->

### Formeln

Nutzung von [KaTeX](https://katex.org)

Funktionsübersich: https://katex.org/docs/supported.html

1. Inline Formeln: `$ ... $` --> $ f(a,b,c) = (a^2+b^2+c^2)^3 $
2. Block Formeln: `$$ ... $$`

   $$
      \sum_{i=1}^\infty\frac{1}{n^2}
           =\frac{\pi^2}{6}
   $$

#### Interaktive Formeln
<!--
@formula: <script>console.html(`<lia-formula formula="@'input" displayMode="true"></lia-formula>`);"LIA: stop"</script>

-->

Zentriert nach `=`

``` latex
\begin{split}
  a &=b+c \\
    &=e+f \\
    &=g+h+i+j\\
a+b+&c+d=12\\
\end{split}
```
@formula

Hinzufügen einer Nummer

``` latex
\tag{33}
\begin{equation}
 a =b+c
\end{equation}
```
@formula

Definition einer Matrix und Nutzung von HTML.

``` latex
\begin{Bmatrix}
   a & b & c & d & e & f \\
   g & h & i & j & k & l \\
   m & n & o & p & q & r \\
   s & t & u & v & w & x \\
   y & z & ä & ö & ü &
   \htmlStyle{color: red; font-size: 26px}{ß}
\end{Bmatrix}
\\
\href{https://katex.org/docs/supported.html#html}{\KaTeX HTML support}
\\
\includegraphics[height=0.8em, totalheight=0.9em, width=0.9em, alt=KA logo]{https://katex.org/img/khan-academy.png}
```
@formula

### Quizzes

### Umfragen

### Aufgaben/Tasks

### Bemerkung zu Versionen



### Klassenräume

### Zeichnen mit ASCII-Art

#### Diagramme

                                    Multiline
    1.9 |    DOTS
        |                 ***
      y |               *     *
      - | r r r r r r r*r r r r*r r r r r r r
      a |             *         *
      x |            *           *
      i | B B B B B * B B B B B B * B B B B B
      s |         *                 *
        | *  * *                       * *  *
     -1 +------------------------------------
        0              x-axis               1

#### Code als Bild

Dokumentation: https://github.com/andre-dietrich/elm-svgbob

```` ascii
  .-----.
  |.---.|
  ||   ||  device
  |.___.|  loads
  | ooo |----+--------------------------+--------------------------.
  | ooo |    |                          |                          |
  | ooo |    |                          |                          |
  '_____'    |                          |                          |
             |                          |                          |
             v                          v                          v
   +-------------------+  .---------------------------.  +-------------------+
   | Loadable module C |  |     Loadable module A     |  | Loadable module B |
   +---------+---------+  |---------------------------|  |   (instrumented)  |
             |            |         .-----.           |  +----------+--------+
             '--------------------> | A.o |           |             |
                 calls    |         '-----'           |             |
                          |    .------------------.   |             |
                          |   / A.instrumented.o / <----------------'
                          |  '------------------'     |    calls
                          '---------------------------'
````



````````````````````````````````
  ┌─┬┐  ╔═╦╗  ╓─╥╖  ╒═╤╕
  │ ││  ║ ║║  ║ ║║  │ ││
  ├─┼┤  ╠═╬╣  ╟─╫╢  ╞═╪╡
  └─┴┘  ╚═╩╝  ╙─╨╜  ╘═╧╛
  ┌───────────────────┐
  │  ╔═══╗ Some Text  │▒
  │  ╚═╦═╝ in the box │▒
  ╞═╤══╩══╤═══════════╡▒
  │ ├──┬──┤           │▒
  │ └──┴──┘           │▒
  └───────────────────┘▒
   ▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒
````````````````````````````````


#### Weiteres



### Spaß mit Tabellen


## Erweiterungen

### Wo finde ich Erweiterungen

https://github.com/topics/liascript-template

 <a href="https://www.w3schools.com/" target="_parent" rel="noopener noreferrer">Visit W3Schools!</a>

### Wie erstelle ich eigene Erweiterungen


## Export zu anderen Formaten

1. Download von [NodeJS](https://de.wikipedia.org/wiki/Node.js):
   https://nodejs.org/de/download/

2. Download des LiaScript-Exporters:
   https://www.npmjs.com/package/@liascript/exporter


## Ein Ausblick: JavaScript

Das Quadrat von
<script output="x" input="range" value="1" min="0" max="1000" step="0.1">
@input
</script>
ist gleich ==>
<script> @input(`x`) * @input(`x`)</script>

### Tabellen und Code
<!--
sin: <script format="number"
             localeStyle="currency"
             currency="EUR"
             locale="de-DE"
             modify="false"
    > Math.sin(@input(`result`) + @input(`amp`) * @0) </script>
-->

Pos: <script run-once
        default="0"
        output="result"
        input="range" value="2" min="0" max="25" step="0.1"
        >
@input
</script>
and amplitude:
<script run-once
        default="0"
        output="amp"
        input="range" value="1" min="0" max="2" step="0.1"
        >
@input
</script>


<!-- data-type="barchart" id="tabelle" -->
| Header 1 | <script>@input(`result`)</script> |
|:-------- |--------: |
| 1        | @sin(1)  |
| 2        | @sin(2)  |
| 3        | @sin(3)  |
| 4        | @sin(4)  |
| 5        | @sin(5)  |
| 6        | @sin(6)  |
| 7        | @sin(7)  |
| 8        | @sin(8)  |
| 9        | @sin(9)  |


### Diagramme

The first value defines some kind of range:
<script input="range" value="2" output="range">@input</script>
, while the second can be interpreted as range
<script input="range" value="50" output="amplitude">@input</script>.
You can double-click on any gray element to inspect and edit its javascript code.


<script run-once style="display: inline-block; width: 100%">
function func(x) {
    x /= 10;
    return Math.sin(x) * Math.cos(x * @input(`range`) + 1) * Math.sin(x * 3 + 2) * @input(`amplitude`);
}

function generateData() {
    let data = [];
    for (let i = -200; i <= 200; i += 0.1) {
        data.push([i, func(i)]);
    }
    return data;
}

let option = {
    animation: false,
    grid: {
        top: 40,
        left: 50,
        right: 40,
        bottom: 50
    },
    xAxis: {
        name: 'x',
        minorTick: {
            show: true
        },
        splitLine: {
            lineStyle: {
                color: '#999'
            }
        },
        minorSplitLine: {
            show: true,
            lineStyle: {
                color: '#ddd'
            }
        }
    },
    yAxis: {
        name: 'y',
        min: -100,
        max: 100,
        minorTick: {
            show: true
        },
        splitLine: {
            lineStyle: {
                color: '#999'
            }
        },
        minorSplitLine: {
            show: true,
            lineStyle: {
                color: '#ddd'
            }
        }
    },
    dataZoom: [{
        show: true,
        type: 'inside',
        filterMode: 'none',
        xAxisIndex: [0],
        startValue: -20,
        endValue: 20
    }, {
        show: true,
        type: 'inside',
        filterMode: 'none',
        yAxisIndex: [0],
        startValue: -20,
        endValue: 20
    }],
    series: [
        {
            type: 'line',
            showSymbol: false,
            clip: true,
            data: generateData()
        }
    ]
}

"HTML: <lia-chart option='" + JSON.stringify(option) + "'></lia-chart>"

</script>
