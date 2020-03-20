https://expressjs.com/en/starter/generator.html for basic info.

    express --no-view

Creates basic framework.

    node start

Invokes the package.json start command which fires up the app. This
starts with app.js and shows the index.html page.

Edit `public/index.html` and change some text. Add a text block:

    <script src="myapp.js">

Which will pull in and render the file. Then create `myapp.js` with the
following stuff in it:

    var msg="hello, world."
    console.log(msg)

Reload the page and you should see stuff in the browser console that works.

## Adding a request

Put this in your myapp.js file:

    fetch("http://localhost:3000")
    .then(res=>{console.log(res)})