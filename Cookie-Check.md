**Command Name:** `a!cookie`

**Subcommand Name:** `a!cookie check`

**Command Description:**
Check how many cookies you, or another user, have.

**Usage:**
`a!cookie check <user>` or `a!cookie check belly <user>` (leave the user part blank if you want to check the amount of your cookies.)

**Code:**
```{if;{lower;{args;1}};==;check;{if;{lower;{args;2}};==;belly;{if;{catch;{user.id;{args;3}};Error};==;Error;The specified user doesn't exist. Make sure you haven't made a typo.;**{user.username;{args;3}}** has eaten {get;EmojiBal}**{perget;{user.id;{args;3}}_Belly}** {if;{perget;{user.id;{args;3}}_Belly};==;1;{get;NameBalS};{get;NameBalP}} in total! {if;{perget;{user.id}_Belly};includes;-;They must be too poor to get a {get;NameBalS}! :cry:}};{if;{catch;{user.id;{args;2}};Error};==;Error;The specified user doesn't exist. Make sure you haven't made a typo.;**{user.username;{args;2}}** has {get;EmojiBal}**{perget;{user.id;{args;2}}_Balance}** {if;{perget;{user.id;{args;2}}_Balance};==;1;{get;NameBalS};{get;NameBalP}}! {if;{perget;{user.id}_Balance};includes;-;They must be too poor to get a {get;NameBalS}! :cry:}}};}```
