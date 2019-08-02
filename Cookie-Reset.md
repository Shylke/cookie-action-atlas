**Command Name:** `a!cookie`

**Subcommand Name:** `a!cookie reset`

**Command Description:**
Reset a user's cookie balance.

**Usage:**
`a!cookie reset <user>` (leave the user part blank if you want to reset your cookie's balance.)

**Code:**
```{if;{args;1};==;reset;{if;{user.roles};includes;606515235591028756;{perset;{user.id;{args;2}}_Balance;0}You resetted **{user.tag;{args;2}}**'s cookie balance.;You're not allowed to do that.};}```
