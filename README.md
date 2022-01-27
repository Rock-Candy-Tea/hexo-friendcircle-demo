# hexo-friendcircle-demo

这个仓库用于存放hexo友链朋友圈的演示页面以及js和css主题文件

如果你想让你的友链朋友圈css魔改被此仓库收录，请将你的css放入Theme文件夹中并提交PR（注意是**完整不基于其他css主题的文件**，我们会进行独立验证）

## “乐于分享，让个人博客连成圈

---

目前已有的css主题和相应cdn链接：

### JS无改动

1. [Akilar](https://akilar.top/)提供的  akilar-SAO主题（也是默认主题）: https://cdn.jsdelivr.net/gh/Rock-Candy-Tea/hexo-friendcircle-demo@main/css/akilar-SAO.css
2. [张洪HEO](https://blog.zhheo.com/)提供的  heo主题: https://cdn.jsdelivr.net/gh/Rock-Candy-Tea/hexo-friendcircle-demo@main/css/heo.css

### JS有改动

1. [林木木](https://immmmm.com/)提供的 immmmm主题， CDN引入方案如下：
   ```html
   <!-- 友链朋友圈样式 -->
   <link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/Rock-Candy-Tea/hexo-friendcircle-demo@main/css/fcircle-lmm.css">

   <!-- 全局引入友链朋友圈配置项 -->
   <script type="text/javascript">
   var fdata = {
       apiurl: 'https://friendcircle-api-fx7ykk2ye-lmm214.vercel.app/api',
       initnumber: 20, //【可选】页面初始化展示文章数量
       stepnumber: 10,//【可选】每次加载增加的篇数
       error_img: 'https://sdn.geekzu.org/avatar/57d8260dfb55501c37dde588e7c3852c' //【可选】头像加载失败时默认显示的头像
   }
   </script>

   <!-- 友链朋友圈JS -->
   <script type="text/javascript" src="https://cdn.jsdelivr.net/gh/Rock-Candy-Tea/hexo-friendcircle-demo@main/js/fcircle-lmm.js"></script>

   <!-- 挂载友链朋友圈的容器 -->
   <div id="fcircleContainer">与主机通讯中……</div>
   ```

   注：此版仅有更新时间排序，UI较为简洁
