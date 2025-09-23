# BGI游戏引擎脚本反汇编/汇编工具

这是一套用于 BGI (Buriko General Interpreter) / Ethornell 游戏引擎脚本文件的反汇编和汇编工具，可以帮助您分析和修改BGI引擎游戏的脚本函数和参数等。

## 分支说明

这里是巧克甜恋3的特殊版本，仅做了剧情脚本的汇编器修正（反汇编正常），bp文件没有处理。

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

注意：汇编后要使用16进制编辑器（比如010 Editor）进行魔术头修复（复制贴贴原版的内容，缺啥补啥就行）

然后将修好的剧情脚本文件放在游戏同根目录下就可以加载了

## 作者

[Imavoyc](https://github.com/Imavoyc)
[KlparetlR](https://github.com/KlparetlR)

## 许可

[MIT](https://github.com/KlparetlR/Bgi_asdis/blob/main/LICENSE)