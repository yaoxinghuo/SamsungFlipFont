# SamsungFlipFont

1. Project点右键，Andriod Tools-Rename Application Package-改成com.monotype.android.font.miao-一路finish和yes
2. 找到assets/fonts 把id为miao的中文字体放进去，删除原来的
3. 找到assets/font-en 把id为miao的英文字体放进去，删除原来的(如果没有英文字体，是不是可以用中文字体替换，这个有待实际检测)
4. 找到assets/miao.xml按F2修改文件名改成相应的id的，然后双击编辑，上面的displayname改成实际的字体名称，
然后把下面的miao.ttf改成实际的id
5. 找到res/string.xml编辑里面的app_name把名称改成实际字体的名字
6. Project点右键Export-Export Android Application-Next-输入两次password-输入这次apk的名字，比如miao.apk-Finish
7. 装到三星机器上验证下便可

后续参考这里
http://bbs.hiapk.com/thread-5336391-1-1.html
大概意思是现在要验证签名或者只有指定几个包名的才让安装字体，所以改成com.monotype.android.font.miao了，然后安装到Internal
