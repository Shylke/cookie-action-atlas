**Command Name:** `a!cookie`

**Alias:** `a!cookie help`

**Command Description:**
Displays a help message.

**Usage:**
`a!cookie help`or `a!cookie`

**Code:** ```{if;{lower;{args;1}};==;help;{if;{user.roles};includes;{get;AdminID};{set;help;2};{set;help;1}}}
{if;{lower;{args;1}};==;;{if;{user.roles};includes;{get;AdminID};{set;help;2};{set;help;1}}}```

```{if;{get;help};==;2;{a!ae;--field1name="Commands";--field1value="• `{guild.prefix}{get;NameAction} give <belly> <user>` to give a {get;NameBalS} to a user.\n• `{guild.prefix}{get;NameAction} steal <user>` to steal a user's {get;NameBalS}.\n• `{guild.prefix}{get;NameAction} eat <all>` to eat a {get;NameBalS}.\n• `{guild.prefix}{get;NameAction} throw <belly> <all>` to get rid of your {get;NameBalP}.\n• `{guild.prefix}{get;NameAction} sacrifice` to sacrifice a {get;NameBalS}!... and maybe get more {get;NameBalP} as well?\n• `{guild.prefix}{get;NameAction} check <belly> <user>` to check your {get;NameBalP}, or another user's {get;NameBalP}.";--field2name="Meta Commands";--field2value="• `{guild.prefix}{get;NameAction} changelog` to get the latest changelog.\n• `{guild.prefix}{get;NameAction} info` to see the dedicated site for this action.\n• `{guild.prefix}{get;NameAction} help` to display this message.";--field3name="Admin Commands";--field3value="• `{guild.prefix}{get;NameAction} award <belly> <user> <amount>` to award a user with {get;NameBalP}.\n• `{guild.prefix}{get;NameAction} remove <belly> <user> <amount>` to remove {get;NameBalP} from a user.\n• `{guild.prefix}{get;NameAction} set <belly> <user>` to set their {get;NameBalS} balance to a number of your choice.\n• `{guild.prefix}{get;NameAction} reset <belly> <user>` to reset their {get;NameBalS} balance back to zero.\n• `{guild.prefix}{get;NameAction} fix <belly> <user>` to manually fix a user's empty number bug. ";--field3inline;--title="{get;NameBalCS} Help";--color="#8e715a";--footer="Version {get;version}, Created by Shylke#8325";--timestamp="true";--description="{get;EmojiBal} {get;NameBalCP} for everyone!"}}```

```{if;{get;help};==;1;{a!ae;--field1name="Commands";--field1value="• `{guild.prefix}{get;NameAction} give <belly> <user>` to give a {get;NameBalS} to a user.\n• `{guild.prefix}{get;NameAction} steal <user>` to steal a user's {get;NameBalS}.\n• `{guild.prefix}{get;NameAction} eat <all>` to eat a {get;NameBalS}.\n• `{guild.prefix}{get;NameAction} throw <belly> <all>`to get rid of your {get;NameBalP}.\n• `{guild.prefix}{get;NameAction} sacrifice` to sacrifice a {get;NameBalS}!... and maybe get more {get;NameBalP} too?\n• `{guild.prefix}{get;NameAction} check <belly> <user>` to check your {get;NameBalP}, or another user's {get;NameBalP}.";--field2name="Meta Commands";--field2value="• `{guild.prefix}{get;NameAction} changelog` to get the latest changelog.\n• `{guild.prefix}{get;NameAction} info` to see the dedicated site for this action. \n• `{guild.prefix}{get;NameAction} help` to display this message.";--title="{get;NameBalCS} Help";--color="#8e715a";--footer="Version {get;version}, Created by Shylke#8325";--timestamp="true";--description="{get;EmojiBal} {get;NameBalCP} for everyone!"}}```
