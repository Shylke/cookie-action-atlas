**Command Name:** `a!cookie`

**Subcommand Name:** `a!cookie sacrifice`

**Command Description:**
Sacrifice a cookie!... and maybe get more cookies as a reward too?

**Usage:**
`a!cookie sacrifice`


**Code:** ```{set;sacrifice;{choose;You sacrificed a {get;NameBalS} to the god of {get;NameBalP}!;You gave **Shylke#8325** a {get;NameBalS} for the effort they put into the cookie commands!;Do you wanna have a bad time? No you don't, so sacrifice that {get;NameBalS}.;:volcano: You threw a {get;NameBalS} into a volcano... Why did you do it?;You donated a {get;NameBalS} to a random stranger!;You hurl the {get;NameBalS} into the sun, while chanting in a language only you understand.}}```

```{if;{lower;{args;1}};==;sacrifice;{if;{perget;{user.id}_Balance};<=;0;:slight_frown: You can't make a sacrifice without a {get;NameBalS}.;{perset;{user.id}_Balance;{math;{perget;{user.id}_Balance}-1}}{get;EmojiBal} {get;sacrifice} {if;{range;0;100};>=;50;{set;reward;{range;2;5}}{perset;{user.id}_Balance;{math;{perget;{user.id}_Balance}+{get;reward}}}You got {get;EmojiBal}**{get;reward}** {get;NameBalP} as a reward!}}}```
