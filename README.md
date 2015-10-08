##Introduction

<p align="center">
<img src ="demo.png" alt="Demo picture"/>
</p>

Color-changer allows user to change colors of a part of a picture, such as hair. It uses two images, a background and a mask.

The coloring of the mask is done using svg filters. Two filters are used, the first one light up and saturate the image that becomes very white. It then act as a canvas for the second filter that colors using the user input.

<a href="https://docs.webplatform.org/wiki/svg/tutorials/smarter_svg_filters">More info on svg filters</a>

##Used Libs
* Spectrum for color selection using javascript: <a href="https://github.com/bgrins/spectrum">https://github.com/bgrins/spectrum</a>
* <a href="https://jquery.com/">JQuery</a>

##Usage
The website also reads query strings, the query parameters "bg" and "cut" can be used to respectively specify a background and mask (cutout) images.

Example:

```
/color/index.html?bg=http://i.imgur.com/LIKTzdo.jpg&cut=http://i.imgur.com/T8xJfrX.png
```

##Running it
1. Make sure apache is installed on your machine
2. Move to your public web folder

  ```bash
  cd /var/www/
  ```

3. Clone the repo

  ```bash
  git clone https://github.com/TTalex/color-changer.git
  ```

4. Access [localhost/color](http://localhost/color)
