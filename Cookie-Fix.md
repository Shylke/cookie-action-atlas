**Command Name:** `a!cookie`

**Subcommand Name:** `a!cookie fix`

**Command Description:**
Fix the empty number bug.

**Usage:**
`a!cookie fix`


**Code:**
```{if;{lower;{args;1}};==;fix;{if;{lower;{args;2}};==;belly;{if;{perget;{user.id}_Belly};==;;{perset;{user.id}_Belly;0}Your belly balance has been corrected, run `{guild.prefix}cookie check belly` to see the results.;:mag: Your belly balance doesn't seem to have any bug. {if;{perget;{user.id}_Balance};includes;-;Though you might want to notice it's less than zero.}};{if;{perget;{user.id}_Balance};==;;{perset;{user.id}_Balance;0}Your cookie balance has been corrected, run `{guild.prefix}cookie check` to see the results.;:mag: Your cookie balance doesn't seem to have any bug. {if;{perget;{user.id}_Balance};includes;-;Though you might want to notice it's less than zero.}}}}```
