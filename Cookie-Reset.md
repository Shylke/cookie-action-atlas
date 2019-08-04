**Command Name:** `a!cookie`

**Subcommand Name:** `a!cookie reset`

**Command Description:**
Reset a user's cookie balance.

**Usage:**
`a!cookie reset <user>` or `a!cookie reset belly <user>` (leave the user part blank if you want to reset your cookie's balance.)

**Code:**
```{if;{args;1};==;reset;{if;{user.roles};includes;606515235591028756;{if;{args;2};==;belly;{perset;{user.id;{args;3}}_Belly;0}You emptied **{user.tag;{args;3}}**'s belly.;{perset;{user.id;{args;2}}_Balance;0}You resetted **{user.tag;{args;2}}**'s cookie balance.};You're not allowed to do that.}}```
