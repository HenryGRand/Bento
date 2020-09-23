    
<div align="center">
<h1>Bento: 🍱 A Clean and Simple Startpage</h1>
</div>

![](https://github.com/MiguelRAvila/Bento/blob/master/assets/preview.png)

### Index

-   [Bento](#)
    -   [Features](#features)
    -   [Usage](#usage)
         - [Home Page](#as-home-page)
         - [New Tab](#as-new-tab)
    -   [Customization](#customization)
         - [Links and Icons](#links-and-icons)
         - [Colors](#colors)
         - [Wather Widget](#weather-widget)
         - [Greetings](#greetings)
         - [Image Background](#image-background)
#### Features:

- **Dark/Light** mode, you can toggle them and It'll be saved in local store
-   **Clock and Date** format can be set to 24 hour (default) or 12 hour
-   **Greetings** are easy to change and modify
-   **Variables** for custom colors in the `css` code
-   **Modular** javascript files for an easy read

<p align="center">
  <img src="https://github.com/MiguelRAvila/Bento/blob/master/assets/preview.gif">
</p>

### Usage:

#### As Home Page:
1. Fork this repo
2. Enable the Github Pages service `Settings > GitHub Pages > Source [master branch] > Save`
3. Set it as Home Page:
    - Click the menu button. and select Options. Preferences.
    - Click the Home panel.
    - Click the menu next to Homepage and new windows and choose to show custom URLs and add your `Github Pages link`

#### As New Tab:
1. You can use different Add-ons/Extensions for it
  - If you use Firefox: [Custom New Tab Page](https://addons.mozilla.org/en-US/firefox/addon/custom-new-tab-page/?src=search)
  - If you use Chromium (Brave, Vivaldi, Chrome): [Custom New Tab URL](https://chrome.google.com/webstore/detail/custom-new-tab-url/mmjbdbjnoablegbkcklggeknkfcjkjia)

### Customization

> All the code is using variables and is comented, It's easy to customize the project to your own, and this sections are the principal customizable elements in the Startpage:

#### Links and Icons
You can change the links (and the icons too) in the HTML Code:

<p align="center">
  <img src="https://github.com/MiguelRAvila/Bento/blob/master/assets/code1.png">
</p>

Change the link in the `href` property with the link you want. (The `target="blank"` makes the link to open a new tab with the link you choose). 
The Project uses [Feather icons](https://feathericons.com/) for the icons, and you can change them in the `data-feather=""` property with the name of the icon. 


#### Colors
In the CSS code you can always change the variables for both themes (Dark and Light)

<p align="center">
  <img src="https://github.com/MiguelRAvila/Bento/blob/master/assets/code2.png">
</p>
<div align="center">
<h5>Light mode (default)</h5>
</div>

<p align="center">
  <img src="https://github.com/MiguelRAvila/Bento/blob/master/assets/code3.png">
</p>
<div align="center">
<h5>Dark mode</h5>
</div>

#### Weather Widget

For setting up the Weather widget you're going to need an API Key in: `https://openweathermap.org/`. Once you have your Key you'll need to set yourlatitude and longitude, you can use: `https://www.latlong.net/` to get them. Once you have the data, you'll need to set them in the `weather.js` in the **js** folder. The code is 

> If you don't like the idea of having your API Key public, you can make the repo into a private one. You can still use the Github Pages service.

#### Greetings
You can put your name and change the greetings.

```js
var name = 'John Doe'; 
var lateTxt = 'Go to Sleep! ';
var morningTxt = 'Good morning! ';
var afterTxt = 'Good afternoon ';
var evenTxt = 'Good evening ';
```

It'll change in order of the hour.

#### Image Background

You can set your own background image with the variable `--imgbg` and set the route to the image you want It's disable by default. If you uncomment the variable, it has by default this image: 

<p align="center">
  <img src="https://github.com/MiguelRAvila/Bento/blob/master/assets/previewbg.png">
</p>

It has a black filter by default in `--imgcol`, and it'ts value is: `rgba(255, 255, 255, 0.7)` and `rgba(0, 0, 0, 0.7)` for the dark theme. You can change them and the opacity for a better experience with your image.
