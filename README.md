# WormPath
 Draws "worms" along vector paths with parametrized brush block.

![Wormpath screenshot](/images/screenshot.png)

## Setup
 1. Copy files to some directory on your hard drive. 
 2. Launch a local server of your choice. (I'm using CodeKit or Visual Studio Code Live Server). 
    - Visual Studio https://code.visualstudio.com/  
    - Visual Studio Code https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer
    - CodeKit https://codekitapp.com/
 3. Install a pug compiler. CodeKit has it built-in, for Visual Code Studio you can use eg.:https://marketplace.visualstudio.com/items?itemName=jaheenafsarsyed.live-pug-compiler 
 3. Open wormpath.html in a browser.

## Using your own paths for drawing 
 Modify images/pathsource.svg in eg. Adobe Illustrator. SVG should ONLY contain paths in a single layer, not groups, not compound paths. So, release those compound paths and ungroup your groups. Keep it simple.

## What works
 Regular fonts don't work as you would think, because they are not made of single strokes. So you need to either draw your own, or use other solutions, for example https://www.templatemaker.nl/singlelinetext/

## Export SVG
 Probably only works with very slow density and low line count. Screenshots are the way to go right now.

## Presets
 There are a few hard coded presets, but you can save settings into your browser's localstorage. Controls are at the bottom of the screen.

## Known issues
 Drawing disappears on resize. Just change any value to redraw.

## Animation
 Animation is in very early steps, only a few properties are supported. Animations are loops where properties change according to sine wave. 
 1. Enter the min/max values of each property in the animation tab. Test with *Step forward* if you like.
 2. Press *Start animation*
 3. Press *Start Capture*
 4. When all frames have been generated, *Stop capture*
 5. Press *Stop animation*

 The animation will be downloaded in a format of choice.
 Screen capture script by https://github.com/spite/ccapture.js
