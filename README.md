# Danbooru-Feed-Guide

### This guide will tell you how to make a Discord webhook feed using Danbooru, webhooks and IFTTT.

1. Create an account at https://ifttt.com.

2. Make a new applet by going to https://ifttt.com/create/, and select RSS then New Feed Item as the trigger.

3. In the feed URL box, put ``https://safebooru.donmai.us/posts.atom?tags=[insert up to 2 tags separated by a + here]``.  Example: ``https://safeborru.donmai.us/posts.atom?tags=touhou+elly``

 3.5. If you want an NSFW feed instead, put ``http://danbooru.donmai.us/posts.atom?tags=[insert 1 tag here]+-rating%3Asafe``.  Example: ``http://danbooru.donmai.us/posts.atom?tags=elly+-rating%3Asafe``

4. For the action, select Webhooks and then Make a Web Request.

5. In your Discord server (you will need the Manage Webhooks permission), go to the channel you want a Danbooru feed in and go to your channel settings. Then, go to Webhooks and press "Create Webhook". Give this webhook any name and  profile pic that you want, and then copy the webhook URL.

6. Back at the IFTTT window, put the Webhook URL you just copied into the URL box. Then, set Method to POST, set Content Type to "application/json" and set Body to ```{"content":"{{EntryTitle}}: {{EntryUrl}}"}```.

7. Finally, press Create Action, give your IFTTT applet a name, and save it. Now, just wait and see that it works!  


Huge thanks to [Hazuzumi](https://twitter.com/hazuzumi) for creating this method. If you have any questions, feel free to DM me on Discord at Scamantus#2505.
[fork me daddy](https://www.amazon.com/Hiware-12-piece-Stainless-Dinner-Cutlery/dp/B01G8HUH8S/)
