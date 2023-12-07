# dev_stataRH8
Stata deployment and development on RH8

#### Ncurses Error when running command-line stata-mp or stata - Missing libncruses.so.5 on RHEL 8
- Fix <br/>
```
$sudo dnf install -y ncurses-compat-libs
```
