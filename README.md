# 生成文档网站 (零配置极简版)

## 构建过程

1. 复制 .github 文件到你的项目根目录上 (主要使用 `.github/workflows/static.yml`)。此时commit后就会自动构建啦，可能需要稍等一段时间 (在顶部栏中的actions可以看到进度)，等待构建完成后进行下一步。
2. github的项目页中，以此选择：setting > page > 启用page，并将branch设置为 `gh-pages`，如下图所示。当启用page后，你就可以通过该图中上面给出的链接来访问你的网站了！
  
  ![alt text](./assets/6a664307563c3775cb5c78cd1f3fbc13.png)

## FAQ (常见问题)

- 为什么我在第二步中没看到 `gh-pages` 分支？
  需要等待构建完成（在顶部栏中的actions可以看到进度，绿色为构建成功，黄色正在构建，红色为构建失败）
- 为什么我在setting中没有看到 page 选项？
  page选项需要是 yourUserName.github.io 的仓库地址或者 organization 内的项目，才有page选项。如果没有，要么将你的仓库位置修改成这些允许有page的位置，要么使用另一套方案（详情搜issue：分离文档仓库与构建系统仓库）
- 报错说分支不对/你的主分支不是main？
  修改yml文件，将里面的分支 `main` 修改为你现在的分支名即可
- 什么时候会自动更新内容？
  正常commit后，会自动进行文档构建，构建结束后就会自动更新网站内容
- 如何使用非github.io部署？
  略，提issue，有人问我再回
- 我没有在这里找到我的问题？
  在issue中搜索看是否有人问过相同的问题，看是否能解决。若没有，则提issue
