# 安装软件

安装分为两部分, 分别是
1. 手动执行部分操作
2. 执行 setup.sh 脚本, 自动化配置主要软件.
   1. 由于本人水平有限, 脚本自动化执行过程中还有一些需要手动确认的地方. 有兴趣的大佬可以考虑使用 export 脚本优化安装过程
3. 手动配置一些收尾工作

## 准则
1. 使用 hosts 指定域名/别名访问而非直接使用IP地址
2. 注意区分 `~/.zshrc` 和 `/etc/profile` 的作用域, 然后在合适的地方写入环境变量

## 一些建议
1. 刚开始时, 总希望可以一次性配置完所有以后用到的, 后来才发现, 一步登天是最不切实际的幻想. 正确的做法是 满足目前使用即可, 遇到需要的软件再去安装. (有点像 奥卡姆剃刀原则 呢)
