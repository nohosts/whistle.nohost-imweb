# whistle.nohost-imweb
> 【重要提醒】本插件只是一个模板，不能直接使用，主要是方便大家快速开发本地连接 nohost 的 whistle 插件，具体用途参见[开发文档](./dev.md)。

访问 nohost 的 whistle 插件，安装此插件前确保你本地运行的 [whistle](https://github.com/avwo/whistle) 为最新版本（`>= v2.3.1`）。
> 需要用到 `v2.3.1` 及以上版本的 whistle，主要是因为项目的 `rules.txt` 里面用到了占位符 `{{whistlePluginPackage.pluginHomepage}}` 自动从插件的 `package.json` 的 `pluginHomepage` 获取值，如果需要兼容低版本，可以直接手动替换即可。

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
