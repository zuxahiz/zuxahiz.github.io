zsxq是一个很好的知识分享平台，对于一些付费内容有复制限制无法直接复制导出以做交流学习之用，对于程序员来说这个是不可接受的。所以我决定找到相应的方法去绕开限制，更加畅快地去学习。

#### 声明：本方法只做交流学习之用，只为便利程序员自己保存资料，知识版权必须得到足够的尊重和保护。

Note:本方法只适用于chrome浏览器

### 在地址栏里输入命令使得页面可直接编辑
首先我们可以打开相应的付费文章阅读页面，在地址栏里输入： javascript:document.body.contentEditable='true'; document.designMode='on'; void 0
之后页面就编程可以直接编辑的状态了，可以被全部选中了。
注意前边的javascript: 可能得手动输入，chrome可能会自动把这些给滤掉。

### 保存当前网页
保存当前网页方便后边修改对应的脚本

### 修改脚本
通过F12查看源代码我们可以发现content-protection.js 的脚本比较可疑，打开它看看内容寻找进一步的线索。
setDisableCopy();
删除这句，刷新保存的网页，发现可以复制了，搞定。


## 20210228 更新
貌似zsxq把代码给改了，可以F12直接选中整段文字复制。。。
