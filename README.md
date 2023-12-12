# dev_stataRH8
Stata deployment and development on RH8

#### Ncurses Error when running command-line stata-mp or stata - Missing libncruses.so.5 on RHEL 8
- Fix <br/>
```
$sudo dnf install -y ncurses-compat-libs
```

#### Passing Values by Reference like Passwords
- Create a file to save your username and password <br/>
```
local myuid MyUserID
local mypwd MyPassword
```

- Reference the file in Stata <br/>
```
quietly include ~/<filename_with_info>

uid(`myuid;) password(`mypwd')
```
