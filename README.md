# Figma Automator Helper Functions
A collection of helpers and guides to use on your automation projects with Figma Automator.


Figma RGB to Web RGB 

```js
eval(function figmaRGBToWebRGB(color) {
  const namesRGB = ['r', 'g', 'b']
	const rgb = []
	namesRGB.forEach((e, i) => {
		rgb[i] = Math.round(color[e] * 255)
	})
	if (color['a'] !== undefined) rgb[3] = Math.round(color['a'] * 100) / 100
	return rgb
}; figmaRGBToWebRGB({{COLOR}}))
```

RGB to Hex

```js
rgbToHex({{COLOR}})
```
