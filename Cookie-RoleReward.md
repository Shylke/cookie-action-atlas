**Command Name:** `a!cookie`

**Subcommand Name:** none

**Command Description:**
Gives you a role after eating a certain amount of cookies.

**Usage:**
None, just eat <X amount of> cookies and it should automatically reward you with the role. The amount variable can be found in `Variables.md`, or at the top of the script box in the dashboard.


**Code:** ```{if;{get;RoleRewardID};!==;;{if;{user.roles};!includes;{get;RoleRewardID};{if;{perget;{user.id}_Balance};>=;{get;BalanceAmount};{user.addrole;{get;RoleRewardID}}{a!say;You now have the **{role.name;{get;RoleRewardID}}** role!};{user.removerole;{get;RoleRewardID}}};}}```

```{if;{get;RoleRewardBellyID};!==;;{if;{user.roles};!includes;{get;RoleRewardBellyID};{if;{perget;{user.id}_Belly};>=;{get;BellyAmount};{user.addrole;{get;RoleRewardBellyID}}{a!say;You now have the **{role.name;{get;RoleRewardBellyID}}** role!};{user.removerole;{get;RoleRewardBellyID}}};}}```
