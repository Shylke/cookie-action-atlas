**Command Name:** `a!cookie`

**Alias:** `a!cookie help`

**Command Description:**
Displays a help message.

**Usage:**
`a!cookie help`or `a!cookie`

**Code:** ```{if;{lower;{args;1}};==;help;{if;{user.roles};includes;606515235591028756;{set;help;2};{set;help;1}}}
{if;{lower;{args;1}};==;;{if;{user.roles};includes;606515235591028756;{set;help;2};{set;help;1}}}```

```{if;{get;help};==;2;{a!ae;--field1name="Commands";--field1value="`{guild.prefix}cookie give <belly> <user>` to give a cookie to a user.\n`{guild.prefix}cookie steal <user>` to steal a user's cookie.\n`{guild.prefix}cookie eat <all>` to eat a cookie.\n`{guild.prefix}cookie throw <belly> <all>`to get rid of your cookies.\n`{guild.prefix}cookie check <belly> <user>` to check your cookies, or another user's cookies.\n`{guild.prefix}cookie fix` to manually fix the empty number bug.";--field2name="Meta Commands";--field2value="`{guild.prefix}cookie changelog` to get the latest changelog.\n`{guild.prefix}cookie help` to display this message.";--field3name="Admin Commands";--field3value="`{guild.prefix}cookie award <belly> <user> <amount>` to award a user with cookies.\n`{guild.prefix}cookie remove <belly> <user> <amount>` to remove cookies from a user.\n`{guild.prefix}cookie reset <belly> <user>` to reset their cookie balance back to zero.";--field3inline;--title=":cookie: Cookie Help :cookie:";--color="#8e715a";--footer="Version {get;version}, Created by Shylke#8325";--timestamp="true";--description="Cookies for everyone!"}}```

```{if;{get;help};==;1;{a!ae;--field1name="Commands";--field1value="`{guild.prefix}cookie give <belly> <user>` to give a cookie to a user.\n`{guild.prefix}cookie steal <user>` to steal a user's cookie.\n`{guild.prefix}cookie eat <all>` to eat a cookie.\n`{guild.prefix}cookie throw <belly> <all>`to get rid of your cookies.\n`{guild.prefix}cookie check <belly> <user>` to check your cookies, or another user's cookies.\n`{guild.prefix}cookie fix` to manually fix the empty number bug.";--field2name="Meta Commands";--field2value="`{guild.prefix}cookie changelog` to get the latest changelog.\n`{guild.prefix}cookie help` to display this message.";--title=":cookie: Cookie Help :cookie:";--color="#8e715a";--footer="Version {get;version}, Created by Shylke#8325";--timestamp="true";--description="Cookies for everyone!"}}```
