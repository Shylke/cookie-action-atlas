**Command Name:** `a!cookie`

**Subcommand Name:** `a!cookie throw`

**Command Description:**
Get rid of cookies.

**Usage:**
`a!cookie throw`, `a!cookie throw all` or `a!cookie throw belly`, `a!cookie throw belly all`

**Code:**
```{if;{lower;{args;1}};==;throw;{set;throw;1}}
{if;{lower;{args;1}};==;throw;{if;{lower;{args;2}};==;all;{set;throw;2}};}
{if;{lower;{args;1}};==;throw;{if;{lower;{args;2}};==;belly;{set;throw;3}};}
{if;{lower;{args;1}};==;throw;{if;{lower;{args;2}};==;belly;{if;{lower;{args;3}};==;all;{set;throw;4}}};}```

```{if;{get;throw};==;1;{if;{perget;{user.id}_Balance};<=;0;:slight_frown: You don't have any cookies to throw away...;{perset;{user.id}_Balance;{math;{perget;{user.id}_Balance}-1}}:toilet: You threw away a cookie!};}
{if;{get;throw};==;2;{if;{perget;{user.id}_Balance};<=;0;:slight_frown: You don't have any cookies to throw away...;:toilet: You threw away {perget;{user.id}_Balance} cookie(s)!{perset;{user.id}_Balance;0}};}```

```{if;{get;throw};==;3;{if;{perget;{user.id}_Belly};<=;0;:slight_frown: You don't have any cookies to throw up...;{perset;{user.id}_Belly;{math;{perget;{user.id}_Belly}-1}}:nauseated_face: You threw up a cookie...};}
{if;{get;throw};==;4;{if;{perget;{user.id}_Belly};<=;0;:slight_frown: You don't have any cookies to throw up...;:nauseated_face: You threw away {perget;{user.id}_Belly} cookie(s)...{perset;{user.id}_Belly;0}};}```
