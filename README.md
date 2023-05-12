# FireFox svg print bug

https://xcatliu.github.io/firefox-svg-print-bug/

A simple svg with `<path>` and `<text>` like this:

```html
<svg
  xmlns="http://www.w3.org/2000/svg"
  xmlns:xlink="http://www.w3.org/1999/xlink"
  style="position: absolute; width: 400px; height: 600px;"
>
  <g>
    <path fill="#ffff00" stroke="none" d=" M 100 100 L 200 100 L 200 200 L 100 200 L 100 100"></path>
    <text fill="#000000" stroke="none" font-size="16pt" x="90" y="150">Yellow background</text>
  </g>

  <g>
    <path fill="#eeeeee" stroke="none" d=" M 100 300 L 200 300 L 200 400 L 100 400 L 100 300"></path>
    <text fill="#000000" stroke="none" font-size="16pt" x="90" y="350">Gray background</text>
  </g>
</svg>
```

The webpage looks like this:

<img width="572" alt="image" src="https://github.com/xcatliu/firefox-svg-print-bug/assets/5453359/ad8b16a3-3772-459d-acb5-f5b754f1db1f">

However, during printing, the area that was supposed to have a gray background turned into an incorrect black background. In contrast, the yellow background appears as normal gray in print view:

<img width="1816" alt="image" src="https://github.com/xcatliu/firefox-svg-print-bug/assets/5453359/9494b8b7-8459-47c2-93eb-2f6f16b2e64a">
