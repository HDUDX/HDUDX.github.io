# 操作手册
本项目使用`hexo`+`stellar`搭建，毫无技术难点，只要你认真一定能接手这个项目的。

# 快速开始
安装`hexo`的依赖环境，如果你是windows那么需要你自己查阅资料，如果你是Linux，那么可以参考我的文章（如果它没失效的话）：[zhywyt'blog hexo+github搭建静态网站](https://zhywyt.github.io/posts/d8eb45be176b/)。运气好能看到它的。

克隆本项目，并切换到`source`分支：
```bash
// 跳过克隆步骤，如果git不会用那也挺难接手这个项目
git checkout -b source
```

你可能需要自己查阅[hexo文档](https://hexo.io/zh-cn/docs/)和[stellar文档](https://xaoxuu.com/wiki/stellar/#start)。加油吧，我相信你能做到的！

# 部署方式

我采用了前端+源文件分分支部署的形式，我们的`master`分支存储了我们每次的前端文件，而我们的`source`分支存储了我们的源代码文件，包括配置和md源代码，这有助于我们迁移我们的主页和文章，而不会因为我的离开而导致无法重新编译。请好好理解这个过程。

由于`hexo-deploy`插件的存在，导致我们可以简单的通过`hexo d`来将前端代码部署到github上，并自动运行action，所以你只需要在大版本更新的时候将源文件上传至source分支。千万注意，每次上传之前请`git fetch`或者`git pull`，总之，保持和远程版本一致是最合理最不容易出错的办法，希望你们能将这个网站越做越好，我只是抛砖的人，你们才是造玉者。

