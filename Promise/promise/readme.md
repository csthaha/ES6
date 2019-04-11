```
function callback() {
            console.log("done");
        }

setTimeout(callback,1000)
- setTimeout 里面调用函数 只需写函数名就可以 不需要()
- Promise 里面 then 也是这样
- setTimeout() 用于在指定的 时间后执行该函数（1000毫秒 = 1 秒）
- 如果想要重复执行 使用 setInterval()方法
- 使用clearTimeout() 来阻止函数的执行