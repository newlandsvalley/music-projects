Summary of Music Projects
=========================

PureScript
----------


| Name                       | Description                                        |
| -----------------------    | -------------------------------------------------- |
| [purescript-abc-editor](https://github.com/newlandsvalley/purescript-abc-editor)   | edit, play and see scores of tunes in ABC notation    |
| [purescript-abc-tutorial](https://github.com/newlandsvalley/purescript-abc-tutorial)    | learn ABC by means of an interactive tutorial    |
| [polyphonic-abc-player](https://github.com/newlandsvalley/purescript-school-of-music/tree/master/polyphonic-player) | play ABC scores that have multiple voices |
| [purescript-school-of-music](https://github.com/newlandsvalley/purescript-school-of-music) | (PSoM) port of the Haskell School of Music |
| [MIDI keyboard player](https://github.com/newlandsvalley/purescript-midi-keyboard)            | play a MIDI keyboard through the browser  |
| [polska-metronome](https://github.com/newlandsvalley/polska-metronome)            | 3/4 metronome with irregular beats |
| [chord-editor](https://github.com/newlandsvalley/chord-editor)            | edit guitar chord diagrams |
| [tunebook](https://github.com/newlandsvalley/tunebook)  | quick and dirty generation of a booklet of scores |
| [tunebank-frontend](https://github.com/newlandsvalley/tunebank-frontend)            | UI to musicrest |
| [purescript-audiograph](https://github.com/newlandsvalley/purescript-audiograph)            | declarative interface into web-audio  |


All these projects run in the browser, and use web-audio to generate sound. All the projects use Halogen as the UI framework although legacy Pux versions exist for some of them. __tunebank-frontend__ incorporates all the ABC utilities. The last project is an experiment built solely around purescript-webaudio. Most of the projects share various libraries whose interdependencies are quite complex and are shown below. Libraries at the end of the dependency chain such as the ABC editor, tutorial, PSOM editor and polyphonic player also exist as independent projects for the browser.

![dependencies](https://github.com/newlandsvalley/music-projects/blob/master/library-dependencies.jpg)

The audio libraries include:


| Name                             | Description                                        |
| -------------------------------- | -------------------------------------------------- |
| [soundfonts](https://github.com/newlandsvalley/purescript-soundfonts) | play notes using web-audio soundfonts              |
| [midi](https://github.com/newlandsvalley/purescript-midi)                  | General MIDI, Web-MIDI and MIDI instruments                  |
| [abc-parser](https://github.com/newlandsvalley/purescript-abc-parser)            | parser for the ABC notation                        |
| [abc-scores](https://github.com/newlandsvalley/purescript-abc-scores)                | generate music scores using VexFlow                 |
| [abc-melody](https://github.com/newlandsvalley/purescript-abc-melody) | convert ABC directly to a monophonic soundfont melody |
| [rhythm-guitar](https://github.com/newlandsvalley/rhythm-guitar) | play ABC chord symbols as if on an acoustic guitar |
| [abc2psom](https://github.com/newlandsvalley/purescript-abc2psom) | convert ABC to a polyphonic PSoM melody |
| [halogen-components](https://github.com/newlandsvalley/purescript-halogen-components)               | various components including a generic player  |

Note that these libraries are for use in the browser and are not available for Node. Note also that there are two alternative mechanisms for playing an ABC melody.  You can use abc-melody (with optional guitar chords) or you can convert the ABC to PSOM format with abc2psom and use the PSOM player.  The former only allows for monophonic melodies, the latter allows for polyphony.

Earlier versions of the projects used Pux exclusively under PureScript 0.11. These used a base [purescript-soundfont-player](https://github.com/newlandsvalley/purescript-soundfont-player) with two specialised players - [purescript-midi-player](https://github.com/newlandsvalley/purescript-midi-player) and [purescript-psom-player](https://github.com/newlandsvalley/purescript-psom-player) built by wrapping the base soundfont player.


Elm
---

Much of the same ground is covered in the Elm projects.  However, these are now long in the tooth, having been written for Elm 0.18. They are no longer being actively maintained (in favour of the purescript implementations) and most have been archived.

Scala
-----

[musicrest](https://github.com/newlandsvalley/musicrest) is the backend for [tradtunedb](http://www.tradtunedb.org.uk/).

Haskell
-------

| Name                             | Description                                        |
| -------------------------------- | -------------------------------------------------- |
| [MidiToAbc](https://github.com/newlandsvalley/MidiToAbc) | An attempt to convert a monophonic MIDI melody into the ABC notation. |
| [Tunebank](https://github.com/newlandsvalley/tunebank) | An experimental rewrite of musicrest using [Servant](https://www.servant.dev/) and Postgresql. |