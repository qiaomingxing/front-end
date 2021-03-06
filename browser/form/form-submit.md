# 表单的重复提交

## 问题概述

提交表单时可能出现的最大问题，就是重复提交表单。在第一次提交表单后，如果长时间没有反应，用户可能会变得不耐烦，这个时候，他们也许会反复单击提交按钮，结果往往很麻烦（因为服务器要处理重复的请求），或者会造成错误，例如说重复下单。

表单提交最好不好使用get请求，一方面是安全的考虑，直接把数据暴露到url上是一种很安全的行为，一方面是防止刷新浏览器时，重复提交表单。

## 解决

解决这个问题的方法有很多，目前遇到的最好的实现是在第一次提交表单后就禁用提交按钮，并且显示提交中。

```javascript
form.addEventListener("submit", function(){
    btn.disabled = true;
    btn.value = "提交中...";
}, false);
```