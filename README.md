reveal-videoplayer
==================

Plugin for [reveal.js](http://revealjs.com/) &mdash; starts a &lt;video&gt; once the slide appears

## Installation

Just copy reveal-videoplayer.js into your plugin directory and include it in your reveal setup:

```
dependencies: [{ 
	src: 'plugin/reveal-videoplayer.js',
	async: true,
	condition: function() {
		return !!document.createElement('video').canPlayType; 
	} 
}]
```