# JDJB
个人自用最全主库，集合可用脚本，适用于青龙面板。

频道：https://t.me/KingRan521  拉库失败查看频道

拉库命令：

国内鸡：（TX云等）

修改青龙 config.sh 文件中的GithubProxyUrl参数为：
https://pd.zwc365.com/ 或 
https://pd.zwc365.com/cfworker/

然后拉库命令填写下方代码：

国外鸡：

ql repo https://github.com/KingRan/JDJB.git "jd_|jx_|jdCookie" "activity|backUp" "^jd[^_]|USER|utils|function|sign|sendNotify|ql|JDJR"

出现拉取失败的进入容器→进入repo文件夹→删除整个库文件夹→重新拉取


1、搬运整理，感谢所有原作者。

2、个人学习目的，请下载后24小时内删除下载的代码。


1.出现这种错误：

Cannot find module 'xxxx'

依赖不完整，解决方法：

docker exec -it qinglong(容器名称) bash

cd /ql/scripts/

pnpm install 'xxxx'

npm install 'xxxx'

这两个安装命令都可以用

2.出现这种错误：

Cannot find module './xxxx'

那就很有是拉库命令不完整，请检查或复制完整的拉库命令。

部分需要的依赖：自行安装

"npm install -g npm"

"pip3 install requests"

"pip3 install pytz"

"npm install -g download"

"pnpm install jsdom"

"apk add --no-cache build-base g++ cairo-dev pango-dev giflib-dev && cd scripts && npm install canvas png-js md5 date-fns axios crypto-js tslib ts-md5 @types/node --build-from-source"

