**Command Name:** `a!cookie`

**Subcommand Name:** `a!cookie remove`

**Command Description:**
Remove cookies from a user's balance.

**Usage:**
`a!cookie remove <user> <amount>` or `a!cookie remove belly <user> <amount>`

**Code:**
```{if;{args;1};==;remove;{if;{user.roles};includes;606515235591028756;{if;{args;2};==;belly;{perset;{user.id;{args;3}}_Belly;{math;{perget;{user.id;{args;3}}_Belly}-{args;4}}}You emptied **{user.tag;{args;3}}**'s belly of :cookie:{args;4} cookie(s).;{perset;{user.id;{args;2}}_Balance;{math;{perget;{user.id;{args;2}}_Balance}-{args;3}}}You took :cookie:{args;3} cookie(s) away from **{user.tag;{args;2}}**.};You're not allowed to do that.};}```
