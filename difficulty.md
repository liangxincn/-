## 关于境内坑存在的访问困难

境内访问本站（本站内容是托管在github.com上）可能会有访问困难，其原因在于境内可能存在的DNS污染，所以，可以通过修改系统*host*文件解决:

Mac的host文件位置为：

```
/etc/hosts
```

Windows的host文件位置为：

```
c:\Windows\System32\drivers\etc\hosts
```

在host文件中添加以下内容：

```
192.30.253.112     github.com
185.199.111.153    assets-cdn.github.com
151.101.193.194    github.globel.ssl.fastly.net
```

如此这般之后，理论上访问困难就可以解决了。（备注：我个人做过测试，笑来老师之前的这些地址有时候已经无法用了，毕竟这是2019年成书时的测试地址）

