[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://www.webcomponents.org/element/monkick/audio-player)

# \<audio-player\>

simple audio player.  
This is playing with web audio api.  
Just write the path to the sound file and you can play it.

## Version
1.8.0

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
    <link rel="import" href="../bower_components/scatter-menu/scatter-menu.html">
    <link rel="import" href="../bower_components/scatter-menu/scatter-menu-item.html">
```

Next. Add the `scatter-menu` custom tag in body.

```html
    <scatter-menu id="menu" row="3" col="3">
        <scatter-menu-item menu-title="menu01" menu-order="1" menu-space="80"></scatter-menu-item>
        <scatter-menu-item menu-title="menu02" menu-order="2" menu-space="80"></scatter-menu-item>
        <scatter-menu-item menu-title="menu03" menu-order="3" menu-space="80"></scatter-menu-item>
        <scatter-menu-item menu-title="menu04" menu-order="1" menu-space="80" menu-column="2"></scatter-menu-item>
        <scatter-menu-item menu-title="menu05" menu-order="2" menu-space="80" menu-column="2"></scatter-menu-item>
        <scatter-menu-item menu-title="menu06" menu-order="3" menu-space="80" menu-column="2"></scatter-menu-item>
        <scatter-menu-item menu-title="menu07" menu-order="1" menu-space="80" menu-column="3"></scatter-menu-item>
        <scatter-menu-item menu-title="menu08" menu-order="2" menu-space="80" menu-column="3"></scatter-menu-item>
        <scatter-menu-item menu-title="menu09" menu-order="3" menu-space="80" menu-column="3"></scatter-menu-item>
    </scatter-menu>
```

* src: path of sound file
* volume: Volume range 1 to 10
* button: Add button argument that button will appear for play sound file. If you want control myself than you can see demo/index.html.

## Event

* onend: It fire when audio is over.

## Parameter

* `control`: appear control ui.
* `analyze`: appear svg of analyze to sound.
* `type`: form of analyze svg. set to `line` or `circle`.
* `loop`: can loop play.


## Method

* `_play`: play sound.
* `_stop`: stop sound.
* `_silent`: play silent sound. For sound from iOS.