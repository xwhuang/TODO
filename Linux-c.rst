* 宏
1) 字符串创建算符(#)
   宏定义:
   #define doit(name) dothis(#name, name)
   
   调用:
   doit(COLOR_RED);
   
   C预处理器扩展为:
   dothis("COLOR_RED", COLOR_RED)



