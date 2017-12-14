# jquery.number-run.js

> jquery.number-run.js 数字滚动插件

## 在线演示：

[https://postbird.gitee.io/jquery.number-run.js/](https://postbird.gitee.io/jquery.number-run.js/)


## 使用方式：

### 示例一：
```html
<span id="number-example-1" class="text-number" number="3276.32" speed="20">3276.32</span>
```
```javascript
$("#number-example-1").numberRun({
    attr: true
});
```
### 示例二：
```html
<span id="number-example-2" class="text-number" number="3276" speed="30">3276</span>

```
```javascript
$("#number-example-2").numberRun({
    attr: true
});
```

### 示例三：
```html
<span id="number-example-3" class="text-number">3276</span>
```
```javascript
$("#number-example-3").numberRun({
    number:3276,
    speed:40
});
```

### 示例四：
```html
<span id="number-example-4" class="text-number">3276</span>
```
```javascript
$("#number-example-4").numberRun({
    number: 3276,
    speed: 60,
    callback:function(){
        alert("滚动完成，number = 3276，speed = 20");
    }
});
```

## 参数说明：

<table class="table table-hover table-striped">
                    <thead>
                        <tr>
                            <th>参数名</th>
                            <th>参数说明</th>
                        </tr>
                    </thead>
                    <tbody>
                        <tr>
                            <td>attr</td>
                            <td>是否从 html 的 attr 中获取参数，如果选择是，则 html 中必须有
                                <code>number</code> 和
                                <code>speed</code> 两个 attr
                            </td>
                        </tr>
                        <tr>
                            <td>number</td>
                            <td>
                                最终需要滚动的数字 可以从 html中获取，也可以配置，支持小数
                            </td>
                        </tr>
                        <tr>
                            <td>speed</td>
                            <td>滚动的速度，speed，滚动速度越慢</td>
                        </tr>
                        <tr>
                            <td>callback</td>
                            <td>回调函数，滚动完成后出发该方法</td>
                        </tr>
                    </tbody>
                </table>

## License：

MIT
