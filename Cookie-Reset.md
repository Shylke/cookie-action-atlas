**Command Name:** `a!cookie`

**Subcommand Name:** `a!cookie reset`

**Command Description:**
Reset a user's cookie balance.

**Usage:**
`a!cookie reset <user>` or `a!cookie reset belly <user>` (leave the user part blank if you want to reset your cookie's balance.)

**Code:**
```{if;{lower;{args;1}};==;reset;{if;{user.roles};includes;{get;AdminID};{if;{lower;{args;2}};==;belly;{if;{catch;{user.id;{args;3}};Error};==;Error;The specified user doesn't exist. Make sure you haven't made a typo.;{a!say;Do you wish to reset **{user.tag;{args;3}}**'s belly balance? If so, type `yes`. You have 30 seconds.}{if;{lower;{channel.awaitMessage;{user.id};30}};===;yes;{perset;{user.id;{args;3}}_Belly;0}You emptied **{user.tag;{args;3}}**'s belly.;:x: Command has been stopped.}};{if;{catch;{user.id;{args;2}};Error};==;Error;The specified user doesn't exist. Make sure you haven't made a typo.;{a!say;Do you wish to reset **{user.tag;{args;2}}**'s balance? If so, type `yes`. You have 30 seconds.}{if;{lower;{channel.awaitMessage;{user.id};30}};===;yes;{perset;{user.id;{args;2}}_Balance;0}You resetted **{user.tag;{args;2}}**'s {get;NameBalS} balance.;:x: Command has been stopped.}}};You're not allowed to do that.}}```
