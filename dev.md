想好名字（可以用团队或公司的英文名，名字只能包含小写字母、数字、中划线），假设你团队名字叫 `imwebtest`，clone nohost插件模版：
```
git clone https://github.com/nohosts/whistle.nohost-imweb.git whistle.nohost-imwebtest
```
项目 clone 到本地后，修改以下文件：

1. [package.json](./package.json)：
    * 把里面的 `nohost-imweb` 改成 `nohost-imwebtest`
    * 将 `pluginHomepage` 及 `whistleConfig/menuConfig/baseUrl` 改成自己的 nohost 域名及端口如： `http://imwebtest.oa.com:8080`
        > 即替换所有 `http://imwebtest.oa.com:8080`
2. [README.md](./README.md)：
    * 把里面的所有 `nohost-imweb` 替换成 `nohost-imwebtest`
    * 把里面的重要提醒删除

发布到 npm：
```
npm publish
```

发布后，即可通过安装插件的方式设置 nohost 代理：
``` txt
w2 i whistle.nohost-imwebtest
```
> 也可以指定 registry：`w2 i whistle.nohost-imwebtest --registry=https://r.npm.taobao.org` 如果是公司内网用了 tnpm 或 cnpm 等 xnpm 命令，也可以采用：`w2 xi whistle.nohost-imwebtest` ，其中 x 表示你们所使用的新 npm 命令前缀。

最后，记得把修改后的项目推送到自己的 Git 仓库。
  