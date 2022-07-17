# c_7731
宅男导航源码整站打包分享源码 分类信息导航网站源码
<br/></br>
[下载地址](https://www.uuid2.com/7731.html "下载地址")
<br/></br>
<h3>源码简介：</h3>
<p>安装说明：
宝塔Nginx -Tengine2.2.3的PHP5.6 + MySQL5.6.44
先导入数据库文件.sql
再修改config.php数据库配置
然后服务器设置好伪静态规则
访问网站OK
后台是：你的域名/admin/login.php 账号：admin 密码：123456
Nginx伪静态规则
rewrite ^/index.html$ /index.php;
rewrite ^/about.html$ /about.php;
rewrite ^/search.html$ /search.php;
rewrite ^/ranking.html$ /ranking.php;
rewrite ^/wz.html$ /wzall.php;
rewrite ^/apply.html$ /apply.php;
rewrite ^/404.html$ /404.php;
rewrite ^/sort([1-9]+[0-9]*).html$ /sort.php?id=$1;
rewrite ^/sort([a-zA-Z]+).html$ /sort.php?alias=$1;
rewrite ^/site_([1-9]+[0-9]*).html$ /site.php?id=$1;
rewrite ^/wz([1-9]+[0-9]*).html$ /wz.php?id=$1;
rewrite ^/wzshow_([1-9]+[0-9]*).html$ /wzshow.php?id=$1;
Apache伪静态规则
RewriteEngine On
rewritebase /
RewriteRule ^index.html /index.php [L,NC]
RewriteRule ^about.html about.php [L,NC]
RewriteRule ^search.html search.php [L,NC]
RewriteRule ^ranking.html ranking.php [L,NC]
RewriteRule ^wz.html wzall.php [L,NC]
RewriteRule ^apply.html apply.php [L,NC]
RewriteRule ^404.html 404.php [L,NC]
RewriteRule ^sort([0-9]+).html sort.php?id=$1 [L,NC]
RewriteRule ^sort([a-zA-Z]+).html sort.php?alias=$1 [L,NC]
RewriteRule ^site_([0-9]+).html site.php?id=$1 [L,NC]
RewriteRule ^wz([0-9]+).html wz.php?id=$1 [L,NC]
RewriteRule ^wzshow_([0-9]+).html wzshow.php?id=$1 [L,NC]<p>
<h3>截图：</h3>
<img src="https://www.uuid2.com/wp-content/uploads/img/uimage/68061646965148.gif" alt="宅男导航源码整站打包分享源码 分类信息导航网站源码">
