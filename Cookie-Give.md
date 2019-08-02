**Command Name:** `a!cookie`

**Subcommand Name:** `a!cookie give`

**Command Description:**
Give a user a cookie!

**Usage:**
`a!cookie give <user>`

**Code:**
```{if;{args;1};==;give;{if;{user.id};==;{user.id;{args;2}};You can't give cookies to yourself!;{perset;{user.id;{args;2}}_Balance;{math;{perget;{user.id;{args;2}}_Balance}+1}}{a!say;{user.username} has given :cookie:1 cookie to {user.mention;{args;2}}!}};}```
