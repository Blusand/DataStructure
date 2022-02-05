# 王道数据结构
主要是对书上的知识进行精简并加上了一点自己的总结，笔记中的大部分内容来自于书本和咸鱼学长的ppt，笔记里包含了所有书本的代码，方便大家随时查阅和运行，还添加了一些书上没有的代码，给予一些思路,使用语言为C++,与书本的C语言差别不大，不同之处有：
- C语言没有&（引用）符，改为\*即可
- 指针p为空时改为NULL：
```C++
int* p = nullptr;   // C++
int* p = NULL;      // C
```
- 分配空间的代码不同，如下：
```C++
#define MaxSize 50

// 顺序表的动态分配
typedef struct {
  ElemType* data;
  int length;
}SeqList;

SeqList L;
L.data = new ElemType[MaxSize]; // C++的初始动态分配
L.data = (ElenType*)malloc(sizeof(ElemType) * MaxSize); // C的初始动态分配
```
使用时注意即可

---

## B站视频

<p align="center">
    <iframe src="//player.bilibili.com/player.html?aid=92191094&bvid=BV1b7411N798&cid=235888729&page=1" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true" width="100%" height="450" sandbox="allow-top-navigation allow-same-origin allow-forms allow-scripts"> </iframe>
</p>

---