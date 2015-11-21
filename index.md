<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**Table of Contents**  *generated with [DocToc](https://github.com/thlorenz/doctoc)*

- [问题记录 && 解决方案](#%E9%97%AE%E9%A2%98%E8%AE%B0%E5%BD%95-&&-%E8%A7%A3%E5%86%B3%E6%96%B9%E6%A1%88)
  - [json 解析错误](#json-%E8%A7%A3%E6%9E%90%E9%94%99%E8%AF%AF)
  - [invalid date 错误](#invalid-date-%E9%94%99%E8%AF%AF)
- [js 深入理解](#js-%E6%B7%B1%E5%85%A5%E7%90%86%E8%A7%A3)
  - [闭包的理解](#%E9%97%AD%E5%8C%85%E7%9A%84%E7%90%86%E8%A7%A3)
  - [setTimeout](#settimeout)
  - [for && while 使用区分 (刺猬书说的)](#for-&&-while-%E4%BD%BF%E7%94%A8%E5%8C%BA%E5%88%86-%E5%88%BA%E7%8C%AC%E4%B9%A6%E8%AF%B4%E7%9A%84)
  - [js 原型理解](#js-%E5%8E%9F%E5%9E%8B%E7%90%86%E8%A7%A3)
  - [如何真正分辨一个类型](#%E5%A6%82%E4%BD%95%E7%9C%9F%E6%AD%A3%E5%88%86%E8%BE%A8%E4%B8%80%E4%B8%AA%E7%B1%BB%E5%9E%8B)
  - [函数的2种调用方法](#%E5%87%BD%E6%95%B0%E7%9A%842%E7%A7%8D%E8%B0%83%E7%94%A8%E6%96%B9%E6%B3%95)
  - [e.target vs e.currentTarget](#etarget-vs-ecurrenttarget)
  - [js notes](#js-notes)
    - [hashchange demo](#hashchange-demo)
    - [cross-domain 问题 跨域](#cross-domain-%E9%97%AE%E9%A2%98-%E8%B7%A8%E5%9F%9F)
    - [jsonp](#jsonp)
    - [复制input[file]内容，怎么处理？](#%E5%A4%8D%E5%88%B6inputfile%E5%86%85%E5%AE%B9%EF%BC%8C%E6%80%8E%E4%B9%88%E5%A4%84%E7%90%86%EF%BC%9F)
    - [uglify js uglifyjs](#uglify-js-uglifyjs)
    - [.a ~ .b](#a--b)
    - [保留小数点 decimal places 2](#%E4%BF%9D%E7%95%99%E5%B0%8F%E6%95%B0%E7%82%B9-decimal-places-2)
    - [callback 中，将this传进去](#callback-%E4%B8%AD%EF%BC%8C%E5%B0%86this%E4%BC%A0%E8%BF%9B%E5%8E%BB)
    - [js format date](#js-format-date)
    - [js](#js)
    - [checkbox 终极算法](#checkbox-%E7%BB%88%E6%9E%81%E7%AE%97%E6%B3%95)
    - [array 去重](#array-%E5%8E%BB%E9%87%8D)
    - [css turn to inline style](#css-turn-to-inline-style)
    - [专题页切图流程](#%E4%B8%93%E9%A2%98%E9%A1%B5%E5%88%87%E5%9B%BE%E6%B5%81%E7%A8%8B)
    - [unique arr](#unique-arr)
    - [placeholder: jquery.html5-placeholder-shim.js](#placeholder-jqueryhtml5-placeholder-shimjs)
    - [remove select option 重新 触发 select change事件](#remove-select-option-%E9%87%8D%E6%96%B0-%E8%A7%A6%E5%8F%91-select-change%E4%BA%8B%E4%BB%B6)
    - [array indexof](#array-indexof)
    - [jquery \$(function(){}); \$(document).load(); window.onload = function(){};](#jquery-%5Cfunction-%5Cdocumentload-windowonload--function)
    - [js Date()](#js-date)
    - [继承 inherit](#%E7%BB%A7%E6%89%BF-inherit)
    - [promise 学习笔记](#promise-%E5%AD%A6%E4%B9%A0%E7%AC%94%E8%AE%B0)
    - [动画模板](#%E5%8A%A8%E7%94%BB%E6%A8%A1%E6%9D%BF)
    - [防止重复提交相同 ajax 请求 request](#%E9%98%B2%E6%AD%A2%E9%87%8D%E5%A4%8D%E6%8F%90%E4%BA%A4%E7%9B%B8%E5%90%8C-ajax-%E8%AF%B7%E6%B1%82-request)
- [escape encodeURI  encodeURIcomponent不同](#escape-encodeuri--encodeuricomponent%E4%B8%8D%E5%90%8C)
- [checkbox 全选](#checkbox-%E5%85%A8%E9%80%89)
    - [移动端 自适应字体](#%E7%A7%BB%E5%8A%A8%E7%AB%AF-%E8%87%AA%E9%80%82%E5%BA%94%E5%AD%97%E4%BD%93)
    - [js false 类型](#js-false-%E7%B1%BB%E5%9E%8B)
    - [js url params to object](#js-url-params-to-object)
    - [flash check](#flash-check)
  - [ie 版本测试](#ie-%E7%89%88%E6%9C%AC%E6%B5%8B%E8%AF%95)
  - [google MAP 使用笔记](#google-map-%E4%BD%BF%E7%94%A8%E7%AC%94%E8%AE%B0)
  - [简单的js 模板](#%E7%AE%80%E5%8D%95%E7%9A%84js-%E6%A8%A1%E6%9D%BF)
  - [js 完美的触发重绘方法 repaint](#js-%E5%AE%8C%E7%BE%8E%E7%9A%84%E8%A7%A6%E5%8F%91%E9%87%8D%E7%BB%98%E6%96%B9%E6%B3%95-repaint)
- [js 原生](#js-%E5%8E%9F%E7%94%9F)
  - [原生操作](#%E5%8E%9F%E7%94%9F%E6%93%8D%E4%BD%9C)
  - [array indexof](#array-indexof-1)
  - [http](#http)
    - [post get](#post-get)
    - [get max length](#get-max-length)
    - [post size limit](#post-size-limit)
- [业务开发技巧](#%E4%B8%9A%E5%8A%A1%E5%BC%80%E5%8F%91%E6%8A%80%E5%B7%A7)
  - [移动端search 开发思路](#%E7%A7%BB%E5%8A%A8%E7%AB%AFsearch-%E5%BC%80%E5%8F%91%E6%80%9D%E8%B7%AF)
  - [表单重复提交问题](#%E8%A1%A8%E5%8D%95%E9%87%8D%E5%A4%8D%E6%8F%90%E4%BA%A4%E9%97%AE%E9%A2%98)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

## 问题记录 && 解决方案

### json 解析错误

json中不能包含 \-这种 单个的反斜杠

```javascript
{    "test": "\-"}
Expecting 'STRING', 'NUMBER', 'NULL', 'TRUE', 'FALSE', '{', '['

http://stackoverflow.com/questions/7717549/what-is-causing-this-syntax-error-while-parsing-json
```

### invalid date 错误

new Date( ‘222-333-00 00:00:00’) 会报错

解决方案：s.replace(/-/g, ‘/‘);


## js 深入理解
### 闭包的理解

2.6.3 single page 的那本书上写的

闭包是阻止垃圾回收器将变量从内存中移除的方法，使得在创建变量的执行环境的外部能够访问到该变量

```
var prison = (function(){
    var p = 'p not recycled';

    return {
        prisoner: function () {
            return p;
        }
    };
})();

console.log(prison.prisoner()); // 'p not recycled'

```

这里的 p，私有变量没有被回收

### setTimeout

http://ejohn.org/blog/how-javascript-timers-work/

timer delay is not guaranteed:
> all JavaScript in a browser executes on a single thread asynchronous events

### for && while 使用区分 (刺猬书说的)

while希望条件为真时使用
for希望执行固定次数时使用
  
### js 原型理解

winter 很牛的文章：
http://www.cnblogs.com/winter-cn/archive/2009/05/16/1458390.html

问答题的回答：
http://www.zhihu.com/question/28055523

* 实现了内部的[[call]]的方法就被认为是function对象
* 只要实现了 [[construct]]方法的就可以被new调用，function实现了[[construct]]，new的时候会调用[[construct]]
* [[construct]]: 创建一个新的对象，将它的[[prototype]]设为函数对象的共有属性prototype，以新对象做为this指针的值，执行函数对象
* new Class = new Class()
* 一条圆形链的属性可以相互赋值调用，前提是这个function必须赋值了prototype
* 当前function的__proto__属性，指向他上一级原形链的prototype
* Object.create(proto) 传入和返回的都是prototype，所以可以这样 var xx = Object.create(parent.prototype) xx.__proto__ === parent.prototype //true
* Class.__proto__ === Function.prototype , Class.prototype.__proto__ === Object.prototype

new的解释

new语法解开语法糖的话可以用下述代码模拟：
var obj = new Foo()
等于
var tmp = Object.create(Foo.prototype, {}) // 创建一个新的空对象，并指定新对象的[[Prototype]]指向constructor的prototype属性所指对象
Foo.call(tmp) // 调用constructor，传入新创建的对象作为this
var obj = tmp // 得到新创建的对象的引用

* function 是一种特殊的 Object

### 如何真正分辨一个类型

Object.prototype.toString.call()
### 函数的2种调用方法

function A() {return 0;}
```
var a = A(); // 0
var b = new A(); //object
```

### e.target vs e.currentTarget
http://stackoverflow.com/questions/5921413/difference-between-e-target-and-e-currenttarget

e.target is what triggers the event dispatcher to trigger and e.currentTarget is what you assigned your listener to.

```javascript
<p>ppp<a href="javascript:;">aaaa</a></p>

//第一种情况：
$('p').on('click', 'a',function (e) {
        console.log('e.target:',e.target);
        console.log('e.currentTarget:',e.currentTarget);
          console.log('e.delegateTarget', e.delegateTarget);

    });
e.target: <a href=​"javascript:​;​">​aaaa​</a>​
e.currentTarget: <a href=​"javascript:​;​">​aaaa​</a>​
e.delegateTarget #document

//第二种
$(document).on('click', 'p',function (e) {
    console.log('e.target:',e.target);
    console.log('e.currentTarget:',e.currentTarget);

});

e.target: <a href=​"javascript:​;​">​aaaa​</a>​
e.currentTarget: <p>​…​</p>​
```

### js notes

* Math.max.apply(null,[1,3,2]) 数组中最大的。 $(‘selector’).map( function(){ return $(this).height(); }); 返回一个数组...
* 没必要， try catch要少用， 会延长作用域链， 尽量少
就是方法在执行的时候， 会产生一个活动的作用域对象， 这个活动的作用域对象跟它的父级作用域，以及最外层的window对象组成一个作用域链。 方法在查找变量的时候会沿着这条作用域链一层一层往外找
当使用try catch 或者with时， 会额外的产生一个作用域对象放到作用域链中，就这样就会延长作用域链， 导致变量查找变慢
查找的是a , 但是a会在 这个方法的作用域对象（这个份对象包含X）和 exception对象查找， exception就是使用try catch额外产生的那个对象

####hashchange demo
```
$(window).on('hashchange', function(){

//用hashchange 的方式记录状态
var url = 'modules/' + window.location.hash.slice(1) + '.html';

$.ajax({
url: url,
dataType: 'html',
success: function (data) {
successHandler(data);
},
error: function(XMLHttpRequest, errorMsg){
console.error(errorMsg);
}
});
});

$(window).trigger('hashchange');
```

####cross-domain 问题 跨域

No 'Access-Control-Allow-Origin' header is present on the requested resource. Origin

* 前端正常post数据，ajaxSubmit form
* 后台加上`response.setHeader("Access-Control-Allow-Origin", "*");`
* nodejs: response.setHeader('Access-Control-Allow-Origin', '*');

####jsonp

jsonp不支持post方法

```
$.ajax({
url: ‘data.jsonp?callback=?',
type: 'get',
dataType: 'jsonp',
jsonpCallback: 'jsonCallback',

success: function(data) {
self.algorithm = data;
},

error: function(a, b, c) {
console.error('error', a, b, c);
}
});

```
data.jsonp中的内容：

```
jsonCallback({
name: 123,
type: 'lala',
fun: function(){}
});
```

####复制input[file]内容，怎么处理？

You can't move the value of one file input to another, it is a security risk. Instead, clone the input, place the clone where the original is, and move the original into the hidden form.

$(".inputfield1").change(function(){
var $this = $(this), $clone = $this.clone();
$this.after($clone).appendTo(hiddenform);
});

####uglify js uglifyjs

https://github.com/mishoo/UglifyJS2

uglifyjs frontend.js -o frontend.min.js -c -m

-c: compress
-m: mangle
-b: beaty [opposite of mangle]

####.a ~ .b
```
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Document</title>
<style>
.a ~ .b {
color: red;
}
</style>
</head>
<body>
<div>
<span class="b">1st</span>
<span class="a">2nd</span>
<span>3rd</span>
<span class="b">4th</span>
<span class="b">5th</span>
</div>
</body>
</html>
```

####保留小数点 decimal places 2

parseFloat(Math.round(number * 100) / 100).toFixed(2);

####callback 中，将this传进去
var _this = this;

_this.$waterfallContainer.waterfall({
maxCol: 4,
maxPage: _this.MAX_PAGE

callbacks: {
renderData: _this._renderWaterfallData.bind(_this)
}
});

#### js format date

```
_generateActivityName: function () {
var now = new Date(), year = now.getFullYear(), month = now.getMonth() + 1, day = now.getDate(), hour = now.getHours(), minute = now.getMinutes(), second = now.getSeconds(), result, fill = function(val) {
return (val < 10 ? "0" : "") + val;
};
month = fill(month);
day = fill(day);
hour = fill(hour);
minute = fill(minute);
second = fill(second);

return year + month + day + '-' + hour;
}
```

#### js
href = 'javascript:;' 如果a标签的javs...拼写错误的话，会取消cancelled掉链接；

####checkbox 终极算法

```
$('.poster-category').on('change', 'input[type=checkbox]', function() {
var $this = $(this),
isChecked = $this.is(':checked');

//如果去选中， 那么选中所有子checkbox
if (isChecked) {

//选中所有子checkbox
$this.parent().siblings('ul').find('input[type=checkbox]').prop('checked', true);

//如果兄弟们都选中了，那么就选中父项， 必须也是递归的
$this.parents('li').each(function(i, obj){
if( !$(obj).siblings('li').find('input:not(:checked)').length) {
$(obj).parent().siblings('label').children().prop('checked', true);
}
});

//如果去掉
} else {

//去掉所有父项选中
$this.parents('ul').siblings('label').find('input[type=checkbox]').prop('checked', false);

//去掉所有子项
$this.parent().siblings('ul').find('input[type=checkbox]').prop('checked', false);
}
});
```

html:
```
<div class="poster-category">
<label class="J_category checkbox-pretty inline-block mr_15 unchecked enabled" data-toggle="checkbox">
<input type="checkbox" name="choise-all-chk"><span>出售中</span>
</label>
<ul>
<li><b class="line-bottom"></b><b class="line-left"></b>
<label class="checkbox-pretty inline-block mr_15" data-toggle="checkbox">
<input type="checkbox" name="item-chkbox" data-id="1016992699"><span>连衣裙</span>
</label>
<ul class="clearfix"></ul>
</li>
<li><b class="line-bottom"></b><b class="line-left"></b>
<label class="checkbox-pretty inline-block mr_15" data-toggle="checkbox">
<input type="checkbox" name="item-chkbox" data-id="1016992700"><span>蕾丝衫/雪纺衫</span>
</label>
<ul class="clearfix"></ul>
</li>
<li><b class="line-bottom"></b><b class="line-left"></b>
<label class="checkbox-pretty inline-block mr_15" data-toggle="checkbox">
<input type="checkbox" name="item-chkbox" data-id="1033229040"><span>寻双贵</span>
</label>
<ul class="clearfix">
<li>
<label class="checkbox-pretty inline-block mr_15" data-toggle="checkbox">
<input type="checkbox" name="item-chkbox" data-id="1033229041"><span>hebad1</span>
</label>
</li>
<li>
<label class="checkbox-pretty inline-block mr_15" data-toggle="checkbox">
<input type="checkbox" name="item-chkbox" data-id="1033229042"><span>hebad2</span>
</label>
</li>
<li>
<label class="checkbox-pretty inline-block mr_15" data-toggle="checkbox">
<input type="checkbox" name="item-chkbox" data-id="1033229043"><span>hebad3</span>
</label>
</li>
</ul>
</li>
</ul>
</div>
```

####array 去重
```
Array.prototype.getUnique = function(){
var u = {}, a = [];
for(var i = 0, l = this.length; i < l; ++i){
if(u.hasOwnProperty(this[i])) {
continue;
}
a.push(this[i]);
u[this[i]] = 1;
}
return a;
};
```

####css turn to inline style
```
(function($) {
var rules = document.styleSheets[document.styleSheets.length - 1].cssRules;
for (var idx = 0, len = rules.length; idx < len; idx++) {
$(rules[idx].selectorText).each(function(i, elem) {
elem.style.cssText += rules[idx].style.cssText;
});
}
$('style').remove();
$('script').remove();
})(jQuery);

```

####专题页切图流程

1. 选出990区域
2. 顶部1920背景的区域

####unique arr
```
var getUnique = function(arr){
var u = {}, a = [];
for(var i = 0, l = arr.length; i < l; ++i){
if(u.hasOwnProperty(arr[i])) {
continue;
}
a.push(arr[i]);
u[arr[i]] = 1;
}
return a;
};

```

####placeholder: jquery.html5-placeholder-shim.js

####remove select option 重新 触发 select change事件

$tplTypeSelect[0].selectedIndex = -1;

####array indexof

```
if (!Array.prototype.indexOf) {
Array.prototype.indexOf = function(searchElement, fromIndex) {

var k;

// 1. Let O be the result of calling ToObject passing
// the this value as the argument.
if (this == null) {
throw new TypeError('"this" is null or not defined');
}

var O = Object(this);

// 2. Let lenValue be the result of calling the Get
// internal method of O with the argument "length".
// 3. Let len be ToUint32(lenValue).
var len = O.length >>> 0;

// 4. If len is 0, return -1.
if (len === 0) {
return -1;
}

// 5. If argument fromIndex was passed let n be
// ToInteger(fromIndex); else let n be 0.
var n = +fromIndex || 0;

if (Math.abs(n) === Infinity) {
n = 0;
}

// 6. If n >= len, return -1.
if (n >= len) {
return -1;
}

// 7. If n >= 0, then Let k be n.
// 8. Else, n<0, Let k be len - abs(n).
// If k is less than 0, then let k be 0.
k = Math.max(n >= 0 ? n : len - Math.abs(n), 0);

// 9. Repeat, while k < len
while (k < len) {
// a. Let Pk be ToString(k).
// This is implicit for LHS operands of the in operator
// b. Let kPresent be the result of calling the
// HasProperty internal method of O with argument Pk.
// This step can be combined with c
// c. If kPresent is true, then
// i. Let elementK be the result of calling the Get
// internal method of O with the argument ToString(k).
// ii. Let same be the result of applying the
// Strict Equality Comparison Algorithm to
// searchElement and elementK.
// iii. If same is true, return k.
if (k in O && O[k] === searchElement) {
return k;
}
k++;
}
return -1;
};
}
```

####jquery \$(function(){}); \$(document).load(); window.onload = function(){};

\$(function(){}); = jQuery.fn.init() = \$(document).ready();

http://stackoverflow.com/questions/4584373/difference-between-window-loadfunction-and-document-readyfunction

* `document.ready` is a jQuery event, it runs when the DOM is ready, e.g. all elements are there to be found/used, but not necessarily all content.
* `window.onload` fires later (or at the same time in the worst/failing cases) when images and such are loaded, so if you're using image dimensions for example, you often want to use this instead.

所以`$(window).load()`中，如果有任何js没有加载到，就会无法执行，`$(document).ready()`则不会

####js Date()

```
_generateActivityName: function() {
var now = new Date(),
year = now.getFullYear(),
month = now.getMonth() + 1,
day = now.getDate(),
hour = now.getHours(),
minute = now.getMinutes(),
second = now.getSeconds(),
result, fill = function(val) {
return (val < 10 ? "0" : "") + val;
};
month = fill(month);
day = fill(day);
hour = fill(hour);
minute = fill(minute);
second = fill(second);

return year + month + day + '-' + hour + minute + second;
},

```

####继承 inherit

http://stackoverflow.com/questions/2107556/how-to-inherit-from-a-class-in-javascript
http://stackoverflow.com/questions/7486825/javascript-inheritance

```
function inherit(subClass, superClass) {
// body...
}

function Animal(name, age) {
this.name = name;
this.age = age;
}
Animal.prototype.doSomething = function() {
console.log('name:', this.name, 'age:', this.age);
};

function Dog() {
Animal.apply(this, arguments);
}

function createObject(proto) {
function F() {}
F.prototype = proto;
return new F();
}

Dog.prototype = createObject(Animal.prototype);
Dog.prototype.constructor = Dog;

// inherit(dog, Animal);

var xx = new Dog('a1', 20);
xx.doSomething();

```

#### promise 学习笔记

https://github.com/barretlee/myPromise
http://www.ruanyifeng.com/blog/2011/08/a_detailed_explanation_of_jquery_deferred_object.html
http://fex.baidu.com/blog/2015/07/we-have-a-problem-with-promises/?url_type=39&object_type=webpage&pos=1

我的自定义函数模板：ajax本身就会返回deferred对象了

```
function myFunc() {
var dtd = $.Deferred();

function wait() {
alert('finished');
dtd.resolve('xxx');
}

setTimeout(wait, 2000);

return dtd.promise();
}

var xx = myFunc();

$.when(xx).done(function(r) {
alert(r);
});

```

推荐链接：

http://www.html5rocks.com/zh/tutorials/es6/promises/

####动画模板

整体思路就是，往queue传一个数组，然后每次调用dequque输出一个~就行了

```
var q = [function() {
$(this).animate({
"width": "200px",
"height": "200px"
}, next)
}, function() {
$(this).animate({
"width": "400px",
"height": "400px"
}, next);
}];

function next() {
$('#test').dequeue('myQueue');
}
$('#test').queue('myQueue', q);
next();
$('#test').queue('myQueue', function() {
$(this).slideUp().dequeue('myQueue');
});

```

####防止重复提交相同 ajax 请求 request
```
currentRequest = jQuery.ajax({
type: 'POST',
data: 'search_text=' + text,
url: 'AJAX_URL',
beforeSend: function() {
if (currentRequest != null) {
currentRequest.abort();
}
},
success: function(data) {
jQuery('#data').html(data).show();
}
});
```e's

##escape encodeURI  encodeURIcomponent不同

http://stackoverflow.com/questions/75980/best-practice-escape-or-encodeuri-encodeuricomponent

 escape 已经被抛弃

如果编码url 用encodeURL（不会破坏url）

encodeURIComponent会编译所有内容 可以传urlParam 的时候使用

## checkbox 全选
$(".checkALL").click(function(){
          if($(this).prop("checked") == true){
               $(".checkALL").prop("checked","true");
               $(".pro-list input[type=checkbox]").prop("checked","true");
          }else{
               $(".checkALL").removeAttr("checked");
               $(".pro-list input[type=checkbox]").removeAttr("checked");
          }
     });

####移动端 自适应字体
//自适应body字体大小 20/320的比例
    function setBodyFontSize() {
        var width = $(window).width(),
            SCALE = 20 / 320,
            targetFontsize;

        targetFontsize = width * SCALE;

        $('body').css('font-size', targetFontsize + 'px');
    }

    $(window).on('resize, load', function() {
        setBodyFontSize();
    });

####js false 类型
null false 0 ‘’ undefined NaN

####js url params to object

https://gist.githubusercontent.com/ryoppy/5780748/raw/267c9d244c767dc43ce4a936c214dc565f5c7320/getQueryParams.js

####flash check

```
checkFlash: function() {
    var hasFlash = false, //是否安装了flash
        flashVersion = 0, //flash版本
        swf;

    try {
        //document.all可用来判断是否是IE浏览器,TRUE即是IE浏览器
        if (document.all) {
            swf = new ActiveXObject('ShockwaveFlash.ShockwaveFlash');
            if (swf) {
                hasFlash = true;
                var VSwf = swf.GetVariable("$version");
                flashVersion = parseInt(VSwf.split(" ")[1].split(",")[0]);
            }
        } else {
            if (navigator.plugins && navigator.plugins.length > 0) {
                swf = navigator.plugins["Shockwave Flash"];
                if (swf) {
                    hasFlash = true;
                    var words = swf.description.split(" ");
                    for (var i = 0; i < words.length; ++i) {
                        if (isNaN(parseInt(words[i]))) {
                            continue;
                        }
                        flashVersion = parseInt(words[i]);
                    }
                }
            }
        }

    } catch (e) {
        return false;
    }

    if (!hasFlash || flashVersion < 11) {
        return false;
    }

    return true;
}
```

```

            Object.defineProperty(this, 'end', {

                //最后设置end的时候，把字符串返回。
                set: function() {
                    return this.toString();
                }
            });
```
### ie 版本测试

```
var v = 'Unknown version : (contact me, I am interested by your config ... ;-)'; var ok = 1; if (document.documentMode == 10) v = 'IE 10'; else if (document.documentMode == 9) v = 'IE 9'; else if (window.postMessage) v = 'IE 8'; else if (window.XMLHttpRequest) v = 'IE 7'; else if (document.compatMode) v = 'IE 6'; else if (window.createPopup) v = 'IE 5.5'; else if (window.attachEvent) v = 'IE 5'; else if (document.all) { document.write('IE 4'); ok = 0; } if (ok == 1) document.getElementById('ieversion').innerHTML = v;
```

### google MAP 使用笔记

嵌入式的方式：
1.直接ditu.google.com，里面编辑，然后点击分享链接，以iframe的形式放到自己的网页中；
2.API的使用：

googleMap的使用方法：
综合使用：front-end/demos/googlemap.html
官方参考实例：https://developers.google.com/maps/documentation/javascript/examples/?hl=zh-cn

### 简单的js 模板

https://github.com/fushanlang/js-template

### js 完美的触发重绘方法 repaint

这个要运用到容器上，才能确保发生效果~~~~

```
$con.style.display='table';
setTimeout(function () { $con.style.display = 'block'; }, 0);
```
http://stackoverflow.com/questions/3485365/how-can-i-force-webkit-to-redraw-repaint-to-propagate-style-changes

## js 原生

https://developer.mozilla.org/zh-CN/docs/Web/API/Element/insertAdjacentHTML

### 原生操作

```javascript
var xx = document.getElementsByTagName('body’)[0]
var content = document.createTextNode('xxxxx')
var content = document.createElement('p')
xx.appendChild(content)

var elIndexTab = document.getElementsByClassName('indexTab')[0],
        elContent = document.getElementsByClassName('indexContent')[0],
        elIndexTabLIs = elIndexTab.querySelectorAll('li'),
        elContentDLs = elContent.querySelectorAll('dl');

    var data = [],
        obj,
        i,
        j,
        temp;

    for (i = 0; i < elIndexTabLIs.length; i++) {
        temp = elContentDLs[i];
        obj = {
            title: elIndexTabLIs[i].innerHTML,
            sub: []
        };

        for (j = 0 ; j < temp.childNodes.length; j++) {
            if(temp.childNodes[j].nodeName === 'DD') {
                obj.sub.push({
                    dd: temp.childNodes[j].innerHTML
                });
            }

            if(temp.childNodes[j].nodeName === 'DT') {
                obj.sub.push({
                    dt: temp.childNodes[j].innerHTML
                });
            }
        }
        data.push(obj);
    }
```

### array indexof

```
if (!Array.prototype.indexOf) {
    Array.prototype.indexOf = function(obj, start) {
     for (var i = (start || 0), j = this.length; i < j; i++) {
         if (this[i] === obj) { return i; }
     }
     return -1;
}
}

```

### http 

#### post get
一个幂等操作的特点是其任意多次执行所产生的影响均与一次执行的影响相同
http://stackoverflow.com/questions/3477333/what-is-the-difference-between-post-and-get
http://stackoverflow.com/questions/504947/when-should-i-use-get-or-post-method-whats-the-difference-between-them

It's not a matter of security. The HTTP protocol defines GET-type requests as being idempotent, while POSTs may have side effects. In plain English, that means that GET is used for viewing something, without changing it, while POST is used for changing something. For example, a search page should use GET, while a form that changes your password should use POST.

#### get max length
http://stackoverflow.com/questions/417142/what-is-the-maximum-length-of-a-url-in-different-browsers
大部分浏览器只支持2000 characters，有时候会根据不同客户端，服务端而改变。

#### post size limit
服务器端的设置，默认是2m
http://stackoverflow.com/questions/2364840/what-is-the-size-limit-of-a-post-request

CRUD:
Create -> Post
Read   -> Get
Update -> Put
Delete -> Delete







## 业务开发技巧

### 移动端search 开发思路

* form 绑定 submit 事件，事件里return false; 防止默认提交
* input绑定focus 进入编辑的样式，blur取消掉编辑样式



### 表单重复提交问题

同一链接, 参数相同, 造成历史返回时造成重复提交.

可以加入时间戳来处理