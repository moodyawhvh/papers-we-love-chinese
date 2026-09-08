# Scripts(脚本)

> 🌐 本文档由 [papers-we-love/papers-we-love](https://github.com/papers-we-love/papers-we-love) 翻译,英文原版见原项目。

用于处理仓库内容的脚本集合。

## 下载工具(Download Utility)
一个用于下载论文的便捷脚本。它会抓取各 README.md 文件中含有 PDF 链接的 URL,并把文件下载到对应的目录。

该下载工具是幂等的,可以安全地重复运行多次。

### 用法(Usage)
打开你顺手的终端,运行:

```bash
$ ./scripts/download.sh
```


可选:要只下载特定主题的论文,把对应目录名作为参数传入:

```bash
$ ./scripts/download.sh android concurrency
```
