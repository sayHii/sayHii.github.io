# Ubuntu 删除用户

linux 命令，添加 `--remove-home` 参数可同时删除用户目录。

```
sudo deluser --remove-home ${userName}
```

删除用户后，同时删除 `sudo` 信息，提高安全性。

```
cd /etc/sudoers.d/
```

有些场景可能不太规范，需要直接修改 `soduers` 文件。

```
vi /etc/sudoers
```