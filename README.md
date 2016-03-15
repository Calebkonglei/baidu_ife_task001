# baidu_ife_task001
#百度前端技术学院第一阶段第八个任务响应式网格（栅格化）布局
#页面展示地址：http://dannisi.github.io/baidu_ife_task001/task08/
#该任务总结：
#1.注意清除浮动。每一行使用伪类选择器before和after来清除浮动。
.row:before, 
.row:after {
    content:"";
    display:table;
    clear:both;
}

#2.使用了outline属性添加边框。outline的用法和border一样，但是它不像border
  会影响元素大小


#3.因为为每个框使用了margin-left:20px属性，所以在媒体查询时，就需要对每个
 框的width减去20像素，并使用了calc（）来让浏览器精确的算出相应値，可以参
 考该博客http://www.w3cplus.com/css3/how-to-use-css3-calc-function.html
 示例代码
      .col-md-4{
        width:calc(33.333% - 20px);
      }
