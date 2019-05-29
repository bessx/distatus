Distatus - A Discord Streaming Status
=================

A small node.js app to set your Discord Streaming Status.

Easily clone from glitch.com with [remix](https://glitch.com/edit/#!/remix/distatus).

Full instructions can be found to install can be found on dayzoon's [youtube](https://www.youtube.com/watch?v=SqeB2ZIf2wo) channel.

Updates to your code will instantly deploy and update live after setup.

To keep alive without keeping a glitch.com tab open, try [uptimerobot.com](https://uptimerobot.com/).

Find out more about [distatus](https://github.com/bessx).

<br />

Setup Instructions
------------

**Create Glitch.com Account**
  1. Go to glitch.com
  2. Create New Project
  3. Select "hello-express" Project
  
**Get Code (Option 1)**
  1. Click here to remix from glitch: [Remix](https://glitch.com/edit/#!/remix/distatus).
  
**Get Code (Option 2)**
  1. Head to [github](https://glitch.com/@bess).
  2. Copy the code in the file.

**Add Required Packages**
  1. Open the package.json file
  2. Hit "Add Package"
  3. Add "discord.js" package
  4. Add "discord" package

**Retrieve Discord Login Token** 
  1. Start Discord app and press ctrl+shift+I
  2. Navigate to the Application Tab
  3. On the left hand pane, navigate to Local Storage > DiscordApp.com
  4. Scroll all the way down the main pane
  5. Restart discord (ctrl+R).
  6. As Discord starts a "token" key will apear below the "user_id_cache" key.
  7. Copy the "token" key while discord is restarting.
  8. Paste token into process.env.SECRET in .env file on glitch.com. (Don't include quotes.)
  
**Change Streaming Text**
  1. Open your server.js file
  2. Go to line 10 (server.js:10:25).
  3. Replace `...blurple.` in `client.user.setActivity('...blurple.', {` with requested status.
  4. ???????
  5. Profit.

**Keep Alive with UptimeRobot**
  1. Open [uptimerobot.com](https://uptimerobot.com/) and create an account.
  2. Hit "Add New Monitor"
  3. Monitor Type: HTTP(s)
  4. Friendly Name: Distatus
  5. URL: https://glitch.com/~distatus (insert your own glitch link here)
  6. Monitoring Interval: Every 5 Minutes
  7. Voila~  You can close your glitch.com tab!!

<br />

Required Packages
------------
- express
- discord.js
- discord

<br />

Made by [bess](https://glitch.com/@bess) and [dayzoon](https://www.youtube.com/watch?v=SqeB2ZIf2wo).
-------------------

\ ゜o゜)ノ