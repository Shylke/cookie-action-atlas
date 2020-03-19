# Cookie Action for the Discord Bot Atlas by *Shylke#8325*

**Disclaimer:** This is *not* an economy action, and it will never be one.

## What is It?
A single action related to cookies with multiple sub-commands that makes use of two persets per user. With a limit of 500 persistent variables per server, ideally it should work in a server with 250 members or less.

### "Admin Commands"?
Yes. You'd want to restrict their access to admins/mods alone. By doing that, replace the ID in `{set;AdminID;ID_HERE}` with the one you want.

#### How to get a role ID;
* Server Settings - Roles - Right click the role you want - Copy ID;
* `a!id @Role`;
* Mention the role - put a `\` before the role - send message.

### Anything Else I Need to Know?
Using `a!cookie check` or `a!cookie check belly` may not give you a number (not even zero), if this happens ***please use `a!cookie fix` or `a!cookie fix belly` specifically*** , it should set your (or someone else's) balance to 0. Any other command may give you a weird result.

After eating a certain amount of cookies, you're given two roles. You *should* edit the role ID in `{set;RoleRewardID;ID_HERE}` and `{set;RoleRewardBellyID;ID_HERE}` into an existing role ID in your server, or remove it at all to disable rewards. You can also change the amount of cookies you need to have/eat before you get the role(s) — just look in `{set;CookieAmount}` and `{set;CookieAmountBelly}`. They're set to 100 by default.

#### What does the *belly* thing mean and/or do?
As I said before, there are two persets per user: balance and belly. Consider the former the amount of cookies you hold or keep in a jar or something, and the latter the amount of cookies you have eaten. Additionally, you can only steal the amount of cookies a user has "on hand", but a mod or an admin can change or reset both values at any time.

### What if I Don't Want Cookies?
Then go ahead and change every bit in my code that refers to cookies. ¯\_(ツ)_/¯

## What's the Idea Behind This?
A friend and I wanted a command that would let you give virtual cookies to each other. I started out with a simple command scraped from Emrison's Antiping, then tweaked to fit what I wanted to do. As I edited my action to make sure it had no errors, both my friend and I came up with other ideas and turned them into the many subcommands that there are today.

## Hey, I Saw this Action on the [Custom Action Repository](https://github.com/doddsy/atlas-custom-actions)! Why Have a Dedicated Repo as Well?
Because the action you saw on the CAR is outdated and filled with bugs. I periodically go through the code and fix and tweak some things, occasionally adding new features, and this repo is where I keep track of said stuff.

## I Don't Know How to Use Actions at All! Can Someone Help Me?
If you need help with actions, you can join [Atlas' support server](https://discordapp.com/invite/AXXBPM7). But generally, unless you know what you're doing, it's best to only set the required variables, and leave the rest as it is.



