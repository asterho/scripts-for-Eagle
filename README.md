# scripts-for-Eagle  

为Eagle编写的油猴脚本，预定实现导入pixiv和booru图站图片功能

## 已实现  

### Pixiv  

在Pixiv页面上添加下载按键，Eagle启动后点击下载即可导入原图，并将页面上所有标签及标签翻译加入Eagle标签。因为没搞清页面的加载方式，暂且使用延迟一秒的方式添加。若在同一页面内打开其他图片，或使用前进后退，无法加载出按键。

* 现在下载图片会自动按照画师分类，优先搜索已有文件夹中最外层有无以对应昵称命名的文件夹，或者“画师”文件夹中有无对应子文件夹，均搜索不到则自动创建。
* 现在下载时会同时保存作者描述
* 现在下载全部会同时“一键三连”（下载、点赞、收藏）

### Danbooru

在收藏按键旁边添加下载按键，处于美观修改了收藏按键的样式（块级元素改为行内）

## 待更新

* 更换下载按钮添加方式
* 修复无法加载下载按钮的情况
* 增加复选框
* 编写gelbooru、konachan、yande.re下载脚本
