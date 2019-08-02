**Command Name:** `a!cookie`

**Subcommand Name:** `a!cookie belly`

**Command Description:**
Check how many cookies you, or another user, have eaten.

**Usage:**
`a!cookie belly <user>` (leave the user part blank if you want to check the amount of the cookies you have eaten.)

**Code:**
```{if;{args;1};==;belly;{a!say;{user.username;{args;2}} has eaten :cookie:{perget;{user.id;{args;2}}_Belly} cookie(s) in total!};}
```
