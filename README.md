# 图片翻译

从 https://github.com/biuuu/shiny-image/tree/image 或者群共享下载原图及裁剪过的小图

小图翻译后提交到 [images](https://github.com/ShinyGroup/ShinyImage/tree/master/images) 目录下对应的文件夹里

## 如何获得图片的原始文件名
打开浏览器 DevTools 的 Network 栏可以看到游戏的图片名是类似这样的：
`https://shinycolors.enza.fun/assets/a92ac5df733751a266d003b69c239c100f251575765ec1345a3661e0646dc912?v=8`

1. 找到想要添加的图片的文件名，复制其中一小段。比如上面这个的：`a92ac5df733751a266`。

2. 切到浏览器 Console 栏，输入`queryImageName('a92ac5df733751a266')`执行。

3. 确保插件已经开启开发模式，然后刷新浏览器。

4. 游戏里再回到那张图片出现时的页面，就能看到 Console 栏里显示了对应图片的原始文件名。

![image](https://user-images.githubusercontent.com/10892119/122636637-df440b00-d11c-11eb-87ba-aab358f8ef3e.png)

`images/ui/common/parts_skill_list.json_image` 就是图片原始文件名。

到 https://github.com/biuuu/shiny-image 修改 image-list.json 文件，添加刚刚找到的原始文件名，就会自动下载新图片到 image 分支了。
