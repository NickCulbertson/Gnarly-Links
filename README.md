# Gnarly Links

An Open Source HTML Template to link your music/game/software product pages in one place. It's as easy as adding a page to your site.

## Features

• Clean Mobile-First Design

• Attractive Social Media Embeds

• Store Marketing Badges

• Easy to Use

• Fully Customizable & Open Source

## Demos

Website - [http://www.gnarlylinks.com](http://www.gnarlylinks.com)

Music Example - [http://www.mobypixel.com/synthwave-escape-original-game-soundtrack](http://www.mobypixel.com/synthwave-escape-original-game-soundtrack)

## Implementation

1. Download the "GnarlyLinks_Template" folder. Here you will find index.html, gnarlystyle.css, sample.mp3, .htaccess, and an image folder.

index.html - The page people will see when they visit `http://www.YOUR_WEBSITE_NAME.com/YOUR_FOLDER_NAME`
gnarlystyle.css - The styles for this page.
sample.mp3 - If you are sharing audio, it might be nice to have a sample. Replace it with your own "sample.mp3" file or delete it if you're not using the audio tag.
.htaccess - This file will remove the need to include "index.html" as url extention.
img - This is where all the art for the page and store badges is stored. Feel free to delete the badges you don't need or add your own.

2. Change the "GnarlyLinks_Template" folder name to whatever you like. I recommend your project name with a `-` between words. 

3. Open the index.html in a code editor and update it with all your product information.

4. Adding your cover artwork by replacing the "cover.png" file in the img folder. You can change the background by replacing the "bg.png" or use the one provided (it does looks pretty sweet). 

5. Add Links to your product. Search through the img folder to see which branding icons are available or add your own. Here is how to add a row:

```
<!-- Item Row -->
<div class="rowDiv">
    <a href="https://STORE_URL_LINK" class="rowLink" target="_blank"></a>
    <img class="rowIcon" src="img/samplerow.png" alt="Store Name"></img>
    <img class="rowArrow" src="img/arrow.png" alt="Visit Link"></img>
</div>
```

Example: App Store Link
```
<!-- Item Row -->
<div class="rowDiv">
    <a href="https://STORE_URL_LINK" class="rowLink" target="_blank"></a>
    <img class="rowIcon" src="img/appstore.png" alt="App Store"></img>
    <img class="rowArrow" src="img/arrow.png" alt="Visit Link"></img>
</div>
```

6. Add the entire folder to your site's root directory. Now your page is available at
`http://www.YOUR_WEBSITE_NAME.com/YOUR_FOLDER_NAME`

7. Share the link and do the happy dance!

## Optional Features

You can add an audio sample to your page:
```
<!-- Audio Sample -->
<audio controls><source src="sample.mp3" type="audio/mpeg"></audio>
```

You can seperate your rows into sections by adding headers:
```
<!-- Section Header -->
<div class="rowHeaderDiv">
    <p>Header Title</p>
</div>
```

This script can be used if you'd like to redirect your visitors automatically to a store if they are on mobile. This can be useful if you have a game on the App Store and you want iPhone visitors to be redirected to the App Store page instead of your link page. Add this in your `<header></header>` tag:
```
<!-- Mobile Auto Redirect -->
<script>
    var agent = navigator.userAgent.toLowerCase();
    if (agent.search("iphone") > -1 || agent.search("ipod") > -1 || agent.search("ipad") > -1 || agent.search("appletv") > -1) {
        //App Store
        window.location.href = "APP_STORE_LINK";
    }else if (agent.search("android") > -1) {
        //Google Play
        window.location.href = "GOOGLE_PLAY_STORE_LINK";
    }else {
         
    }
</script>
```

Add social media links to the bottom of the page:
```
<!-- Share Your Socials -->
<div class="textBubbleDiv">
    <p>Follow us:
        <a href="https://www.twitter.com/" target="_blank"><img class="socialLink" src="img/twitter.png" alt="Visit Link"></img></a>
        <a href="https://www.facebook.com" target="_blank"><img class="socialLink" src="img/facebook.png" alt="Visit Link"></img></a>
        <a href="https://www.instagram.com" target="_blank"><img class="socialLink" src="img/instagram.png" alt="Visit Link"></img></a>
    </p>
</div>
```

## About Gnarly Links

This project was born out of neccessity. I launched an album to all the platforms, and I relied on a service to share those links in one place. I didn't like the idea of those pages going away if I stopped using their service, so I made my own. I'm making this template Open Source because I want to empower creatives to support themselves. You've worked too hard, too long to give away control. I hope it helps make a first impression for your followers most triumphant! 

If you have any questions, suggestions, or feedback please send them my way. This is as much for me as it is for you.

Enjoy!

Nick Culbertson
