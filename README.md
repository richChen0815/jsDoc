# 题外话
初衷:在学习jsDoc 之前先来说一下github的README.md文件写法，毕竟这是个门面，知道一些常规写法不为过。

# 1.标题
```
  # 一级标题
  ## 二级标题
  ### 三级标题
```
 tips: #和文字之间需要有一个空格
 
# 2.字体样式 -- 粗体斜体
```
  *斜体*
  **粗体**
  ***粗体斜体***
```
 tips:一对*代表斜体，2对*代表粗体，3对*代表粗体加斜体
 
 
 # 3.代码块写法
  ```
   (async(ctx,next)=>{
    awiat xxxx;
   })();
  ```
  
  
 # 4.插入链接
 ```
  [this is url link](http://baidu.com)
 ```
 [this is url link](http://baidu.com)
 
 # 5.插入图片
   一般不要直接复制到README.md文件中，建议把README.md需要应用的图片文件放到仓库中,在引用仓库地址。
   加载图片的写法</br>
   
  ```
   ![提示](图片地址)
 ```
 
  
   **![图片加载错误的时候提示](https://github.com/richChen0815/jsDoc/blob/master/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20190621172243.jpg)**
    
    
 地址链接和图片链接相近 都是中括号加一对括弧，前者没有感叹号，后者加感叹号。



**题外话讲的有点多了，下面来总结jsDoc写法**

# jsDoc 注释
 必须要 /** 开头，否则不能被jsDoc解析器解析。根据js注释，生成类似于接口的阅读文档。
 
# jsDoc 注释标签  
 一般采取@符号开头
 
# jsDoc 运行
 ```
 1. npm install jsdoc --save-dev | -g  
 2. jsdoc xx.js

```
# demo
```
 /**
 * 这是一个student 类
 * @constructor
 * @param {string} name - 学生姓名
 * @param {string} sex  - 学生性别
 */
  class Student{
    constructor(name,sex){
      this.name = name;
      this.sex = sex;
    }
    
    /**
    * 获取学生姓名
    * @returns {string|*}
    */
    
    getUserName(){
      return this.name
    }
    
    /**
    * 设置学生性别
    *  @param sex {string}
    */
    
    setUserSex(sex){
     this.sex = sex;
    }
  }
```






 

