# migrate-hexo-to-mweb
这个脚本可以帮你把 hexo 中的 md 文件全部转成 mweb 中的笔记

[脚本地址为](https://github.com/imzhizi/migrate-hexo-to-mweb/blob/master/import.sh)

此项目使用了 gnu-sed 和 macOS 中的 date 命令, 用于字符串中字符的替换和文件UUID.

主要需要修改的地方在脚本的第 142 行, 需要把 `hexoSrcDir`、`mWebBase` 修改为与本机地址一致, MWeb 存在 iCloud 中建议先行移出.

笔记的名称是 hexo 的文件名, 在脚本的第 173 行可以自行调整.

在脚本的第 213 行和 218 行会分别插入 toc 标签和 readmore 标签 (静态博客有用), 大家可以根据需求自行开关.

大概是这样了, 想要通过 MWeb 管理静态博客, 我的 [mweb-theme-machi](https://github.com/imzhizi/mweb-theme-machi) 应该有帮助.