# BGI游戏引擎脚本反汇编/汇编工具

这是一套用于 BGI (Buriko General Interpreter) / Ethornell 游戏引擎脚本文件的反汇编和汇编工具，可以帮助您分析和修改BGI引擎游戏的脚本函数和参数等。

## 功能概述

本工具集提供了两种主要功能：

1. **剧情脚本处理** - 以`bgi`开头的文件用于处理游戏的主要剧情脚本
   - bgidis.py: 剧情脚本反汇编器（该版本目前测试支持`bs5`的脚本文件，`bss`版本请以樱之诗分支（等代码上传）为基础）
   - bgias.py: 剧情脚本汇编器

2. **系统脚本处理** - 以`bp`开头的文件用于处理BGI引擎的系统脚本
   - bpdis.py: 系统脚本(._bp文件)反汇编器
   - bpas.py: 系统脚本(._bp文件)汇编器

## 文件说明

- asdis.py: 公共汇编/反汇编功能
- bgiop.py: BGI剧情脚本操作码表
- bpop.py: BGI系统脚本操作码表
- bgidis.py: 剧情脚本反汇编工具
- bgias.py: 剧情脚本汇编工具
- bpdis.py: 系统脚本反汇编工具
- bpas.py: 系统脚本汇编工具

## 使用方法

### 剧情脚本反汇编

```bash
python bgidis.py <文件名>
```

作用：将无扩展名的剧情脚本文件反汇编为.bsd文件

### 剧情脚本汇编

```bash
python bgias.py <文件名.bsd>
```

作用：将.bsd文件汇编回无扩展名的剧情脚本文件

### 系统脚本反汇编

```bash
python bpdis.py <文件名._bp>
```

作用：将._bp系统脚本文件反汇编为.bpd文件

### 系统脚本汇编

```bash
python bpas.py <文件名.bpd>
```

作用：将.bpd文件汇编回._bp系统脚本文件

## 注意事项

- 这是基础版本，**不保证兼容所有BGI引擎的游戏**，要保证反汇编后还能汇编回去，所以容错率较小，运行后报错是有概率的
- 用户可按需要根据特定游戏修改脚本代码
- 可查看本仓库的其他分支，了解更多针对特定游戏的定制版本

## 作者

[Imavoyc](https://github.com/Imavoyc)

## 贡献

如果您对特定BGI游戏有更好的支持方案，欢迎提交PR或者创建新的分支。

## 许可

[MIT](https://github.com/KlparetlR/Bgi_asdis/blob/main/LICENSE)

## 跨引擎移植实例

renpy：

 - [樱之诗](https://github.com/Imavoyc/Sakuranouta-RenPy-Part1)

 - [巧克甜恋3](https://b23.tv/RtmlI9c)

 - [向日葵的教会与长长的暑假](https://www.bilibili.com/video/BV1MTxtzkE2Z/)


