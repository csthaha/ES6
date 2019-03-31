## array-find
- finde 找到第一个,返回满足条件的第一个

-findeIndex 找到值的索引
- filter 找到满足条件的所有值

- every 每一项都必须满足条件
- some 只需有一项满足条件就可以

###数组结构
        const arr = [18, 19, 30];
        // es5
        var a = arr[0] , b = arr[1] , c = arr[2];

        //es6 解构 数组解构 [18,19,30]
        const [d,e,f] = arr;

        const [g,[h],i] = [18,[20],30];

###object
        ```const obj = {
            foo: 'foo val',
            bar: 'bar val',
            baz: 'baz val'
        }```
-  const {baz, foo} = obj; 
   <!-- //不存在顺序 ,如果结构不存在的属性则 undefined -->
   const {baz: str1} = obj; 冒号 定义变量 

   ``` const obj1 ={
            p:['hello',{msg:'world'}]
        }
        const { p: [hello, world] } = obj1;
        ```

### function-expand
```
function Person (name) {
            if (!name){
                name = 'default name'
            }
            this.name = name;
        }
        const p1 = new Person ('cst');
        // {name: 'cst'}

        const p2 = new Person();

        // {name: 'default name'}

```
es5 的时候 赋默认值: 
            if (!name){
                name = 'default name'
             }
es6 :  this.name = name || 'default name';

- Arguments 是一个了数组对象 具有length 属性,我们可以通过 索引( Arguments[0]) 取到它的值
- 类数组没有 map 方法
- Array.from 从一个类数组创建 一个真数组
- ul,li 也是一个 类数组

const obj = {
            0: 1,
            1: 2,
            2: 3,
            3: 4,
            length : 5
        }
        const obj_arr = Array.from(obj);
        第五个 undefined
        //Array.from 跟着我们的 length 变化