**Command Name:** `a!cookie`

**Subcommand Name:** `a!cookie give`

**Command Description:**
Give a user a cookie!

**Usage:**
`a!cookie give <user>` or `a!cookie give belly <user>`

**Code:**
```{if;{lower;{args;1}};==;give;{set;give;1}}
{if;{lower;{args;1}};==;give;{if;{lower;{args;2}};==;belly;{set;give;2}}}

{if;{get;give};==;1;{if;{user.id};==;{user.id;{args;2}};You can't give cookies to yourself!;{if;{catch;{user.id;{args;2}};Error};==;Error;The specified user doesn't exist. Make sure you haven't made a typo.;{perset;{user.id;{args;2}}_Balance;{math;{perget;{user.id;{args;2}}_Balance}+1}}**{user.username}** has given :cookie:1 cookie to {user.mention;{args;2}}!}}}
{if;{get;give};==;2;{if;{user.id};==;{user.id;{args;3}};You can't give cookies to yourself!;{if;{catch;{user.id;{args;3}};Error};==;Error;The specified user doesn't exist. Make sure you haven't made a typo.;{perset;{user.id;{args;3}}_Belly;{math;{perget;{user.id;{args;3}}_Belly}+1}}**{user.username}** has fed {user.mention;{args;3}} :cookie:1 cookie!}}}```
