# Entry 5
##### 4/20/25

 ### Tool: Aframe:
### What I learned about my tool
I learned that Aframe is a tool you can use to make 3D stuff on a website, and even build virtual reality scenes. You can add shapes like boxes, spheres, and planes, and move them around, change their size, and color them however you want. 

### How I learned my tool
I started learning Aframe by watching some YouTube videos that explained how to get started. The first one I watched showed me how to set up a simple scene and add shapes. I also went on the Aframe website and copied some example code to play around with. Changing the colors and background helped me understand how things worked. It was fun just testing stuff to see what happened.

### What I tried, changed, or made
At first, I added some basic shapes and a green plane as the ground, then changed the background to black. Later, I started trying to make candlesticks because my project is about trading. I messed around with their height and size to get them looking right. I’m still working on building the full trading platform scene, and next I want to add some indicators too.

![Screenshot 2025-04-20 112154](https://github.com/user-attachments/assets/7920aec1-60d3-40a0-91f3-57f36d27ee32)

![Screenshot 2025-04-20 105346](https://github.com/user-attachments/assets/184e8293-94aa-42c3-bb1a-3984088a5429)
_________________________________________________________________________________________________________________________________________________________________
### Sources: 
🎥 YouTube Video – <a href="https://www.youtube.com/watch?v=jhEfT9YjLcU">Easily code a virtual reality web experience with A-Frame</a>
This video helped me understand the basics of setting up a scene and using shapes in Aframe.

🌐 Official Website – <a href="https://aframe.io/">Aframe.io</a>
I used the documentation here to copy example code and learn how different components work.

🎥 YouTube Video – <a href="https://www.youtube.com/watch?v=v6mpIq-OcRs">Multiplaying using Networked-Aframe and Mediapipe</a>
This video helped me try to build candlesticks and get ideas for my trading-themed project.
__________________________________________________________________________________________________________________________________________________________________
### Skills:
One skill I’ve gotten better at is figuring things out when stuff doesn’t work. When I was trying to make the candlesticks for my trading chart, I had to play around with the sizes and shapes a lot to get them to look right. It wasn’t easy, and I had to keep testing and changing numbers until it finally looked good.

Another skill I’ve developed is learning how to use tutorials and documentation to teach myself something new. I watched videos and read through the Aframe website to understand how everything works.
__________________________________________________________________________________________________________________________________________________________________
```<html>
  <head>
    <script src="https://aframe.io/releases/1.6.0/aframe.min.js"></script>
  </head>
  <body>
    <a-scene>
      <a-sky color="white"></a-sky>
      <a-plane color="lightblue" rotation="-90 0 0" height="20" width="20"></a-plane>
      <a-assets>
        <video id="antarctica" autoplay loop="true" src="antarctica.mp4"> </video>
      </a-assets>

      <!-- Using the asset management system. -->
      <a-videosphere src="#antarctica"></a-videosphere>
      
<!-- Green candlestick (bullish) - Trend -->
<a-box
position="-2 3 0"
depth="0.1"
height="2"
width="0.4"
color="#4CAF50"
shadow="cast: true; receive: true"
></a-box>
<a-box
position="-1.5 4 0"
depth="0.1"
height="2"
width="0.4"
color="#4CAF50"
shadow="cast: true; receive: true"
></a-box>
<a-box
position="-1 4.5 0"
depth="0.1"
height="2"
width="0.4"
color="#4CAF50"
shadow="cast: true; receive: true"
></a-box>
<a-box
position="-0.5 6 0"
depth="0.1"
height="2"
width="0.4"
color="#4CAF50"
shadow="cast: true; receive: true"
></a-box>

<!-- Red candlestick (bearish) - Trend -->
<a-box
position="0 5.5 0"
depth="0.1"
height="2"
width="0.4"
color="#F44336"
shadow="cast: true; receive: true"
></a-box>
<a-box
position="0.5 4.5 0"
depth="0.1"
height="2"
width="0.4"
color="#F44336"
shadow="cast: true; receive: true"
></a-box>
<a-box
position="1 4 0"
depth="0.1"
height="2"
width="0.4"
color="#F44336"
shadow="cast: true; receive: true"
></a-box>
<a-box
position="1.5 3 0"
depth="0.1"
height="2"
width="0.4"
color="#F44336"
shadow="cast: true; receive: true"
></a-box>

<!-- Camera -->
<a-camera position="0 5 10"></a-camera>

    </a-scene>
  </body>
</html>
```
