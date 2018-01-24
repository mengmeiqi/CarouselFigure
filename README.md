# CarouselFigure
    轮播图
## 知识点
### 定时器
#### setInterval()和setTimeout()
        setInterval() 按照指定的周期（以毫秒计）来调用函数或计算表达式
        setTimeout() 指定的毫秒数后调用函数或计算表达式
        异同：
        (1)二者参数相同(function(){},time)
        (2)setInterval是一直执行，到点就执行，除非把它clear
        (3)setTimeout就执行一次，不再执行
        举例：
        (1) var i=0;
            var time1 = setInterval(function(){
                console.log(i++);
                if(i==5){
                    clearInterval(time1);
                }
            },1000); //结果为 0,1,2,3,4

        (2) var i = 0;
            var time2 = setTimeout(function(){
                console.log(i++);
            },1000); //结果为 0
