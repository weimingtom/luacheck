https://github.com/Malcolm3141/brackets-luacheck


weimingtom 
2017-4-30 05:42 来自 微博 weibo.com
搞明白怎么在windows xp下运行luacheck，首先用Mingw编译lua-5.3.4，然后把exe放到bin目录，再把src目录下的luacheck文件夹复制到bin目录下。此时因为同时存在luacheck.lua和luacheck文件夹，所以需要把luacheck.lua改名成luacheck_bat.lua，相应也修改luacheck.bat里面的内容，最后运行luacheck.bat即可（后面接文件名作为参数）

weimingtom 
2017-4-6 10:44 来自 微博 weibo.com
不过感觉上Luacheck的检查可能会很死，例如function前面不加local会发出警告，但是要全部function前面都加local估计就觉得很繁琐了，好不好用还是很难说。。。

weimingtom
2017-4-6 10:41 来自 微博 weibo.com
成功在brackets上运行luacheck，效果是这样，我用的插件好像会报错，
https://github.com/Malcolm3141/brackets-luacheck
所以注释掉有问题的js代码才能成功安装运行，至于windows版的luacheck在github上有，在luacheck仓库的release那里（好像只有最新版才有编译版的exe），
https://github.com/mpeterv/luacheck/releases
下载后把exe添加到PATH目录即可。使用方法是点击右下角的lint区域就会弹出警告列表
