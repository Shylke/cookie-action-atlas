**Command Name:** `a!cookie`

**Subcommand Name:** `a!cookie changelog`

**Command Description:**
Gets the latest changelog.

**Usage:**
`a!cookie changelog`


**Code:** 
```{if;{args;1};==;changelog;{a!ae;--title=":cookie: Cookie Command {get;version} Changelog :cookie:";--color="#8e715a";--footer="Created by Shylke#8325";--timestamp="true";--description="[**You can read the full changelog here**](https://github.com/Shylke/cookie-action-atlas/blob/master/CHANGELOG.md)."}}```
