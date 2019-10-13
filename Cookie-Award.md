**Command Name:** `a!cookie`

**Subcommand Name:** `a!cookie award`

**Command Description:**
Award a user with cookies.

**Usage:**
`a!cookie award <user> <amount>` or `a!cookie award belly <user> <amount>`


**Code:**
```{if;{lower;{args;1}};==;award;{if;{user.roles};includes;606515235591028756;{if;{lower;{args;2}};==;belly;{if;{catch;{user.id;{args;3}};Error};==;Error;The specified user doesn't exist. Make sure you haven't made a typo.;{perset;{user.id;{args;3}}_Belly;{math;{perget;{user.id;{args;3}}_Belly}+{args;4}}}You fed **{user.tag;{args;3}}** :cookie:{args;4} cookie(s).};{if;{catch;{user.id;{args;2}};Error};==;Error;The specified user doesn't exist. Make sure you haven't made a typo.;{perset;{user.id;{args;2}}_Balance;{math;{perget;{user.id;{args;2}}_Balance}+{args;3}}}You gave :cookie:{args;3} cookie(s) to **{user.tag;{args;2}}**.}};You're not allowed to do that.};}```
