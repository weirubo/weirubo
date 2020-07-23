<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Title</title>
    <!-- 参考阮一峰里面的百分比布局，要实现和上面一样的效果（一侧固定，一侧随父级进行变化） -->
    <!-- flex: 1 =? 1 1 0%
    flex: auto => 1 1 auto
    flex: none => 0 0 auto;
    flex-basis优先级 自身设定 > 0%(flex:1按字体的高度) > auto(采用height) -->
    <style>
      .wrap {
        margin: 0 auto;
        width: 80%;
 
        display: flex;
      }
      #left {
        flex: 0 0 200px; /* 左侧固定200px */
        height: 500px;
        background: red;
      }
      #right {
        /* 此处解释下
        flex: 1 1 0%
        0%表示此处宽度是按照自身内容宽度来，此处自身内容宽度为0，但是分配剩余的空间，所以可以自适应变化
         */
        flex: 1; /* 随父级变化 */
        height: 500px;
        background: burlywood;
      }
    </style>
 
</head>
<body>
<div class="wrap">
  <aside id="left"></aside>
  <section id="right">5555</section>
</div>
 
</body>
</html>
