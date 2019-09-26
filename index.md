# My Cheatsheet

## Systemd

*what services are enabled?*

```bash
systemctl list-unit-files | grep enabled
systemctl list-unit-files --state=enabled
```


## Git

*preventing git to use ssl*

```bash
git config --global http.sslVerify false
```

# Vi

```bash
vi :tabe :Ex
```
```bash
Ctrl-v or Ctrl-q --> vi Block
```
