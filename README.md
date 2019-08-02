# Cookie Action for the Discord Bot Atlas - V. 2.5.0 by *Shylke#8325*

**Disclaimer:** This is *not* an economy action, and it will never be one.

## What is It?
A single action related to cookies with multiple sub-commands split into three different sub-actions to prevent hitting the character limit; for this some sub-commands may have a longer delay, but it shouldn't be noticeable. This action makes use of two persets per user. With a limit of 500 persistent variables per server, ideally it should work in a server with 250 members or less.

### "Dev Commands"?
They're called "dev" because I was the only who had access to them in my own servers while I was making this action. And you'd want to restrict the access to admins/mods alone. By doing that, replace the ID in `{if;{user.roles};includes;606515235591028756...}` with the one you want.

#### How to get a role ID;
* Server Settings - Roles - Right click the role you want - Copy ID;
* `a!id @Role`;
* Mention the role - put a `\` before the role - send message.

### Anything Else I Need to Know?
Using `a!cookie check` or `a!cookie belly` may not give you a number (not even zero), if this happens ***please use `a!cookie reset` specifically*** , it should set your balance to 0. Any other command may give you a weird result.


## What's the Idea Behind This?
A friend and I wanted a command that would let you give virtual cookies to each other. I started out with a simple command scraped from JaM's Antiping and the void action, then tweaked to fit what I wanted to do. As I edited my action to make sure it had no errors, I came up with other ideas and turned them into the many subcommands that there are today.

## Why Isn't This on the [Custom Action Repository](https://github.com/doddsy/atlas-custom-actions)?
Unfortunately it doesn't follow the requirements, and as for now this action is more a mess than anything. That being said, you're free to look around and grab the code, provided you have enough knowledge of Discord and Atlas.



