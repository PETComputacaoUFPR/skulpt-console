```
   ______        __     __          _____                   __
  / __/ /____ __/ /__  / /_  ____  / ___/__  ___  ___ ___  / /__
 _\ \/  '_/ // / / _ \/ __/ /___/ / /__/ _ \/ _ \(_-</ _ \/ / -_)
/___/_/\_\\_,_/_/ .__/\__/        \___/\___/_//_/___/\___/_/\__/
               /_/
```

 --------------------------------------------------------------------
Polymer component wrapping Skulpt and CodeMirror

## What is this?
Skulpt-Console is a web component built with [Polymer](https://www.polymer-project.org/) that wraps [Skulpt](http://www.skulpt.org/) and [CodeMirror](https://codemirror.net/) in a text editor.

## Installation and usage
Install it with:
#### npm
`npm i --save skulpt-console`
#### bower
`bower install --save skulpt-console`

In your html file import the component and just drop the tag. You'll need a `<canvas>` and a `<pre>` tag with ids to output the result.

```html
...
<head>
    <link rel="import" href="bower_components/skulpt-console.html"/>
</head>
<body>
    <skulpt-console>
    import turtle

    t = turtle.Turtle()

    for c in ['red', 'green', 'yellow', 'blue', 'lime']:
        t.color(c)
        t.forward(72)
        t.left(72)
    </skulpt-console>
    <pre id="output"></pre>
    <canvas id="canvas"></canvas>
</body>
```

Skulpt-Console expects the pre element do be identified as 'output' and the canvas as 'canvas'. You can change the names passing the id to it.

```html
    <skulpt-console output="my-custom-output" canvas="my-canvas">
        ...
    </skulpt-console>
    <div id="my-custom-output"></div>
    <div id="my-canvas"></div>
```

## Next features:
* [ ] Create an output element
* [ ] Console mode (as seen on skulpt.org)

## Contributing
Feel free to contribute by sendig a PR.
