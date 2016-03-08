---
layout: app
title: App
permalink: /app/
---
<script src="app.js"></script>
<center>
<div>
# moveServos
<input type="range" id="neck" min="0" max="180" value="90" step="5" onchange="setNeck(this.value)"/> Neck<br>
<input type="range" id="left"  min="0" max="180" value="90" step="5" onchange="setLeft(this.value)"/> Left<br>
<input type="range" id="right" min="0" max="180" value="90" step="5" onchange="setRight(this.value)" /> Right<br>


# moodlights
<input type="range" id="red" min="0" max="255" value="0" step="5" onchange="setRed(this.value)"/> Red<br>
<input type="range" id="green"  min="0" max="255" value="0" step="5" onchange="setGreen(this.value)"/> Green<br>
<input type="range" id="blue" min="0" max="255" value="0" step="5" onchange="setBlue(this.value)" /> Blue<br>

# playSound
<input type="range" id="sound" min="0" max="255" value="0" step="5" onchange="callFunction('playSound', this.value)"/> Volume<br>

<div onclick="setInterval(getNoise, 2500);
setInterval(getBrightness, 2500);">
<h1 id="noiselevel">noise</h1>
<h1 id="brightnesslevel">brightness</h1>
</div>

</div>
</center>