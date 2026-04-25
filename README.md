# Reverse Engineering MaaS 

## Overview

Found this malware because of a "try my game" social-engineering message on Discord. Wanted to figure out what it does / how it works.

At first I thought it would take me a few hours to figure it out, but I was wrong. After a few days of spending countless hours on it, I have reconstructed the code and now know how it works.

In this document I will explain what data it steals, how it steals said data and what methods it uses to obfuscate its code.

## Backstory

Someone I knew on Discord messaged me and asked me if I could try their game out for 5 minutes. Told me it was their project for college. Although, once I asked a few question about it, they quickly removed me from their friends list. All of this was very suspicious so I went in thinking that it had some sort of malware. 

I first visited their youtube video game trailer that they have sent to me. The video had a few thousand views and a decent amount of positive comments. In the comments, they included their website. The website looked well made, although it was most likely made with ChatGPT as the code included an image with ChatGPT in its file name.

The download button just linked you to a DropBox download. The file name was `InnerEvilSetup.exe` with the size of `59.43MB`. The author of this DropBox link was `alone`, clearly showing that most "hackers" are losers.

*You should always use a VPN or TOR when entering shady websites*

<table>
  <tr>
    <th>Website</th>
    <th>DropBox Downlaod</th>
  </tr>
  <tr>
    <td><img src="pictures/website.png" alt="website page" width=1000px></td>
    <td><img src="pictures/download.png" alt="download page" width=1000px></td>
  </tr>
</table>