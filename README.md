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
    <path fill="#ff9999" stroke="none" d=" M 100 300 L 200 300 L 200 400 L 100 400 L 100 300"></path>
    <text fill="#000000" stroke="none" font-size="16pt" x="90" y="350">Red background</text>
  </g>

  <g>
    <path fill="#eeeeee" stroke="none" d=" M 100 100 L 200 100 L 200 200 L 100 200 L 100 100"></path>
    <text fill="#000000" stroke="none" font-size="16pt" x="90" y="150">Gray background</text>
  </g>
</svg>
```
