# LastFM-Discord-RPC
![logo](assets/logo.png)<br />
LastFM-Discord-RPC adds a Remote Procedure Call (RPC) to Discord from LastFM.
Adding RPC to Discord will display:<br />
* Currently playing song from LastFM to Discord
* Your LastFM profile picture to Rich Presence (Optional)
* Scrobble amount (how many times you listened to a song) to Rich Presence (Optional)
* The currently playing song's lyrics to your bio (Optional, Beta -  [Please read](#lyrics))


<details>
<summary><a name="lyrics"></a><H2>Add Lyrics to Discord Bio</H2></summary>
To add Lyrics:

1. Go to Discord (https://discord.com/) and select **Login**. 
2. Enter your Email or phone number and password.
3. After logging in, select the Gear Icon (**User Settings**) on the lower-left corner of Discord.
4. Go to **User Settings > Profiles > About Me**.
5. Right-click in the About Me text-box and select **Inspect**.
6. A panel opens in your browser:<br/>
     * For Microsoft Edge, select Network icon.<br/>
     * For Google Chrome and FireFox, select Network tab.</br>
8. Edit your bio and select **Save Changes**.
9. A event called "Profile" should now be in the network section, right click it and copy as cCurl (Bash). 
10. Paste it into https://curlconverter.com/python/ 
11. Open lyricsBoy.py and paste the output of curlconverter into the cookies and headers section

</details>
   
## Requirements 🛠️
1. Create a LastFM API Key (https://www.last.fm/api/account/create).
2. Install the packaged version [here](https://github.com/chubbyyb/LastFM-Discord-RPC/releases/tag/v0.2).
3. Run ```lfmRPC.exe```<br />
           ![image](https://github.com/chubbyyb/LastFM-Discord-RPC/assets/79348344/b574a340-135f-44d0-93e8-a9b014021057)
4. Press settings, input your username and API key.
           ![image](https://github.com/chubbyyb/LastFM-Discord-RPC/assets/79348344/fc20e5f6-0d4a-4447-8ce6-78b12e319517)
6. Restart the program.

# Build 🛠️
I like using electronmon because it hot reloads, feel free to edit manually
1. ```bash
   npm install
   ```
2. ```bash
   npm install electronmon
   ```
3. ```
   npx electronmon .
   ```
   
 
## Images 🎵
![eg1](assets/eg1.png)<br />
![eg3](assets/eg3.png)<br />
> Using profile picture as small image<br />
![DiscordCanary_mxJ0OSuhNA](https://github.com/chubbyyb/LastFM-Discord-RPC/assets/79348344/e65be998-42d9-4132-a630-f587ed5f0b64)<br />





<details>
<summary>💽 Supported Platforms:</summary>
<ul>
<li>Anything that scrobbles to LastFM is supported</li>
<li>This extension scrobbles most of the major streaming platforms: https://chrome.google.com/webstore/detail/web-scrobbler/hhinaapppaileiechjoiifaancjggfjm</li>
</ul>
</details>
