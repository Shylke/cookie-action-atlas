**Command Name:** `a!cookie`

**Subcommand Name:** `a!cookie eat`

**Command Description:**
Eat a cookie.

**Usage:**
`a!cookie eat`

**Code:**
```{if;{args;1};==;eat;{if;{perget;{user.id}_Balance};<=;0;:slight_frown: You don't have any cookies to eat...;{perset;{user.id}_Balance;{math;{perget;{user.id}_Balance}-1}}{perset;{user.id}_Belly;{math;{perget;{user.id}_Belly}+1}}:cookie: You ate a cookie!};}{if;{perget;{user.id}_Belly};==;100;{user.addrole;606864358995263596} You now have the **Cookie Lover** role!}```
