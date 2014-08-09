polymer_docs_nginx
==================
前提条件：

- 编译环境ok（可以没有GAE）,需要能够通过`grunt --force` 完成`_site`的生成

nginx站点配置文件

- 参见 [c0710204/polymer_docs_nginx] ( https://github.com/c0710204/polymer_docs_nginx )

使用方法：

1. 将`docs_site.nginx`放入你的nginx站点文件夹(sites-available)或者加入您的nginx.conf中

2. 替换$polymer_docs_root为你的polymer/docs根路径(git路径)

3. 修改你的polymer/docs根路径(git路径)的权限使nginx所用账户可以访问文件

4. 改端口号40000为你想要的端口号

5. reload或restart你的nginx

编写/修改i方法：

对于每条app.yaml中的配置,均可直接转换成nginx的rewrite配置,只需注意nginx的正则替换为类似`$1`而非`\1`
请注意修改时规则的顺序以防止错误的匹配

