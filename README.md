# Cookie Action for the Discord Bot Atlas - V. 3.1.0 by *Shylke#8325*

**Disclaimer:** This is *not* an economy action, and it will never be one.

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

#### What does the *belly* thing mean and/or do?
As I said before, there are two persets for user and these are balance and belly. Consider the former the amount of cookies you hold or keep in a jar or something, and the latter the amount of cookies you have eaten. Additionally, you can only steal the amount of cookies a user has "on hand", but a mod or an admin can change or reset both values at any time.


## What's the Idea Behind This?
A friend and I wanted a command that would let you give virtual cookies to each other. I started out with a simple command scraped from JaM's Antiping and the void action, then tweaked to fit what I wanted to do. As I edited my action to make sure it had no errors, I came up with other ideas and turned them into the many subcommands that there are today.

## Why Isn't This on the [Custom Action Repository](https://github.com/doddsy/atlas-custom-actions)?
Unfortunately it doesn't follow the requirements, and as for now this action is more a mess than anything. That being said, you're free to look around and grab the code to use on your own server, provided you have enough knowledge of Discord and Atlas.



