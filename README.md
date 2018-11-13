# Tunet.Auth

tunetAuth is a python script to login https://auth4.tsinghua.edu.cn and(or) https://auth6.tsinghua.edu.cn
this script use selenium firefox headless to login

```bash
// do login
tunetAuth 

// do logout
tunetAuth -o
```
tunetAuth will use ~/.TsinghuaNet/netTHUAuth
```json
{
  "username": "username",
  "password": "password"
}
```

if you want login in automatically, you can
```bash
ping -c 1 -W 1 info.tsinghua.edu.cn >/dev/null 2>&1 || tunetAuth 
```
and add it to crontab

Enjoy it.
