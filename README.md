[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://www.webcomponents.org/element/owner/my-element)

# \<audio-player\>

simple audio player.  
This is playing with web audio api.  
Just write the path to the sound file and you can play it.

## DEMO

<!--
```html
<custom-element-demo>
  <template>
    <script src="../webcomponentsjs/webcomponents-lite.js"></script>
    <link rel="import" href="audio-player.html">
    <next-code-block></next-code-block>
  </template>
</custom-element-demo>
```
-->
```html
<audio-player src="./demo/sound.mp3" volume="5" button></audio-player>
```

## Installation

```
$ bower install --save monkick/audio-player
```

## Usage

At first. Import it at header.  

```html
    <link rel="import" href="../bower_components/audio-player/audio-player.html">
```

Next. Add the `audio-player` custom tag in body.

```html
    <audio-player src="./demo/sound.mp3" volume="5" button></audio-player>
```

* src: path of sound file
* volume: Volume range 1 to 10
* button: Add button argument that button will appear for play sound file. If you want control myself than you can see demo/index.html.

## Event

* onend: It fire when audio is over.

## Parameter

* `control`: appear control ui.
* `analyze`: appear svg of analyze to sound. 

## Method

* `_play`: play sound.
* `_stop`: stop sound.
* `_silent`: play silent sound. For sound from iOS.