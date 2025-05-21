# 使用

安装环境

```bash
./install_env
```

使用 venv 环境

```bash
source venv/bin/activate
```

获取源码，指定包名

```bash
dbuilder source get <包名>
```

检查源码有没有依赖，没输出说明依赖没缺失。

```bash
dbuilder source dep <包名>
```

获取源码并做预处理

```bash
dbuilder source pre <包名>
```

设置推送分支，设置 none 时，默认推送到 master 分支，设置为其他分支名如 test，则推送到 topic-test 分支，后续属于 topic-test 分支的包会放到一个主题中，方便提测。

```bash
dbuilder hub branch <分支名>
```

设置关联的 issue，提交 commit 时会附上链接。设置为 none，commit 上不会添加链接。

```bash
dbuilder hub issue <issue 🔗>
```

推送代码到仓库

```bash
dbuilder hub push <>
```
