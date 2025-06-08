---
draft: "true"
---
----
E Book Manager

Source: [Calibre](https://calibre-ebook.com/)

---
# Using Calibre to LCP to EPub

Source: [Reddit](https://www.reddit.com/r/Calibre/comments/1c2ryfz/2024_guide_to_dedrm_kindle_books/)

### 1. Install Calibre
### 2. Install the following Calibre plugins

- **KFX Input**, can be found by going to Preferences ⮟ > Get plugins to enhance calibre > Search ‘KFX’.
- **DeDRM Tool**, which needs to be loaded into Calibre separately. I had a few issues with adding it into Calibre so this is the process that finally worked for me*: 
- Download the zip file [here](https://github.com/noDRM/DeDRM_tools/releases/tag/v10.0.9).
- Once downloaded, create a new folder and name it whatever you like.
- Extract the zip file into that folder.
- Go to Calibre, then Preferences > Advanced > Plugins > Load plugin from file > New folder you created > Select DeDRM_plugin.zip
- Plugin should successfully load into Calibre.
### 3. Install Kindle for PC - Version 2.3.70682

- I used [this](https://www.download3k.com/Install-Kindle-for-PC.html) link - ensure that the ‘70682; is included in the .exe file, otherwise it will download the older version of the Kindle app, but not allow you to download your books as it is an outdated version.
- Log into your Kindle account, and download the books you want to convert.
- Once downloaded, go to Calibre and select Add Books. Select the books you wish to convert into EPUBs/other formats and they should load onto Calibre.
- Once downloaded, select the book(s) and press Convert Books.
- When the new menu pops up, ensure the Output Format on the top right is what you require, and press OK.
- Voila! It should remove the DRM from your Kindle book