# Cookie Action for the Discord Bot Atlas - V. 3.3.4 by *Shylke#8325*

**Disclaimer:** This is *not* an economy action, and it will never be one.

## New Features and Fixes
* `a!cookie throw` subcommands;
* Subcommands and other variables are case insensitive now;
* Now it should properly award a role.
* Now it should also un-award the role if the belly amount goes lower than 100.

## What is It?
A single action related to cookies with multiple sub-commands that makes use of two persets per user. With a limit of 500 persistent variables per server, ideally it should work in a server with 250 members or less.

### "Dev Commands"?
They're called "dev" because I was the only who had access to them in my own servers while I was making this action. And you'd want to restrict their access to admins/mods alone. By doing that, replace the ID in `{if;{user.roles};includes;606515235591028756...}` with the one you want.

#### How to get a role ID;
* Server Settings - Roles - Right click the role you want - Copy ID;
* `a!id @Role`;
* Mention the role - put a `\` before the role - send message.

### Anything Else I Need to Know?
Using `a!cookie check` or `a!cookie check belly` may not give you a number (not even zero), if this happens ***please use `a!cookie reset` or `a!cookie reset belly` specifically*** , it should set your balance to 0. Any other command may give you a weird result.

After eating a certain amount of cookies, you're given a role. You *should* probably edit the role ID into an existing role in your server, otherwise it won't work. Feel free to change the required number for the role, or to remove this part: `{if;{perget;{user.id}_Belly};>=;100;{user.addrole;606864358995263596} You now have the **Cookie Lover** role!}` at all.

#### What does the *belly* thing mean and/or do?
As I said before, there are two persets per user: balance and belly. Consider the former the amount of cookies you hold or keep in a jar or something, and the latter the amount of cookies you have eaten. Additionally, you can only steal the amount of cookies a user has "on hand", but a mod or an admin can change or reset both values at any time.

### What if I Don't Want Cookies?
Then go ahead and change every bit in my code that refers to cookies. ¯\_(ツ)_/¯

## What's the Idea Behind This?
A friend and I wanted a command that would let you give virtual cookies to each other. I started out with a simple command scraped from JaM's Antiping, then tweaked to fit what I wanted to do. As I edited my action to make sure it had no errors, both my friend and I came up with other ideas and turned them into the many subcommands that there are today.

## Why Isn't This on the [Custom Action Repository](https://github.com/doddsy/atlas-custom-actions)?
~~Unfortunately it doesn't follow the requirements, and as for now this action is more a mess than anything. That being said, you're free to look around and grab the code to use on your own server, provided you have enough knowledge of Discord and Atlas.~~

It is now. Still, keep an eye on this repo as well for potential future updates — you'll never know.



