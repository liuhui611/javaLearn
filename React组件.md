# 组件笔记

##  类组件和函数组件

### 函数组件

```jsx
function Hello（props）{

return  <div>这是一个Hello组件 -- {props.name}</div>

}
```

在组件里的值是只读的，不能修改

```jsx
const  dog ={
name: '大黄',
age: 3,
gender: '雄'
}

//调用render函数渲染
ReactDOM.render(<div>
123
{/*  直接把组件的名称以标签的形式丢到页面上  */}
<Hello name={dog.name}></Hello>

)
```

```jsx
<Hello {...dog}></Hello>
//这是ES6的语法，展开，直接将三个值传进去
```

