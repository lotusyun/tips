# tipshow
vue提示框插件，依赖vue2.0以上版本。 原插件地址：https://github.com/jiqianggirl/tipshow

# 使用tipshow
下载文件放到components里

main.js文件中
```javascript
//需要引入vue，以及vue-tipshow
import Vue from 'vue'
import tipshow from '@/components/tipshow'

//使用tipshow
Vue.use(tipshow)

 export default {
    methods: {
        //函数需要返回一个函数
        tishi(){
               this.$tipshow({
                      'msg': '提示信息',
                      'type': 'warning'
                });
        }
    }
}
```

#options对象

名称|描述|默认值|值类型
---|---|---|---
msg|提示信息||String
type|元素为提示框类型，可设置类型black,warning,success|black|String
duration|提示框延迟多少时间隐藏|1500|Number

