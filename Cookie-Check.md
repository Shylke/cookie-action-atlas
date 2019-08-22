**Command Name:** `a!cookie`

**Subcommand Name:** `a!cookie check`

**Command Description:**
Check how many cookies you, or another user, have.

**Usage:**
`a!cookie check <user>` or `a!cookie check belly <user>` (leave the user part blank if you want to check the amount of your cookies.)

**Code:**
```{if;{lower;{args;1}};==;check;{if;{lower;{args;2}};==;belly;**{user.username;{args;3}}** has eaten :cookie:{perget;{user.id;{args;3}}_Belly} cookie(s) in total!;**{user.username;{args;2}}** has :cookie:{perget;{user.id;{args;2}}_Balance} cookie(s)!};}```
