**Command Name:** `a!cookie`

**Subcommand Name:** `a!cookie award`

**Command Description:**
Award a user with cookies.

**Usage:**
`a!cookie award <user> <amount>` or `a!cookie award belly <user> <amount>`


**Code:**
```{if;{lower;{args;1}};==;award;{if;{user.roles};includes;{get;AdminID};{if;{lower;{args;2}};==;belly;{if;{catch;{user.id;{args;3}};Error};==;Error;The specified user doesn't exist. Make sure you haven't made a typo.;{if;{args;4};==;;Please specify the number to award!;{if;{find;{args;4};\d+};==;{args;4};{perset;{user.id;{args;3}}_Belly;{math;{perget;{user.id;{args;3}}_Belly}+{args;4}}}You fed **{user.tag;{args;3}}** {get;EmojiBal}**{args;4}** {if;{args;4};==;1;{get;NameBalS};{get;NameBalP}}.;That's not a valid number.}}};{if;{catch;{user.id;{args;2}};Error};==;Error;The specified user doesn't exist. Make sure you haven't made a typo.;{if;{args;3};==;;Please specify the number to award!;{if;{find;{args;4};\d+};==;{args;4};{perset;{user.id;{args;2}}_Balance;{math;{perget;{user.id;{args;2}}_Balance}+{args;3}}}You gave {get;EmojiBal}**{args;3}** {if;{args;3};==;1;{get;NameBalS};{get;NameBalP}} to **{user.tag;{args;2}}**.;That's not a valid number.}}}};You're not allowed to do that.};}```
