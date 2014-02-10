require('nv:util')
=======

####获取对象方式:
    var util = require('nv:util');

####接口:

#####函数切片
    util.aop(FunctionArray);

返回值: Function 执行这个函数会执行数组中的所有函数.

#####对象扩展
    util.extend(targetObject,object1[,object2,object2,...]);

返回值: Object 扩展后的targetObject.

#####将对象转换为“可观察对象”(若参数为空则创建一个新的) #浏览器支持ES6后可取消
    var obj = util.convert({
        age:0
    }).watch(['a'], function(name,newval,oldval){
        alert(name + ':' + oldval + '==>' + newval);
    });
    obj.age = 10;

返回值: Object 转换后的“可观察对象”.

#####class管理(简版,后面会逐渐扩展替代Zepto)
    util.dom(el).addClass('class1');
    util.dom(el).removeClass('class1');

返回值: Object Dom模型对象