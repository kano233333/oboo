# oboo
vue components + ui

## 安装

```
npm install oboo --save
```

## 全局使用

```
//main.js
import 'obo.less'
import Oboo from 'oboo'
Oboo(Vue);
```

## 组件

### global-loading

> 页面顶部预加载

```html
<global-loading :imgs=[]></global-loading>
```

## UI

> <span style="color:#337AB7;">primary</span>
>
> <span style="color:#959595;">info</span>
>
> <span style="color:#62ff6f;">success</span>
>
> <span style="color:#ff9953;">warning</span>
>
> <span style="color:#FF6058;">danger</span>
>
> <span style="color:#FFB7C8;">girl</span>
>
> <span style="color:#D087FF;">dream</span>

```
@color_name:primary,info,success,warning,danger,girl,dream;
@color_rgb:#337AB7, #959595, #62ff6f, #ff9953,#FF6058,#FFB7C8,#D087FF;
```

```
#container
.column //列
.row  //行
.col_1 - .col_24 
.bg_@{colorName}  //背景颜色
.lin_side_@{colorName}  //两边渐变
.lin_left_@{colorName}  //to left渐变
.lin_right_@{colorName} //to right渐变
.bq_@{colorName} //引用框左边框
.a_link_@{colorName} //a:hover 下划线
.t_@{colorName}  //字体颜色
//按钮大小
.btn_l .btn_m .btn_ms .btn_s
.circle //50%
```

