**Command Name:** `a!cookie`

**Subcommand Name:** `a!cookie remove`

**Command Description:**
Remove cookies from a user's balance.

**Usage:**
`a!cookie remove <user> <amount>` or `a!cookie remove belly <user> <amount>`

**Code:**
```{if;{lower;{args;1}};==;remove;{if;{user.roles};includes;{get;AdminID};{if;{lower;{args;2}};==;belly;{if;{catch;{user.id;{args;3}};Error};==;Error;The specified user doesn't exist. Make sure you haven't made a typo.;{if;{args;4};==;;Please specify a number to remove!;{if;{find;{args;4};\d+};==;{args;4};{perset;{user.id;{args;3}}_Belly;{math;{perget;{user.id;{args;3}}_Belly}-{args;4}}}You emptied **{user.tag;{args;3}}**'s belly of {get;EmojiBal}**{args;4}** {if;{args;4};==;1;{get;NameBalS};{get;NameBalP}}.;Please specify a valid number.}}};{if;{catch;{user.id;{args;2}};Error};==;Error;The specified user doesn't exist. Make sure you haven't made a typo.;{if;{args;3};==;;Please specify a number to remove!;{if;{find;{args;3};\d+};==;{args;3};{perset;{user.id;{args;2}}_Balance;{math;{perget;{user.id;{args;2}}_Balance}-{args;3}}}You took {get;EmojiBal}**{args;3}** {if;{args;3};==;1;{get;NameBalS};{get;NameBalP}} away from **{user.tag;{args;2}}**.;Please specify a valid number.}}}};You're not allowed to do that.};}```
