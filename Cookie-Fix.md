**Command Name:** `a!cookie`

**Subcommand Name:** `a!cookie fix`

**Command Description:**
Fix the empty number bug.

**Usage:**
`a!cookie fix`


**Code:**
```{if;{lower;{args;1}};==;fix;{if;{user.roles};includes;{get;AdminID};{set;fix;true};You're not allowed to do that.}}
{if;{get;fix};==;true;{if;{args;2};==;;You need to mention someone! {set;fixed;false};{set;fixed;1}}}
{if;{get;fix};==;true;{if;{lower;{args;2}};==;belly;{if;{args;3};==;;You need to mention someone!{set;fixed;false};{set;fixed;2}};}}
{if;{get;fixed};==;1;{if;{perget;{user.id;{args;2}}_Balance};==;;{perset;{user.id;{args;2}}_Balance;0}**{user.tag;{args;2}}**'s cookie balance has been corrected, run `{guild.prefix}cookie check {user.tag;{args;2}}` to see the results.;:mag: **{user.tag;{args;2}}**'s cookie balance doesn't seem to have any bug. {if;{perget;{user.id;{args;2}}_Balance};includes;-;Though you might want to let them know it's less than zero.}}{set;fixed;0}}```
{if;{get;fixed};==;2;{if;{perget;{user.id;{args;3}}_Belly};==;;{perset;{user.id;{args;3}}_Belly;0}**{user.tag;{args;3}}**'s cookie balance (belly) has been corrected, run `{guild.prefix}cookie check belly {user.tag;{args;3}}` to see the results.;:mag: **{user.tag;{args;3}}**'s cookie balance (belly) doesn't seem to have any bug. {if;{perget;{user.id;{args;3}}_Belly};includes;-;Though you might want to let them know it's less than zero.}}}```

