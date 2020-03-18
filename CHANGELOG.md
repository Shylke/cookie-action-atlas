# Cookie Action - *Ver. 4.4.0*

## Bug Fixes 

* Fixed the long ass message when it included the reward part as well.

### Example
**Before:**

![Before](https://i.imgur.com/AIevqT7.png)

**After:**

![After](https://i.imgur.com/H5g1MEg.png)

(I still haven't figured out how to get the reward message to show at the end.)

## New Features
* `a!cookie info` — redirects you to my shiny new GitHub-powered [website](https://shylke.github.io/cookie-action-atlas).
* You can now set rewards for both the amount of cookies you have (Balance), and the amount of cookies you have eaten (Belly). Used to support only the latter before.
* ... or you can disable them altogether by clearing the `RoleRewardID` and/or `RoleRewardBellyID` variable(s).
* New Variables: `RoleRewardBellyID`, `CookieAmount`, `CookieAmountBelly`!
* You can now *easily* set the amount of cookies you need in order to get a reward, mess around with the `CookieAmount` and `CookieAmountBelly` variables.
* Now it'll properly display the role you have set for reward in the reward messages. Used to be "Cookie Lover" before.
* `a!cookie chnagelog` has changed to include only the link to this page.
* Updated [README.md](https://github.com/Shylke/cookie-action-atlas/blob/master/README.md) page.




# Cookie Action - *Ver. 4.1.7*

## Bug Fixes

* Fixed that bug when the "You now have the Cookie Lover role!" would appear every. Fucking. Time. If your belly amount was over 100;
* Fixed that other bug where the bot wouldn't check if the user existed before messing with their balance; 
### Example 
**Before:**

![Before](https://i.imgur.com/DRurAWn.png)

**After:**

![After](https://i.imgur.com/yteyLCp.png)

* The empty number bug hasn't been fixed globally, but now there is a command to fix it for yourself.
### Example
![Bug](https://i.imgur.com/7kqWCtO.png)

## New Features
* `a!cookie fix` — fix the empty bug number if you ran into it;
* `a!cookie sacrifice` — sacrifice a cookie, has a 50% chance to give you 2-5 cookies as a reward;
* `a!cookie changelog` — basically what you're reading now;
* Improved the help command;
* `a!cookie reset` now asks you whetever you're sure to do it, and gives you 30 seconds to reply;
* `a!cookie check` now gives a little flair message if your amount is below 0; 
* This page.
* Updated [README.md](https://github.com/Shylke/cookie-action-atlas/blob/master/README.md) page.
