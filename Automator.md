##Automator生成后无法打开的解决办法
- 我们经常会使用Automator来生成一些实用的小app或者服务组件，但是我们发现，我们生成的app和组件经常会发生打不开的情况或者没有效果，这里我告诉大家怎么解决这个问题。
 
###解决app
- 我们生成完app后需要到：系统设置>安全&隐私>隐私>Accessibility（忘记中文什么意思了，就是左边第五个有小人图标的那个）,然后我们点击+这个图标，然后我们把我们生成好的app添加进去就行了！

###解决服务组件
- 组件的话，我们需要到：系统设置>键盘>快捷键，然后我们看左边第六个的服务，我们可以在这设置我们组件的快捷键，我们生成好后的组件是在：/Users/<user_name>/Library/Services/这个路径，如果我们有些生成好的组件不能设置或者没什么效果，我们需要把生成好后的service文件放到系统的Services文件夹就ok了。我们用Automator生成的服务组件是在/Users/<user_name>/Library/Services/这个路径（<user_name>这写你电脑的用户名，比如我的用户名是admin，那么我的完整路径就是：/Users/admin/Library/Services/。），系统的路径是：/System/Library/Services。复制进去后，我们需要重新启动下我们的mac，然后我们再回到：系统设置>键盘>快捷键里面的服务那，就能看到我们创建的服务组件了！
- 如果还找不到你生成的服务的话，我会上传一个类似win下快速查找文件路径的软件到github上。

#以上就是解决服务和app无法运行的办法了，还有一种情况就是我们生成的app和服务的快捷键和系统自带的冲突了，这个我们只需要修改下就ok了，如果找不到/Users/<user_name>/Library/Services/这个路径，那么就在finder里面按下:command+shift+.快捷键来显示全部隐藏文件。Ends