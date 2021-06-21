Welcome to arobicOS!
I got this idea from a april fools github and I was like "Shit, why not"
Some things may say glizzy instead of arobic, this was originally a joke. But at this point its starting turning into something cool.

This is NOT REQUIRED, but you'll want to disable Same-Origin-Policy for the OS to be fully functional. Scroll down https://stackoverflow.com/questions/29983786/blocked-a-frame-of-origin-null-from-accessing-a-cross-origin-frame-chrome/65234451 here to find out how for your browser.

A lot of the original apps are stolen BTW. (FROM GITHUB)

FOR DEVELOPERS LOOKING TO MAKE APPS:

NOTE: Making apps is STILL in beta. I even came across an issue while making the example app, and had to modify the code to fix it!

Apps in this operating system are just a website embedded in an iframe.

To make your own app, here's a tutorial:

1: Clone the Example folder, under apps/custom. This is a pretty basic example of an app. (You can also create your own, but this is a good tutorial for beginners lolol)
2: Click on index.html - This is the part off the app that will always be shown when the user clicks on the app. I can't teach you html, but w3schools has good examples: https://www.w3schools.com/html/ 
3: Modify index.html to create your own app.
4: If wanted, you can make an index.js file(for code), and style.css files(to make the website look good)
5: To fit the theme of the site, you can optionally import materialize, by adding:
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/materialize/1.0.0/css/materialize.min.css" />
  <link rel="stylesheet" href="https://fonts.googleapis.com/icon?family=Material+Icons" />
  <script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>
To the top of your site, just below the head, and
  <script src="https://cdnjs.cloudflare.com/ajax/libs/materialize/1.0.0/js/materialize.min.js"></script>
  Just above the end of the body.
6: Create an install file. this is what the Operating system uses to install new apps, so you don't want to mess it up.
- Create an install.abrp file in your code(If your using the test app it should already be there);
Here's the format for the install file:

- The path to the apps folder(Case sensitive)
- The name of the app that will be shown when it is loaded
- The version of the app
- The icon for the app(FIND ICONS AT https://fonts.google.com/icons)
- The color of the app(FIND COLORS AT https://materializecss.com/color.html)
- The width of the BARRIER of the app
- The height of the BARRIER of the app
- The width of the FRAME of the app
- The height of the FRAME of the app
- The scale of the FRAME of the app(if it doesnt fit)
- If the app supports fullscreen(true or false)

So, with you knowing that, here's the format of the example app:

Example
Example
0.0.2
thumb_up
blue-grey lighten-3
450px
450px
500px
500px
1.1
false

So there you go! After your done, drag your app folder into apps/custom, and use the package manager to select your install.abrp file. After, press refresh, and you are done!
