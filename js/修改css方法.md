## 实例方法

 1. CSSStyleSheet.insertRule()

    ​		CSSStyleSheet.insertRule方法用于在当前样式表插入一个新的css规则

    ```js
    var sheet = document.querySelector('#styleElement').sheet;
    sheet.insertRule('#block{color:white}',0)
    sheet.insertRule('p{color:red}',1)
    ```

    该方法接受两个参数,第一个参数是表示css规则的字符串,这里只能有一条规则,否则会报错,第二个参数是该规则在样式表的插入位置(从0开始),该参数可选,默认为0(即默认插入在样式表的头部) 如果插入位置大于现有规则数目会报错

​		该方法的返回值是新插入规则的位置序号

​		注意,浏览器对脚本在样式表里面插入规则有很多限制