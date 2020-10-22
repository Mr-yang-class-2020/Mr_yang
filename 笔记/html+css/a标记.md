# a标记

> < a href='' > 超级连接标签 </a>

a标签在html中用于网页与网页之间的跳转，或者是网页内部的跳转。对于a标签我们的使用有2中方式



### 1. 网页与网页之间的跳转

+ 跳转形式有2种

  + 1.绝对路径 

    + 固定域名的网络地址，都可以称之为绝对路径

    + https://www.baidu.com

    + ```html
      <a href="https://www.baidu.com" title=''>
      	连接到百度页面
      </a>
      ```

    + ![image-20200917155824811](img\image-20200917155824811.png)

  + 2.相对路径

    +  从当前文件的位置，访问指定位置的html文件

    + ./../xxx.html  

    + 在20200917文件夹下，存有2个文件 a.html 和a-1.html

    + <img src="img\image-20200917160344800.png" alt="image-20200917160344800" style="zoom: 80%;" />

    + > a.html
      >
      > ```html
      > <a href='a-1.html'>点击我，可以连接到a-1.html页面</a>
      > ```

    + > a-1.html
      >
      > ```html
      > <a href='./a.html'>点击我，可以连接到a.html页面</a>
      > ```

    + ![image-20200917160648797](D:\web前端\笔记\html\img\image-20200917160648797.png)

    + ![image-20200917160702180](D:\web前端\笔记\html\img\image-20200917160702180.png)

    + 以上两个页面之间就可以相互进行跳转





### 2.a标签的锚标记方法使用

a的锚标记方法是可以用过href属性 定位 其他元素的name属性。通过连接查找name值。进行同页面跳转，

在href属性中。`#`代表查找的意思

通过href查找指定的name名字。实现锚标记跳转效果



+ 1.查找锚标记

  + >  a-2.html
    >
    > ```html
    > <!--注释:在href中通过#查找当前页面中定义的name值。做锚标记跳转-->
    > <a href='#address1'>位置1</a> <br/>
    > <a href='#addr2'>位置2</a> <br/>
    > <a href='#addr3'>位置3</a> <br/>
    > ```

+ 2.定义锚标记点

  + > a-2.html
    >
    > ```html
    > <p>
    > 	<a name='address1'>位置1address1<a>
    > 	Lorem ipsum dolor sit, amet consectetur adipisicing elit. Odio, nulla. Cupiditate, itaque. Provident quos cum culpa corrupti, optio nesciunt fugit tenetur molestiae nulla rerum perferendis, accusamus ullam repellat expedita omnis!
    > </p>
    > <br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/>        
    > <p>
    > 	<a name='addr2'></a>
    > 	位置2,address2,Lorem ipsum, dolor sit amet consectetur adipisicing elit. Distinctio dolores aspernatur accusamus magnam provident, perspiciatis quibusdam numquam accusantium sed quisquam, eos maiores quasi ea nihil nemo possimus commodi sit natus.
    > </p>
    > <br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/>
    > <p>
    > 	<a name='addr3'></a>位置3address3
    >     Lorem ipsum dolor sit amet consectetur adipisicing elit. Cumque consequatur aut amet explicabo pariatur facere earum distinctio exercitationem ea eius placeat autem aperiam optio impedit doloribus, quas illo? Debitis, tempore?
    > </p>
    > <br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/>
    > ```

  + 注意：当前我们p的内容距离小。所以需要在p与p之前用br来撑开距离

  + 通过用a 的name属性来定义锚标记点。在用href属性查找

+ 通过定义和查找。即可实现同页面锚标记跳转

+ 查看效果：取代码。自己去测试











