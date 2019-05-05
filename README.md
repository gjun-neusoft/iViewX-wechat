![](https://repository-images.githubusercontent.com/183588214/f7bd8100-6843-11e9-9060-3ff216a4bcfa)

## iView-wechatX

一个基于iView-wechat端的UI扩展框架

作者(g.jun)完善并修改了iView-weapp官方组件中的一些bug和问题，

使iViewWeapp用起来更加舒适，附合实际项目需求

#### cell

修改i-cell组件，添加title、label的size大小 

```javascript
properties:{
    titleSize: {
        type: Number,
        value: 18
    },
    labelSize: {
        type: Number,
       	value: 14
    }
}

```

```html
<i-cell titleSize="18" labelSize="14"></i-cell>
```



#### input

添加 titleRight 属性，设置title文本布局，name属性

添加name属性

```javascript
properties:{
    titleRight: {
        type: Boolean,
        value: false
    },
    labelSize: {
        type: Number,
       	value: 14
    },
    name: {
        type: String,
        value: ''
    }
}

```

```html
<i-input titleRight="{{true}}" labelSize="10" name="name"></i-input>
```



#### button



添加hidden属性，控制按钮显示隐藏

添加formType : submit支持表单提交

```
properties:{
    hidden: {
        type: Boolean,
        value: false
    }
}

```

```html
<i-button hidden="{{true}}"></i-button>
```



#### checkbox

添加name、value、title属性，针对官方checkbox组件无name与title的bug做补充

```
properties:{
    name: {
        type: Striing,
        value: ''
    },
   title: {
       type: String,
       value: ''
   }
}

```

```html
<i-checkbox name="name" title="title"></i-checkbox>
```



#### radiobox

添加name、value、title属性，针对官方radiobox组件无name与title的bug做补充

```javascript
properties:{
    name: {
        type: Striing,
        value: ''
    },
   title: {
       type: String,
       value: ''
   }
}

```

```html
<i-radio name="name" title="title"></i-radio>
```

