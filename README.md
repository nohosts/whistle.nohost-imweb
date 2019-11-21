# whistle.nohost-imweb
访问 nohost 的 whistle 插件，安装此插件前确保你本地运行的 [whistle](https://github.com/avwo/whistle) 为最新版本。

# 安装或更新 whistle
``` sh
npm i -g whistle --registry=https://r.npm.taobao.org
w2 restart
```

# 安装插件
``` sh
w2 i whistle.nohost-imweb
```
> 也可以指定 registry：`w2 i whistle.nohost-imweb --registry=https://r.npm.taobao.org`
> 如果是公司内网用了 `tnpm` 或 `cnpm` 等 `xnpm` 命令，也可以采用：`w2 xi whistle.nohost-imweb`，其中 `x` 表示你们所使用的新 npm 命令前缀。

安装成功后，可以在 whistle 界面的 `Plugins` 列表看到 `nohost-imweb` 插件，插件默认处于启用状态，如果不需要可以禁用掉，这是插件的规则会自动被移除，更新插件只需重新安装下插件即可。
