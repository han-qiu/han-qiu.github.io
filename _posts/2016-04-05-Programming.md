# C++程序设计

@(仇涵的笔记本)

---

##Week 7
####Lesson 4
#####输入输出
与输入相关的类
+ ios
+ istream
+ ifstream
+ ostream
+ iostream
+ fstream

+ 输入流对象： cin
+ 输出流对象：1. cout 2. cerr 3. clog
cerr 和clog标准错误输出，缺省和cout一样
cin cout 可以被重定向为文件输入输出
例如
>freopen("test.txt","w",stdout);//将标准输出重定向
>freopen("t.txt","r",stdin);//
——————————————————————
+ while(cin>>x){}//判断输入流结束
+ getline(char *buf,int bufSize)
+ bool eof();判断输入刘是否结束
+ if(!cin.getline())
+ peek//读取下一个字符，但不从流去掉
+ putback放回
+ ingore删掉
