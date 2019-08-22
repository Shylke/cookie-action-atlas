**Command Name:** `a!cookie`

**Subcommand Name:** `a!cookie steal`

**Command Description:**
Steal a cookie from a user!

**Usage:**
`a!cookie steal <user>`

**Code:**
```{if;{lower;{args;1}};==;steal;{if;{user.id};==;{user.id;{args;2}};You can't take cookies away from yourself!;{if;{perget;{user.id;{args;2}}_Balance};<=;0;:slight_frown: You can't take steal from someone who doesn't have them in the first place...;{if;{range;0;100};>=;50;{perset;{user.id;{args;2}}_Balance;{math;{perget;{user.id;{args;2}}_Balance}-1}}{perset;{user.id}_Balance;{math;{perget;{user.id}_Balance}+1}}{user.username} has stolen :cookie:1 cookie from {user.mention;{args;2}}!;You failed to steal a cookie from {user.mention;{args;2}}...}}};}```
