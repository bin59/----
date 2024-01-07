# vim 编辑时由于异常退出正在编辑的文件，再次编辑该文件时出现提示

<!-- <img src="../.img/vim编辑时由于异常退出正在编辑的文件，再次编辑该文件时出现提示.png" /> -->

![](https://gitee.com/binbin59/imgs/raw/master/Operating-system/Linux/Linux%E7%A2%B0%E5%88%B0%E7%9A%84%E9%97%AE%E9%A2%98/vim%E7%BC%96%E8%BE%91%E6%97%B6%E7%94%B1%E4%BA%8E%E5%BC%82%E5%B8%B8%E9%80%80%E5%87%BA%E6%AD%A3%E5%9C%A8%E7%BC%96%E8%BE%91%E7%9A%84%E6%96%87%E4%BB%B6%EF%BC%8C%E5%86%8D%E6%AC%A1%E7%BC%96%E8%BE%91%E8%AF%A5%E6%96%87%E4%BB%B6%E6%97%B6%E5%87%BA%E7%8E%B0%E6%8F%90%E7%A4%BA.png)

解决：[nginx 配置踩坑 Found a swap file by the name “.nginx.conf.swp“](https://blog.csdn.net/Lostcoders/article/details/125744646)

在 nginx 目录下输入 ls -a 会发现一个.nginx.conf.swp 文件
执行 rm -rf .nginx.conf.swp 命令删除该文件即可

```bash
    ls -a

    rm -rf .nginx.conf.swp
```
