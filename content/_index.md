---
title: xxx 的文档
titleOnly: true
weight: 1
bookToc: false
---

# 文档模板

阅读地址：<https://os2c.github.io>

仓库地址：<https://github.com/os2c/os2c.github.io>

## 添加/更新文档

在 `content/` 目录添加或者更新文档。

以下是一些 make 命令简化流程：

* `make new doc=design/hi.md`：从模板中创建 `content/design/hi.md` 文件
* `make serve`：本地预览文档
  * 如需修改地址和端口，使用 `make serve BIND=xxx PORT=xxx`
* `make generate`：在 public 目录中生成静态网页
  * 通常需要 baseURL 调整地址：`make generate baseURL=your-url`

注意：make 命令将把 README.md 的内容复制到 `content/_index.md`，以保持生成的网页主页与 README 内容一致。
