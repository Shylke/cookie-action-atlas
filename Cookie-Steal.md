**Command Name:** `a!cookie`

**Subcommand Name:** `a!cookie steal`

**Command Description:**
Steal a cookie from a user!

**Usage:**
`a!cookie steal <user>`

**Code:**
```{if;{lower;{args;1}};==;steal;{if;{user.id};==;{user.id;{args;2}};You can't take {get;NameBalP} away from yourself!;{if;{perget;{user.id;{args;2}}_Balance};<=;0;:slight_frown: You can't steal {get;NameBalP} from someone who doesn't have them in the first place...;{if;{catch;{user.id;{args;2}};Error};==;Error;The specified user doesn't exist. Make sure you haven't made a typo.;{if;{range;0;100};>=;50;{perset;{user.id;{args;2}}_Balance;{math;{perget;{user.id;{args;2}}_Balance}-1}}{perset;{user.id}_Balance;{math;{perget;{user.id}_Balance}+1}} **{user.username}** has stolen {get;EmojiBal}**1** {get;NameBalS} from {user.mention;{args;2}}!;You failed to steal a {get;NameBalS} from {user.mention;{args;2}}...}}}};}```
