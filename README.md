# scripts-for-Eagle  

为Eagle编写的油猴脚本，预定实现导入pixiv和booru图站图片功能

## 已实现

所有脚本默认保存标签，若不需要请将脚本中saveTags项改为false

### Pixiv  

在Pixiv页面上添加下载按键，Eagle启动后点击下载即可导入原图，并将页面上所有标签及标签翻译加入Eagle标签。  
在首页图片上添加下载按键，因未知原因无法绘制SVG图标，暂使用文字替代，有机会再优化

* 现在下载图片会自动按照画师分类，优先搜索已有文件夹中最外层有无以对应昵称命名的文件夹，或者“画师”文件夹中有无对应子文件夹，均搜索不到则自动创建。
* 现在下载时会同时保存作者描述（eagle2.0版本以上生效）
* 现在下载全部会同时“一键三连”（下载、点赞、收藏）

### Danbooru

#### posts

在收藏按键旁边添加下载按键，处于美观修改了收藏按键的样式（块级元素改为行内）

* 若属于pool，下载按pool创建文件夹，若最外层存在同名文件夹，则不创建并直接下载到同名文件夹中
* 下载时同时保存所有tag

#### pools

在标题下方添加下载按键

* 按pool名创建文件夹，若最外层有同名文件夹，则不创建并下载到同名文件夹中
* 下载时保存所有tag
* 下载时将图片来源修改为danbooru上标记的来源

### Gelbooru

仅在posts图片下方添加download按键，下载时保存标签，不创建文件夹

### yande. re

在posts图片下方添加下载按键，下载时保存标签，若图片属于某个pool则以pool名创建文件夹。未在pool中添加一键下载全部。

### konachan

同上

## 待更新

### Pixiv已知问题

* 更换下载按钮添加方式
* 修复无法加载下载按钮的情况
* 增加复选框
