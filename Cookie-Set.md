**Command Name:** `a!cookie`

**Subcommand Name:** `a!cookie set`

**Command Description:**
For setting a user's balance when you're too lazy to do the math.

**Usage:**
`a!cookie set <user> <amount>` or `a!cookie set belly <user> <amount>`


**Code:**
```{if;{lower;{args;1}};==;set;{if;{user.roles};includes;{get;AdminID};{if;{lower;{args;2}};==;belly;{if;{catch;{user.id;{args;3}};Error};==;Error;The specified user doesn't exist. Make sure you haven't made a typo.;{if;{args;4};==;;Please specify the number to set!;{if;{find;{args;4};\d+};==;{args;4};{perset;{user.id;{args;3}}_Belly;{args;4}}You set **{user.tag;{args;3}}**'s belly balance to {get;EmojiBal}**{args;4}** {if;{args;4};==;1;{get;NameBalS};{get;NameBalP}}.;That's not a valid number.}}};{if;{catch;{user.id;{args;2}};Error};==;Error;The specified user doesn't exist. Make sure you haven't made a typo.;{if;{args;3};==;;Please specify the number to set!;{if;{find;{args;3};\d+};==;{args;3};{perset;{user.id;{args;2}}_Balance;{args;3}}You set **{user.tag;{args;2}}**'s balance to {get;EmojiBal}**{args;3}** {if;{args;3};==;1;{get;NameBalS};{get;NameBalP}}.;That's not a valid number.}}}};You're not allowed to do that.};}```
