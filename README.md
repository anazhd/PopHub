# PopHub
Can't pop her cherry? Why not pop cat or pop dog?

# PopCat bot/hack
Our first PopAnimals script, kick started by social media trend in Taiwan and Malaysia.

* Website: [popcat.click](https://popcat.click/)
* Script: [popcat_bot.js](/popcat_bot.js)

## Features
This simple script have few "features" compared to other shorter alternatives:
* **Tracks** how many pops you sent
* **Notifies** you if there's issue with sending pops
* **Ban-proof** (rate limited to 800 every 30 seconds)
* Shows which **country** you are contributing to
* **Light** on system resources
* Works even if you got marked as bot (yes, works even if the cat is shooting laser)

![Screenshot 2021-08-17 022153](https://user-images.githubusercontent.com/14260598/129611627-5a98da4e-c049-4020-9862-9911785beb78.png)

## Known restrictions
It is known that popcat.click can only accept 800 pops per 30 seconds, and you cannot request API again during the 30 seconds cooldown. 

The website also have a function that checks if you clicked more than 800 times and it will track how many times you hit the threshold. You will need to hit the threshold 10 consecutive times to be marked as a bot. The counter will reset when you miss the threshold.

![Screenshot 2021-08-15 141448](https://user-images.githubusercontent.com/14260598/129469081-6dbda7c2-c5cb-46b1-8c11-0dc1601ae84d.png)

If the variable `sequential_max_pops` reaches 10, you will be flagged as bot and the cat eyes will light up. 
You may **clear the website cookies** to unflag yourself.

Please don't try running this on same IP (even with different tab, browser, or devices), it won't work, only 1 request every 30 seconds is accepted for each IP.

![Screenshot 2021-08-14 184105](https://user-images.githubusercontent.com/14260598/129443727-7e95a17c-06b9-49e7-894b-2d2da5ff8a25.png)

# PopDog bot/hack
Second PopAnimals script. Still optimizing.

* Website: [popdog.click](https://popdog.click/)
* Script: [popdog_bot.js](/popdog_bot.js)

## Features
Our PopDog script have following features:
* **Optimized** for highest efficiency per UUID (approx 2000 clicks per 3.8 seconds)
* **Notifies** and tracks amount of clicks sent
* **Light** on system resources
* Silent

![Screenshot 2021-08-17 022301](https://user-images.githubusercontent.com/14260598/129612530-ff081088-09f1-4ca4-97a4-a6cb1f341e73.png)

# PopAss bot/hack
Third PopAnimals (PopHuman?) script. Still optimizing.

* Website: [popass.click](https://popass.click/)
* Script: [popass_bot.js](/popass_bot.js)

## Features
Our PopAss script have following features:
* **Optimized** for highest efficiency per IP (approx 1000 clicks per 0.6 seconds)
* **Notifies** and tracks amount of clicks sent
* Considerably **less resource intensive** compared to using keyDown event
* Works even if you got marked as bot

![Screenshot 2021-08-17 191113](https://user-images.githubusercontent.com/14260598/129716707-755534d7-807e-4e6a-bf40-b651c2438137.png)

# PopPig bot/hack
Most efficient hack for poppig.click.

* Website: [poppig.click](https://poppig.click/)
* Script: [poppig_bot.js](/poppig_bot.js)

## Feature
Our PopPig script has one feature:
* **Simple** (just 1 line of code)

# FAQ

## How do I use these scripts on an Android Chrome browser?
You may run the script by connecting to a PC with Chrome and use the **remote debugging** feature:
https://developer.chrome.com/docs/devtools/remote-debugging/

## Why Popcat is throwing 503 errors?
Popcat will sometimes respond with an error "503 - Haven't found your country code yet (try again later)". Despite what the error describing, it is most likely not to do with detecting your country, but rather CloudFlare have flagged you as a bot, and the API call failed. Unfortunately, you might need to wait it out.

AdBlocker is known to cause issue as well, simply disable them and see if it works.
