**Command Name:** `a!cookie`

**Subcommand Name:** `a!cookie give`

**Command Description:**
Give a user a cookie!

**Usage:**
`a!cookie give <user>` or `a!cookie give belly <user>`

**Code:**
```{if;{lower;{args;1}};==;give;{if;{user.id};==;{user.id;{args;2}};You can't give cookies to yourself!;{if;{args;2};==;belly;{if;{user.id};==;{user.id;{args;3}};You can't feed yourself cookies!;{perset;{user.id;{args;3}}_Belly;{math;{perget;{user.id;{args;3}}_Belly}+1}}**{user.username}** has fed {user.mention;{args;3}} :cookie:1 cookie!};{perset;{user.id;{args;2}}_Balance;{math;{perget;{user.id;{args;2}}_Balance}+1}}**{user.username}** has given :cookie:1 cookie to {user.mention;{args;2}}!}};}```
