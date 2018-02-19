# Project 01 Report
This is a web-based VR application that allows you to navigate through a decorated room and interact with select objects. The application was created using the A-Frame web framework. This project was completed for the purposes of the CS 4331-002 Virtual Reality class at Texas Tech University.

You can access the web-based application [here](https://christine-elise.github.io/).

The video demo can be found [here](https://drive.google.com/file/d/1nCwzZjx2y0-rtu1WPxGSnuVloK6WQnei/view?usp=sharing).

[Source Code](https://github.com/christine-elise/christine-elise.github.io/blob/master/index.html)

[Assets](https://github.com/christine-elise/christine-elise.github.io/tree/master/Assets)

*Project Screenshot*

![](/Assets/Report/Project01Screenshot.png)

## Getting Started

### Framework & Software Choices
The project was to be done in an HTML document as it needed to be web-based. A combination of basic HTML tags and JS were used to create a small portion of this application. The main portion of the application was coded using the [A-Frame web framework](https://aframe.io). In addition, I also included the help of the [A-Frame Extras](https://github.com/donmccurdy/aframe-extras) library to include the **universal-controls** add-on to the camera component. This allows for the app to be accessible through a computer or a phone with/without a Google Cardboard.

This project was coded in the [Sublime Text](https://www.sublimetext.com/) editor.

In order to view live updates of my code during the development process, I downloaded [live-server](https://github.com/tapio/live-server). 

### Low-Fidelity Prototyping
First, I decided to do some low-fidelity prototyping and sketch out the floor design for my project. I included furniture placement as well as some front and side views of the furniture so I knew how to design them out of the basic geometry A-Frame offers. Originally, I had planned to design every piece of furniture myself using the basic geometry in order to minimize rendering time; however, this changed later as development went on.

*Paper Prototype*

![](/Assets/Report/IMG_0037.JPG)

## Duties

In order to achieve an excellent rating, I needed to produce a room with 15 unique models. Some models needed to be interactable by animating and/or producing sound. The room needed to be appropriately lit, and the user should have control over the lighting. And last, but certainly not least, the user should be able to navigate around the room using either keyboard and mouse input or phone touch input with/without a Google Cardboard.

### Unique Models
*Couch*

![](/Assets/Report/Couch.png)

*Chair*

![](/Assets/Report/Chair.png)

*Desk Chair*

![](/Assets/Report/DeskChair.png)

*Piano Bench*

![](/Assets/Report/PianoBench.png)

*Bar Stool*

![](/Assets/Report/BarStool.png)

*Bar*

![](/Assets/Report/Bar.png)

*Wine Bottle*

![](/Assets/Report/WineBottle.png)

*Bar Shelf*

![](/Assets/Report/BarCabinet.png)

*Glass Tables*

![](/Assets/Report/GlassTable01.png) ![](/Assets/Report/GlassTable02.png) ![](/Assets/Report/GlassTable03.png)

*Desktop Tower*

![](/Assets/Report/DesktopTower.png)

*Keyboard*

![](/Assets/Report/Keyboard.png)

*Mouse*

![](/Assets/Report/Mouse.png)

*Canvases*

![](/Assets/Report/Canvas01.png) ![](/Assets/Report/Canvas02.png)

### Interactable Models
*TV On/Off*

*While on, TV plays a video*

![](/Assets/Report/TVon.png) ![](/Assets/Report/TVoff.png)

*Monitors On/Off*

*While on, middle monitor plays a video*

![](/Assets/Report/MonitorsOn.png)
![](/Assets/Report/MonitorsOff.png)

*Dim Lights & Control Blinds Buttons*

![](/Assets/Report/ControlButtons.png)

*Blinds animate down when Control Blinds is pressed*

![](/Assets/Report/Blinds.png)

*Result when Dim Lights button is pressed*

![](/Assets/Report/DimLights.png)

*Lamp On/Off*

![](/Assets/Report/LampOn.png)
![](/Assets/Report/LampOff.png)

*Piano plays when clicked*

![](/Assets/Report/Piano.png)

### gltf Models
As stated above, I wanted to originally minimize rendering time by creating my own models out of the basic geometry A-Frame offers; however, this changed due to the models not fitting the atmosphere of the room - they were too box-y. I decided to add a few gltf models, but to keep it at a very small number. As you can see, I managed to only include 4 gltf models, and the rendering time remains relatively low.

## Obstacles

### Getting Used to A-Frame
Getting started with A-Frame was rough after being so accustomed to Unity. The visual inspector does not include as many capabilities as that of Unity's. It is very basic when it comes to adding entities. In Unity, when an object is added, it automatically comes with geometry and material components. In A-Frame, those must be individually added. Unity also has many drag and drop features that A-Frame lacks. However, despite some of these shortcomings, I was eventually able to warm up to A-Frame's framework and develop a rhythm of utilizing the visual inspector and writing source code.

### Local Files
At first, the images that I used for my materials would not load. After some quick research, I learned that Google Chrome denies requests to local files. To fix this issue, I downloaded and hosted my code temporarily on live-server for the development process.

### gltf Models
Originally, my gltf models would not show up anywhere in the scene. While this is a very rookie mistake, I realized this was due to the use of backslashes in my file paths instead of utilizing the correct method of forward slashes.

### Animating the Blinds
My original approach for all interactable objects was to utilize the **AFRAME.registerComponent()** functionality to attach click event listeners. However, this method did not appear to be compatible when it came to emitting a pre-defined **a-animation**. Instead, I rewrote each of my events as JS functions and called them using the **onclick** events. This not only was a simpler approach, but it improved readability.

### A-Frame Extras
As I reached the final stages of my development, one problem still stood before me - navigating around the space using the Google Cardboard. After some research, I found that the A-Frame Extras library solved this problem by utilizing the **universal-controls** add-on. As of now, this seems to be the best solution; however, there is a small functionality issue. When navigating using a mouse and keyboard, the controls occasionally "rubber-band" you back to a previous position. Hopefully this issue will be fixed in a future update.

## Conclusion
For this project, I designed a well-lit room that the user could navigate through and interact with select objects. The application is accessible through both a computer and phone; however, the computer navigation does have some small issues. Some obstacles were encountered when it came to warming up to the A-Frame and web development environments, but these issues were eventually eliminated. Overall, I completed a solid product that contains all the requirements to receive an excellent rating.

## Asset References
### Image Textures
http://www.ivotopalov.com/2017/05/wood-floor-texture-seamless/best-wood-floor-texture-seamless-light-wood-floor-texture-seamless/

https://i.pinimg.com/736x/18/fa/1d/18fa1daed91d722ae2360399b4b944b5--wood-texture-seamless-wood-floor-texture.jpg

http://clipground.com/images/and-wallof-stone-clipart-14.jpg

https://www.sketchuptextureclub.com/public/texture_d/0003-white-wood-flooring-texture-seamless-hr.jpg 

http://www.lol-wallpapers.com/artwork/dark-star-orianna-khazix-login-screen/

https://art-of-lol.com/aurelion-sol-teasing/

https://na.leagueoflegends.com/en/page/star-guardian-skins-now-live

http://www.theedlos.com/granite-kitchen-countertops-texture_black-granite-texture-seamless-viewing-gallery_10.html

http://www.ivotopalov.com/2017/08/stone-tile-texture/modern-stone-tile-texture-black-subway-tile-texture-floor-tiles-subway-bevelled-long/

https://www.replacementlaptopkeys.com/lenovo-yoga-3-pro-13-laptop-keyboard-key-replacement/

http://www.descargar-musica320.com/e4c527721896-mouse-pad-texture.html

https://www.mavericklabel.com/blog/10-wine-bottle-label-designs-you-should-see/

http://handpickedselections.com/product/490-2011-Merlot.htm

https://tablascreek.com/wines/2009_esprit_de_beaucastel_blanc

http://seamless-pixels.blogspot.com/2014/07/grass-4-seamless-turf-lawn-green-ground.html


### Video Texture
https://media.giphy.com/media/RQQqlCw32bR7i/giphy.gif

### Sound
https://freesound.org/people/HerbertBoland/sounds/29834/

### gltf Models
*gltf model authors are included in their respective assets folders!*
