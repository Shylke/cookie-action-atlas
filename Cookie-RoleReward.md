**Command Name:** `a!cookie`

**Subcommand Name:** none

**Command Description:**
Gives you a role after eating a certain amount of cookies.

**Usage:**
None, just eat 100 cookies and it should automatically reward you with the role.


**Code:** ```{if;{user.roles};!includes;606864358995263596;{if;{perget;{user.id}_Belly};>=;100;{user.addrole;606864358995263596} You now have the **Cookie Lover** role!;{user.removerole;606864358995263596}};}```
