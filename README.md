# 浏览器 import 行为测试







## 嵌套 import

见 /next-import

````shell
 - A
 		- B 
 			 - D
 		- C 
````



<img src="https://typora-1300781048.cos.ap-beijing.myqcloud.com/img/202309081258906.png" alt="image-20230908125823796" style="zoom:25%;" />

<img src="https://typora-1300781048.cos.ap-beijing.myqcloud.com/img/202309081258055.png" alt="image-20230908125810909" style="zoom:25%;" />

最终引入顺序为 A B C D

网络请求顺序是层序遍历的顺序

log 是 D B C A 

但最终执行顺序还是深度递归的执行顺序

？？？这难道是浏览器的什么优化策略吗？
