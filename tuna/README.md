https://tuna.moe/blog/2015/tex/

活动记录: TeX 与汉字处理

May 15, 2015. | By: Justin Wong

5 月的北京，夜晚的阵阵清风吹过宁静清华园，空气中飘荡着初夏的味道，这是发布新版本的季节！

2015 年 5 月 21 日，TUNA 协会邀请到了 pTex-ng 的作者 马起园(李阿玲)、 中文 TeX 文档类/宏包 CTeX-kit 的开发者 刘海洋 还有 TUNA 协会成员，ThuThesis 维护者 赵涛(Alick Zhao) 等人， 共同分享 TeX 与汉字处理的技术与应用，还有 pTeX-ng、CTeX 2.0、最新版 ThuThesis 特性的演示。

活动开始前不久，30人的小教室就几乎刚好坐满，既热闹，又没有距离感，新出炉的 TUNA 贴纸套装很受欢迎，会长带来的 100 张贴纸瞬间 发出了 50 张。



第一个话题是由 马起园带来的 pTeX-ng 细节介绍，马起园从 6 年前开始接触 TeX，但各类 TeX 引擎在处理汉字和 pdf 方面表现的并不 完美，而现存的一些能原生处理汉字的 TeX 引擎多是上世纪 80 年代开发，21 世纪后便鲜有维护了。在世界人民都期盼着能有更完美的 东亚语言 TeX 引擎出现的时候，马起园坚定的扛起了振兴东亚语言文字的大旗，基于 pTeX 和 Y&Y TeX 开始开发新一代 TeX 引擎， 命名为 pTeX-ng。（现今项目进一步升级，称为 asia pTeX 或 ApTex。）

文字排版引擎的细节问题非常多，马起园介绍了汉字排版的编码、字体等各类细节问题和 pTeX-ng 的解决方案，未来 pTeX-ng 也将发布新版并趋于稳定。由于 pTeX-ng 是一个底层引擎，一般用户并不需要知道它的存在，目前的几乎所有 LaTeX 解决 方案也都可以无缝接入。



第二个话题是来自隔壁北京大学的 刘海洋带来的 CTeX 2.0 新特性介绍。刘海洋幽默风趣地介绍了 LaTeX 处理汉字的血泪史， 从最早的 CCT 到后来的 CJK，直到 2007 年 XeLaTeX 发布后才稍微有所改观。但无论如何，用户排版中文都需要做非常多的 配置工作，不能做到开箱即用，体验很差。 CTeX 出现后，人们只需要使用

\documentclass{ctexart}
\begin{document}
这是一个普通的 \LaTeX{} 文档
\end{document}
即可得到完美的中文排版，做到了开箱即用，极大的方便了用户。但 CTeX 1.0 在 Linux 和 Mac OS X 上并不能直接工作， 仍然需要额外配置，并且一些配置命令格式不统一，也产生了一些困扰。CTeX 2.0 则通过 特征文件 黑科技实现了 操作系统智能判断，达到 Windows XP/7/8+, Linux 和 Mac OS X 的开箱即用，并且在配置命令等方面使用统一的 \ctexset 命令，进一步简化操作，引擎方面也支持了更先进的 luatexja，未来还会支持 pTeX-ng。



最后是 TUNA 成员，ThuThesis 维护者赵涛带来的 “ThuThesis 最新动态”。ThuThesis 上一次更新是 2011 年的 4.6 版， 该版本流传广泛，但也有很多 bug。2014 年，ThuThesis 发布了最新的 4.8.1 版，底层基于 CTeX 实现，转向 UTF-8 编码，增加了硕士论文英文封面等支持，兼容清华最新的学位论文排版标准，还修正了很多 bug。所以 2015 届毕业生，更应该 使用最新版 ThuThesis 撰写学位论文。而在进行中的 4.8.2 版会进一步修正 bug，计划中的 4.9 版会支持 CTeX 2.0，进一步 完善格式等。赵涛还列举了一些隐藏的坑，例如同一个字体不要安装多遍、参考文献不能为空等。最后，赵涛鼓励大家 多多到 ThuThesis 的 GitHub 反馈问题，帮助改进。

以下是本次演讲幻灯片列表:

* TeX与汉字处理: 过去、现在、未来 [下载](https://tuna.moe/assets/slides/doc-ptex-ng-zh.pdf)
* CTeX 2.0 : 新的开始 [下载](https://tuna.moe/assets/slides/ctex2talk.pdf)
* ThuThesis 最新动态 [下载](https://tuna.moe/assets/slides/thu-thesis-1.0.pdf)