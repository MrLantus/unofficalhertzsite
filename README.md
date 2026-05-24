# !!UNOFFICAL!! HERTZ SITE
 An open source fork of the [Temportal](https://temportal.neocities.org) website with sample places for Hertz users alike.

## Important
This is not intented to profit off of nedford321's creations, nor pass it off as official or claim to be affliated with him, but  rather this is a passion project by a (dedicated?) fan of Hertz, and I do not intend any harm or any dangerous intentions whatsoever :))) if you don't want this up, please contact me and I'll take it down - T. Lantus
P.S: if you want a game to be added fill out this application: will add once it is finished based on input from friends after I finish a prototype of it and bring it up to said friends on discord via a private channel on a server of mine lol

## How to Use
If you want to run this locally, you can install a program or package like [http-server](https://www.npmjs.com/package/http-server) and run it inside the directory with all the website files. You can also upload the files to a static webhoster like Neocities and run it that way.

### Running with http-server
To run the unofficial Hertz site with http-server installed, open Command Prompt and navigate to the folder on your computer with the Temportal website files. Enter `http-server` and a web server should start locally on your machine. The window should tell you what link to go to in your web browser but it should default to `localhost:8080`. If you want to stop the server, you can press CTRL+C with the Command Prompt window open.

### Adding Places
The lists of places and minigames are handled by two JSON files which are then parsed by the JavaScript code. The two JSON files for places (named `places.json` respectively) are located in the `data` folder, the sample place metadata included in the code serve as a blueprint for the places you can add. 

Each game is represented by a dictionary with properties defining the information that should be displayed on the website. Here is what an entry for a game looks like in `places.json`.
```javascript
{
	"name": "brickyard_v1", // The name
	"description": "A demo place with all available tools and some buildings.", // The description
	"thumbnail": "/screenshots/places/1/Level.jpg", // The thumbnail. For places, please see this list for thumbnail formats availabe during this time: TBA once I start work on it after I finish the application and release the final product of it lol
	"released": "2025-01-11", // Release date
	"data": "/data/places/1.rbxl", // Link to the game. Depending on your hoster, you might need to upload the games somewhere else.
	"author": "Torran", // The author of the game.
	"tag":  "Builds", // The tag or genre used to categorize the game.
	"client": "May 24, 06", // The reccomended client to play the game with. This has no effect on the pages for minigames.
	"mplink": "" // If a link is added, a "Visit Online" button will appear on the place's page. ONLY USE FOR MAPS SET TO JUNE 1ST 2006 OR AFTER THAT DATE CLIENTS
},
```
###### Do not copy this code with the comments included or it will break. 

Where you upload your games and screenshots is up to you as you specify the link for each of them in the JSON data but there are specific folders made in the repository for ease of organization. When adding new games to the JSON files, you may need to press CTRL+F5 to do a full refresh of the page to see your changes.

### Modifying the header and footer
The header and footer files are located inside the `include` folder and are added to the webpages with JQuery. You can edit them as you would any other HTML file. One hurdle is that doing CTRL+F5 to do a full refresh on the page doesn't always update the header/footer so you might need to manually clear all of your browser data for your website or opening the website in Incognito Mode.

## A Personal Request
Please don't flood webhosters like Neocities with a bunch of clones of that site. If you want to create a fork of it and put games on it, I request that you put your own twist on it and not just leave a stock installation with no changes. I imagine a lot of people using this are going to be young kids making their first (and hopefully last (get out while you still can)) revival so I strongly encourage you to try something unique with this instead of leaving it as an empty website with nothing to do.

## Usage Rights
This project is published under the MIT license so attribution is required. I'm not gonna go after you if you use a snippet of code here and there because Gev basically did the same thing with random threads on Stack Overflow. If you use the whole repository, I would strongly appreciate you to properly attribute Gev. Here is how you can attribute Gev.
```
This project uses code and/or assets from the Temportal Website.
Copyright (c) 2023-present Gev (https://gev.neocities.org)

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```
Some screenshots may contain traces of the skybox "null_plainsky" by Jauhn Dabz who gave explicit permission for the skybox to be freely used in commercial or non-commercial projects.
