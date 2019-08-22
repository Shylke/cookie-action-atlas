**Command Name:** `a!cookie`

**Subcommand Name:** `a!cookie eat`

**Command Description:**
Eat a cookie.

**Usage:**
`a!cookie eat` or `a!cookie eat all`

**Code:**
```{if;{lower;{args;1}};==;eat;{if;{perget;{user.id}_Balance};<=;0;:slight_frown: You don't have any cookies to eat...;{if;{lower;{args;2}};==;all; :cookie: You ate {perget;{user.id}_Balance} cookie(s)!{perset;{user.id}_Belly;{math;{perget;{user.id}_Belly}+{perget;{user.id}_Balance}}}{perset;{user.id}_Balance;{math;{perget;{user.id}_Balance}-{perget;{user.id}_Balance}}};{perset;{user.id}_Balance;{math;{perget;{user.id}_Balance}-1}}{perset;{user.id}_Belly;{math;{perget;{user.id}_Belly}+1}}:cookie: You ate a cookie!}};}```
