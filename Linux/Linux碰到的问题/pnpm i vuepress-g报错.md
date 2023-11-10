# pnpm i vuepress -g报错
报错信息：

```bsah

ERR_PNPM_NO_GLOBAL_BIN_DIR  Unable to find the global bin directory

Run "pnpm setup" to create it automatically, or set the global-bin-dir setting, or the PNPM_HOME env variable. The global bin directory should be in the PATH.
```

原因：

npm 安装 pnpm的时候没有执行配置环境变量的命令


解决：

1. 
```bash
pnpm setup
```
2.
```bash
source ~/.bashrc
```

再次运行：`pnpm i vuepress -g`即可
