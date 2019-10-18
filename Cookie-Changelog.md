**Command Name:** `a!cookie`

**Subcommand Name:** `a!cookie changelog`

**Command Description:**
Gets the latest changelog.

**Usage:**
`a!cookie changelog`


**Code:** `{set;version;4.1.7}`

```{if;{args;1};==;changelog;{a!ae;--field1name="Bug Fixes";--field1value="• Fixed that bug when the 'You now have the Cookie Lover role!' would appear every. Fucking. Time. If your belly amount was over 100.\n• Fixed that other bug where the bot wouldn't check if the user existed before messing with their balance.\n• The empty number bug hasn't been fixed globally, but now there is a command to fix it for yourself.";--field2name="Features";--field2value="• `a!cookie fix` — fix the empty bug number if you ran into it.\n• `a!cookie sacrifice` — sacrifice a cookie, has a 50% chance to give you 2-5 cookies as a reward.\n• `a!cookie changelog` — basically what you're reading now.\n• Improved the help command.\n• `a!cookie reset` now asks you whetever you're sure to do it, and gives you 30 seconds to reply.\n• `a!cookie check` now gives a little flair message if your amount is below 0.\n• The changelog page lul.\n Updated the [README](https://github.com/Shylke/cookie-action-atlas/blob/master/README.md) page.";--title=":cookie: Cookie Command {get;version} Changelog :cookie:";--color="#8e715a";--footer="Created by Shylke#8325 • Command ran by {user.tag}";--timestamp="true";--description="[You can read the full changelog here](https://github.com/Shylke/cookie-action-atlas/blob/master/CHANGELOG.md)."}}```
