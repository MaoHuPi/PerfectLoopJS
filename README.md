# PerfectLoopJS

> 2023 &copy; MaoHuPi

> Flawlessly loop between one or more audio files.

## Import

```html
<script src="perfectloop.js"></script>
```

## Example

```js
let pl = new PerfectLoop();
let audioPath = 'audio/MaoHuPi - goodbyWorld.wav';
for(let _ = 0; _ < 2; _++){
	let audio = new Audio();
	audio.src = audioPath;
	pl.push(audio);
}
document.body.addEventListener('click', () => {
	pl.paused ? pl.play() : pl.pause();
});
```