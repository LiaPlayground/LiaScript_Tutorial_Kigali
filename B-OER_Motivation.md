<!--
author:   Sebastian Zug, André Dietrich

email:    Sebastian.Zug@informatik.tu-freiberg.de

version:  0.0.1

language: de

narrator: Deutsch Male

mode:     Presentation

comment:  This course discusses the applicability of OER concepts on learning
          materials designed with LiaScript.

logo:     ./images/logo.png

translation: Deutsch  translations/German.md

-->

[![LiaScript](https://raw.githubusercontent.com/LiaScript/LiaScript/master/badges/course.svg)](https://LiaScript.github.io/course/?https://raw.githubusercontent.com/LiaPlayground/LiaScript_Tutorial_Kiel/main/B-OER_Motivation.md)

# A) Vision and challenges of Open Educational Ressources (OER)

![OER logo](images/Global_Open_Educational_Resources_Logo.png "OER-Logo - Quelle: Jonathasmello - Eigenes Werk, CC BY 3.0, [https://commons.wikimedia.org/w/index.php?curid=18460156](https://commons.wikimedia.org/w/index.php?curid=18460156)")

This presentation illustrates the vision of _Open Educational Ressources_ and its application on LiaScript. The document was used during a tutorial at eLearning Africa on 10th Mai 2022.

_The sources of the presentation can be found at [Link](https://github.com/LiaPlayground/LiaScript_Tutorial_Kigali/blob/main/B-OER_Motivation.md) zu finden._

------------------------------------------------------

Sebastian Zug, André Dietrich

Faculty of Mathematics and Computer Science

TU Bergakademie Freiberg

[sebastian.zug@informatik.tu-freiberg.de](mailto:sebastian.zug@informatik.tu-freiberg.de)

------------------------------------------------------

## Starting point

> {0-5}{Teachers want to realize motivating, interactive teaching materials.}

             {{1-2}}
********************************************************************************

---------------------

Beispiele:


- [[male (der)] (female [die]) [neuter (das)]]
- [    [X]           [ ]             [ ]     ]  Mann - German for man
- [    ( )           (X)             ( )     ]  Frau - German for woman

---------------------

??[ear model](https://sketchfab.com/3d-models/ear-anatomy-468e2039bde34a3fabb9e90bff9cd56b)

********************************************************************************


            {{2-5}}
********************************************************************************
- __Strategy strategy 1__: I do everything myself

  + The teacher has to think about all the content herself/himself
  + The teacher has to face significant technical challenges


********************************************************************************


{{3-5}}
********************************************************************************

- __Solution strategy 2__: I use materials from other teachers.

    + The optimal alignment with my own didactic goals is missing.

********************************************************************************

{{4-5}}
********************************************************************************

> Obviously, hybrid approaches - use and adaptation - are required! Can these requirements be further specified?

********************************************************************************

## OER as a game changer?

>  **Open Courseware / Open Educational Resources** ... teaching, learning and
> research materials in any medium, digital or otherwise,that reside in the
> **public domain** or have been released under an open license that permits
> no-cost access, use, **adaptation** and **redistribution** by others with no or 4
> limited restrictions. Open licensing is built within the existing framework of
> intellectual property rights as defined by relevant international conventions
> and respects the authorship of the work
>
> -- UNESCO 2002 Forum on the Impact of Open Courseware for Higher Education in Developing Countries [(Link)](https://unesdoc.unesco.org/ark:/48223/pf0000128515)

           {{0-1}}
********************************************************************************

| requirement       | meaning                          |
| ----------------- | -------------------------------- |
| `storing/copying` | downloading, storing and copying |
| `use`             | use in learning context          |
| `process`         | transformation                   |
| `adapting/mixing` | extraction and combination       |
| `disseminate`     | (digital) publication            |

*_Definition of OER according to 5V Modell described by Jöran Muuß-Merholz und Jörg Lohrer für [open-educational-ressources](https://open-educational-resources.de)_*

> _OER can be the trigger for innovation and new forms of learning in the 21st century._
>
> -- Translation from _Handreichung OER - Der Einstieg in den Umgang mit Open Educational Ressources_, Bericht des Projektes OERsax, 2018

********************************************************************************


### Perfect OER Material - a text file

<!--
style="width: 100%; max-width: 860px; display: block; margin-left: auto; margin-right: auto;"
-->
```ascii

Version 1.0                           Version 1.1
+---------------------------+          +---------------------------+
| Course  German Literatur  |          | Course  German Literature |
| Authors John Muster       | "Error"  | Authors John Muster       |
|                           |------->  |         Angelika Maier    |----->
|~~~~~~~~~~~~~~~~~~~~~~~~~~~|          |~~~~~~~~~~~~~~~~~~~~~~~~~~~|
| In 1756 Goethe visited    |---.      | In 1786 Goethe visited    |--.
| Italy ...                 |   |      | Italy ...                 |  |
                                |                                     |
                                |                                     |    +----------------------------+
                                |                                     |    | Course  Deutsche Literatur |
                                |                                     |    | Authors John Muster        |
                                |                                     .--> |         Angelika Maier     |
                                |                                          |         Steve Gray         |
                                |                                          |~~~~~~~~~~~~~~~~~~~~~~~~~~~~|
                                |                                          | 1786 reiste Goethe nach    |
                                |                                          | Italien ...                |
                                |       Version 1.0
                                |      +---------------------------+
                                |      | Course  Goethe & Schiller |
                                |      | Authors John Muster       |
                                .-->   |         Angelika Maier    |----->
                                       |~~~~~~~~~~~~~~~~~~~~~~~~~~~|
                                       | The correspondence during |
                                       | the Italian journey ...   |
```
*Versions of the teaching content of a course and its reuse in other courses*.

{{0-1}}
********************************************************************************

| requirement       | txt |                                                         |
| ----------------- | --- | ------------------------------------------------------- |
| `storing/copying` | ++  | advantageous because of small size                      |
| `use`             | ++  | analog / digital distribution to students uncomplicated |
| `process`         | ++  | processable without additional software                 |
| `adapting/mixing` | ++  | simple combination of text fragments via copy&paste     |
| `disseminate`     | ++  | easily exportable                                       |

> **A pure text file can cover all ideas of OER? Obviously our list of requirements is not complete.**

********************************************************************************

{{1-2}}
********************************************************************************

he 5V definition ...

> _1. ... focuses on the Open in OER but leaves aside the Education._
>
> _2. ... ignores the need for a version management system.
>
> _3. ... does not consider the findability of OER content._

| requirement                                   | txt                           |                                                         |
| --------------------------------------------- | ----------------------------- | ------------------------------------------------------- |
| `storing/copying`                             | ++                            | advantageous because of small size                      |
| `use`                                         | +                             | analog / digital distribution to students uncomplicated |
| `process`                                     | ++                            | processable without additional software                 |
| `adapting/mixing`                             | ++                            | simple combination of text fragments via copy&paste     |
| `disseminate`                                 | ++                            | easily exportable                                       |
| <!-- Style="color:green" --> manage / version | <!-- Style="color:red" --> ?? |                                                         |
| <!-- Style="color:green" --> motivate         | <!-- Style="color:red" --> -- | no contemporary formats and interactive content         |

> __Obviously, we need formats that cover the extended set of requirements in addition to the positive aspects of text representations.__

********************************************************************************

### Comparison with Wikipedia

> Can Wikipedia be the inspiration for OER?

| Aspect     | Wikipedia - Solution                                                             | Disadvantage                                                             |
| ---------- | -------------------------------------------------------------------------------- | ------------------------------------------------------------------------ |
| search     | one instance of an article directly retrievable                                  | no different expressions possible for one topic.                         |
| tools      | integrated editor based on a Markdown dialect                                    | strong limitation of possibilities to structured texts, formulas, images |
| quality    | sophisticated review system with experts, version data collection and comparison |                                                                          |
| visibility | authorship visible in version history                                            |                                                                          |

### OER in reality

                {{0-1}}
********************************************************************************

Types of files labeled with "OER" on TU Bergakademie's servers:

<!-- data-type="BarChart"
data-title="Anteil der Datenformate im Kontext der OPAL OER Materialien"
data-xlabel="Datentyp"
data-ylabel="% of Anzahl" -->
| Dateityp | Anzahl | ratio    |
| -------- | ------ | -------- |
| `pdf`    | 5242   | 0.494995 |
| `jpg`    | 1040   | 0.098206 |
| `mkv`    | 873    | 0.082436 |
| `mp4`    | 586    | 0.055335 |
| `png`    | 494    | 0.046648 |
| `zip`    | 443    | 0.041832 |
| `html`   | 387    | 0.036544 |
| `docx`   | 376    | 0.035505 |
| `pptx`   | 245    | 0.023135 |
| `xlsx`   | 191    | 0.018036 |


The materials in OPAL come predominantly without licenses and as closed file format. A reuse is accordingly only with difficulty possible.

********************************************************************************

                 {{1-2}}
********************************************************************************


| Level                               | Core Statement                                                                   |
| ----------------------------------- | -------------------------------------------------------------------------------- |
| Emotional classification            | "_Everyone can use my work for themselves!_"                                     |
|                                     | "_Anyone can control me!_"                                                       |
| Legal Challenges                    | "_I use a lot of graphics whose copyright I am unsure of at best!_"              |
| Findability                         | "_I can't find content that I can profitably integrate into my teaching!_"       |
| <!-- Style="color:red" --> Effort   | <!-- Style="color:red" --> "_You must have studied computer science!_"           |
| <!-- Style="color:red" --> Coverage | <!-- Style="color:red" --> "_But there are missing interfaces for my tools XY!_" |


## LiaScript Vision

OER Materials must ...

> 1. be transformable to enable reuse. (_Process/Use/Disseminate_).
> 2. contain metadata to be discoverable. (_Disseminate_)
> 3. embed an systematic version history (_Manage_).

<!--
style="width: 100%; max-width: 860px; display: block; margin-left: auto; margin-right: auto;"
-->
```ascii
   +---------------------+
   | # Digital Systeme V1|\
 +--------------------+  +-+
 | # Digital Systeme  |\
+------------------+  +-+
| # Digital Systems|\                                      .-----------.
| (SoSe 2021)      +-+                              ╔══════|   LMS  X  |══════╗
|                    |  --------------------------> ║      '-----------'      ║
| ## Task 1          |                              ║ Digital Systems 2021    ║
|                    |                              ║                         ║
| + Implement ...    | --------------+              ║ import numpy as np      ║
|                    |    Trans-     |              ║ ...                     ║
|                    |    formation  |              ╚═════════════════════════╝
+--------------------+               v
                                .-,(   ),-.                .-----------.
License: ...                 .-(           )-.      ╔══════|   LMS  Y  |══════╗
Content: ...                (    OER Cloud    )     ║      '-----------'      ║
Author: ...                  '-(           )-'  +-->║ Digital Systems 2021    ║
Versions: ...                   '-.(   ).-'     |   ║                         ║
                                     |          |
                                     +----------+          .-----------.
                                                |   ╔══════|  Webapp   |══════╗
                                                |   ║      '-----------'      ║
                                                +-->║ Digital Systems 2021    ║
                                                    ║                         ║

```
*Transformation of OER materials for use in various LMSs.*


### Experiences with the use of OER

-> Course overview of the _Software Development and Robotics_ working group on [GitHub](https://github.com/TUBAF-IfI-LiaScript).

Results:

1. a "we" idea emerges from collaboration on materials in the context of a core team.
2. bugs are weeded out much faster than in years past. "Short-term" quality increases.
3. interaction between teachers and students increases - *"Shouldn't we explain it better this way... "*.
4. the understanding about distributed development develops very positively, even the non-computer science students are able to deal with the methods.
