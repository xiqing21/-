# Markdown快速入门



## 1、代码块

```java
//代码语法
``` java
    
public class WebSite {
   
    /**
     * 站点url
     */
    private String url;
       
    /**
     * 需要爬行的url队列
     */
    private UrlQueue<String> urls = new UrlQueue<>();
       
    /**
     * 已爬行过的页面url
     */
    private List<String> exitUrls = Collections.synchronizedList(new ArrayList<>());
       
    private static final int TOTAL_THREADS = 12;  
       
    private final CountDownLatch mStartSignal = new CountDownLatch(1);  
       
    private final CountDownLatch mDoneSignal = new CountDownLatch(TOTAL_THREADS);   
       
    public WebSite(String url){
        this.url = url;
        urls.offer(url);//把网站首页加入需要爬行的队列中
    }
```

### Shell语法

```shell
expr $a + $b
expr $a - $b
expr $a * $b //乘法 \ : 转意符号
expr $a / $b
expr $a % $b //取余数
```



## 2、标题

``` java
# 一级标题
## 二级标题
### 三级标题
#### 四级标题
##### 五级标题
###### 六级标题
```

# 一级标题
## 二级标题
### 三级标题
#### 四级标题
##### 五级标题
###### 六级标题

## 打开结构图

**CTRL+shift+1**

## 3、字体

``` java
// 加粗
**CTRL+shift+1**
// 代码高亮显示
==A梦资源网==
// 删除线
~~被删除的文字~~
// 斜体
*被斜体的内容*
```

// 加粗
**CTRL+shift+1**
// 代码高亮显示
==A梦资源网==

// 删除线
~~被删除的文字~~
// 斜体
*被斜体的内容*

## 4、引用

``` java
//引用语法
>作者：郑鑫鑫
>>作者：郑鑫鑫
>>>作者：郑鑫鑫
```

//引用语法
>作者：郑鑫鑫
>>作者：郑鑫鑫
>>
>>>作者：郑鑫鑫

## 5、分割线

``` java
// 分割线
---
// 分割线2
***
```

---



***

## 6、图片插入



````java
//在线图片 / 本地图片
![我的照片](/image/myPhoto) --图片路径
    ctrl+shift+i
````

![myPhoto](C:\Users\youya\Documents\MarkdownNote\微信图片_20210416172052.gif)

![微信图片_20210416172052](http://i0.hdslb.com/bfs/album/b90abc901ee71e182a574ba3348fc2b884531eda.gif)

## 7、正斜杠和反斜杠

``` java
正斜杠，又称左斜杠，符号是"/"；反斜杠，也称右斜杠，符号是"\"。
在Unix/Linux中，路径的分隔采用正斜杠"/"，比如"/home/hutaow"；而在Windows中，路径分隔采用反斜 杠"\"，比如"C:\Windows\System"。
有时我们会看到这样的路径写法，"C:\\Windows\\System"，也就是用两个反斜杠来分隔路径，这种写法在网络应用或编程中经 常看到，事实上，上面这个路径可以用"C:/Windows/System"来代替，不会出错。但是如果写成了"C:\Windows\System"， 那就可能会出现各种奇怪的错误了。
```

**正斜杠，又称左斜杠，符号是"/"；反斜杠，也称右斜杠，符号是"(\)"。**

## 8、超链接

```java
// 超链接跳转
[你的b站学习页](https://www.bilibili.com/video/BV1hJ411X75X?from=search&seid=17955461182644614592)
```

// 超链接跳转
[你的b站学习页](https://www.bilibili.com/video/BV1hJ411X75X?from=search&seid=17955461182644614592) **按住ctrl＋鼠标左键可以直接跳转**

## 9、列表

```java
//无序列表
- 目录1
- 目录2
- 目录3
// 数字键+.+空格+名称
    1. 我爱你
```

- 目录1
- 目录2
- 目录3

1. 我爱你
2. 罗丽
3. 多久呢
4. 一生一世

## 10、表格

```java
// 表格
ctrl+T
```



| 姓名 | 语文 | 数学 |
| ---- | ---- | ---- |
| 张三 | 78   | 87   |
|      |      |      |
|      |      |      |

## 11、查看语法

``` java
ctrl+/
```



## 12、为什么使用typora

***使用markdown后你会发现笔记比以前工整很多，特别是要将一篇篇笔记往一些博客平台上传的时候，发现都不用排版，就能很好看，节省很多排版布局的时间！第二点就是markdown是存在一些语法规则的，如果您直接使用快捷键，你永远都无法真正理解markdown，学任何一门技术的时候都不应该忽视底层。***

## 13、治疗脱发

1.非那雄胺，每天要定时吃一颗。 在晚上7-9点。一定要定同样的时间点。维持体内药物浓度在最佳状态。坚持吃3-6个月。后面自己慢慢减少用量。我拿三个月的药，吃了快5个月。后面就很少吃了。我现在会隔几天吃一次。京东可以买，比药店便宜了。

----



2.米诺，早晚用一次，每次喷4-6次，不能喷多哦！喷后要按摩头部，促进血液循环，很多人喷上去就不管了。我买了真空梳，喷后，用梳子拍打头部，然后梳头5分钟内，懒惰的我可能就1分钟左右哈哈哈哈。建议剃圆寸，好用药。

