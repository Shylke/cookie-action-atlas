**Command Name:** `a!cookie`

**Subcommand Name:** `a!cookie check`

**Command Description:**
Check how many cookies you, or another user, have.

**Usage:**
`a!cookie check <user>` (leave the user part blank if you want to check the amount of your cookies.)

**Code:**
```{if;{args;1};==;check;{a!say;**{user.tag;{args;2}}** has :cookie:{perget;{user.id;{args;2}}_Balance} cookie(s)!};}```
