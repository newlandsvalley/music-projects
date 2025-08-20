Summary of Music Projects
=========================

PureScript
----------


| Name                       | Description                                        |
| -----------------------    | -------------------------------------------------- |
| [purescript-abc-editor](https://github.com/newlandsvalley/purescript-abc-editor)   | edit, play and see scores of tunes in ABC notation    |
| [purescript-abc-tutorial](https://github.com/newlandsvalley/purescript-abc-tutorial)    | learn ABC by means of an interactive tutorial    |
| [share-a-tune](https://github.com/newlandsvalley/share-a-tune) | play (possibly polyphonic) ABC scores and share them |
| [purescript-school-of-music](https://github.com/newlandsvalley/purescript-school-of-music) | (PSoM) port of the Haskell School of Music |
| [MIDI keyboard player](https://github.com/newlandsvalley/purescript-midi-keyboard)            | play a MIDI keyboard through the browser  |
| [polska-metronome](https://github.com/newlandsvalley/polska-metronome)            | 3/4 metronome with irregular beats |
| [chord-editor](https://github.com/newlandsvalley/chord-editor)            | edit chord diagrams |
| [tunebook](https://github.com/newlandsvalley/tunebook)  | quick and dirty generation of a booklet of scores |
| [tunebank-node](https://github.com/newlandsvalley/tunebank-node)            | A tune store for ABC |
| [tunebank-frontend-for-node](https://github.com/newlandsvalley/tunebank-frontend-for-node)            | UI to tunebank-node |
| [purescript-audiograph](https://github.com/newlandsvalley/purescript-audiograph)            | declarative interface into web-audio  |


All these projects run in the browser, and use web-audio to generate sound. All the projects use Halogen as the UI framework although legacy Pux versions exist for some of them. __tunebank-frontend-for-node__ incorporates all the ABC utilities. The last project is an experiment built solely around purescript-webaudio. The first four projects share various libraries whose interdependencies are shown below. 

![dependencies](https://github.com/newlandsvalley/music-projects/blob/master/ps-dependencies.jpg)

The audio libraries include:


| Name                             | Description                                        |
| -------------------------------- | -------------------------------------------------- |
| [purescript-soundfonts](https://github.com/newlandsvalley/purescript-soundfonts) | play notes using web-audio soundfonts              |
| [purescript-midi](https://github.com/newlandsvalley/purescript-midi)                  | General MIDI, Web-MIDI and MIDI instruments                  |
| [purescript-abc-parser](https://github.com/newlandsvalley/purescript-abc-parser)            | parser for the ABC notation                        |
| [purescript-abc-scores](https://github.com/newlandsvalley/purescript-abc-scores)                | generate music scores using VexFlow                 |
| [purescript-abc-melody](https://github.com/newlandsvalley/purescript-abc-melody) | convert ABC directly to a monophonic soundfont melody |
| [purescript-abc2psom](https://github.com/newlandsvalley/purescript-abc2psom) | convert ABC to a polyphonic PSoM melody |
| [purescript-halogen-components](https://github.com/newlandsvalley/purescript-halogen-components)               | various components including a generic player  |

Note that these libraries are for use in the browser and are not available for Node.

Earlier versions of the projects used Pux exclusively under PureScript 0.11. These used a base [purescript-soundfont-player](https://github.com/newlandsvalley/purescript-soundfont-player) with two specialised players - [purescript-midi-player](https://github.com/newlandsvalley/purescript-midi-player) and [purescript-psom-player](https://github.com/newlandsvalley/purescript-psom-player) built by wrapping the base soundfont player.


Elm
---

Much of the same ground is covered in the Elm projects.  However, these are now long in the tooth, having been written for Elm 0.18. They are no longer being actively maintained (in favour of the purescript implementations) and most have been archived.

Scala
-----

[musicrest](https://github.com/newlandsvalley/musicrest) is the backend for [tradtunedb](http://www.tradtunedb.org.uk/). This is now deprecated in favour of tunebank-node.

Haskell
-------

| Name                             | Description                                        |
| -------------------------------- | -------------------------------------------------- |
| [MidiToAbc](https://github.com/newlandsvalley/MidiToAbc) | An attempt to convert a monophonic MIDI melody into the ABC notation. |
| [Tunebank](https://github.com/newlandsvalley/tunebank) | An experimental rewrite of musicrest using [Servant](https://www.servant.dev/) and Postgresql. |