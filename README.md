<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Title</title>
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
