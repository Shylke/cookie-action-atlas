**Command Name:** `a!cookie`

**Subcommand Name:** `a!cookie help`

**Command Description:**
Displays a help message.

**Usage:**
`a!cookie help` (leave the user part blank if you want to check the amount of the cookies you have eaten.)

**Code:**
```{if;{args;1};==;help;{if;{user.roles};includes;606515235591028756;{a!ae;--field1name="Commands";--field1value="`{guild.prefix}cookie give <user>` to give a cookie to a user.\n\n`{guild.prefix}cookie steal <user>` to steal a user's cookie.\n\n`{guild.prefix}cookie eat` to eat a cookie.\n\n`{guild.prefix}cookie check <user>` to check your cookies, or another user's cookies.\n\n`{guild.prefix}cookie belly <user>` to check how many cookies you, or another user, have eaten.\n\n`{guild.prefix}cookie help` to display this message.";--title=":cookie: Cookie Help :cookie:";--color="#8e715a";--timestamp="true";--description="Give cookies to whoever you want!";--footer="Version 2.5.0, Created by Shylke#8325";--field2name="Dev Commands";--field2value="`{guild.prefix}cookie award <user> <amount>` to award a user with cookies.\n\n`{guild.prefix}cookie remove <user> <amount>` to remove cookies from a user.\n\n`{guild.prefix}cookie reset <user>` to reset their cookie balance back to zero."};{a!ae;--field1name="Commands";--field1value="`{guild.prefix}cookie give <user>` to give a cookie to a user.\n\n`{guild.prefix}cookie steal <user>` to steal a user's cookie.\n\n`{guild.prefix}cookie eat` to eat a cookie.\n\n`{guild.prefix}cookie check <user>` to check your cookies, or another user's cookies.\n\n`{guild.prefix}cookie belly <user>` to check how many cookies you, or another user, have eaten.\n\n`{guild.prefix}cookie help` to display this message.";--title=":cookie: Cookie Help :cookie:";--color="#8e715a";--timestamp="true";--description="Give cookies to whoever you want!";--footer="Version 2.5.0, Created by Shylke#8325"}}}```
