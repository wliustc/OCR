# OCR

主要功能

1、登陆QQ，任意界面按下Ctrl+Alt+F触发截图，无需打开消息框。

2、选取需要的区域，按下“√”，自动保存并上传截图。

3、调用百度AI文字识别、百度翻译，将英文自动翻译为中文。

4、识别、翻译完成后自动打开文档。

5、可重复使用，自动关开文档。


注意事项

1、建议仅在使用时打开此软件，不建议长时间后台运行。

2、使用此软件前，建议将记事本保存，以免被程序强制关闭而导致数据丢失。

3、每天最多可识别500次，请节约使用，使用次数每日更新。

4、英语识别有时不准，结果仅供参考。

5、初版程序比较粗糙，后续将完善，欢迎童鞋们留言建议。

6、原本调用微信的dll实现离线截图，但小编的是64位Python，因此选用了QQ的在线截图。

7、原本使用pyhook监听键盘实现快捷截图，但一直没装成功，因此选用了监听剪切板。


基本原理

程序监听剪切板 ----> Ctrl+Alt+F触发截图 ---->检测到剪切板有输入 ---->如果不是图片，就忽略；否则 ---->图片上传进行文字识别 ---->识别到的文字进行百度翻译 ---->将总的结果写入本地文本 ---->打开文本 ---->结束代码分部详解
