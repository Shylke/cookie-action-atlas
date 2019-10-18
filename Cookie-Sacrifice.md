**Command Name:** `a!cookie`

**Subcommand Name:** `a!cookie sacrifice`

**Command Description:**
Sacrifice a cookie!... and maybe get more cookies as a reward too?

**Usage:**
`a!cookie sacrifice


**Code:** ```{set;sacrifice;{choose;You sacrificed a cookie to the mighty god of cookies!;You gave **Shylke#8325** a cookie for the effort they put into the cookie commands!;Do you wanna have a bad time? No you don't, so sacrifice that cookie.;:volcano: You threw a cookie into a volcano... Why did you do it?;You donated a cookie to the hungry people!}}```

```{if;{lower;{args;1}};==;sacrifice;{if;{perget;{user.id}_Balance};<=;0;:slight_frown: You can't make a sacrifice without a cookie.;{perset;{user.id}_Balance;{math;{perget;{user.id}_Balance}-1}}:cookie: {get;sacrifice} {if;{range;0;100};>=;50;{set;reward;{range;2;5}}{perset;{user.id}_Balance;{math;{perget;{user.id}_Balance}+{get;reward}}}You got **{get;reward}** cookies as a reward!}}}```
