## JS的诞生
### JavaScript诞生背景

  1994年，在互联网刚兴起的时代，网景公司（Netscape）发布了Navigator浏览器0.9版。这是历史上第一个比较成熟的网络浏览器，轰动一时。但是，这个版本的浏览器只能用来浏览，不具备与访问者互动的能力。因此网景公司急需一种**网页脚本语言**，使得浏览器可以与网页互动。

  网页脚本语言到底是什么语言？网景公司当时有两个选择：一个是采用现有的语言，比如Perl、Python、Tcl、Scheme等等，允许它们直接嵌入网页；另一个是发明一种全新的语言。这两个选择各有利弊。第一个选择，有利于充分利用现有代码和程序员资源，推广起来比较容易；第二个选择，有利于开发出完全适用的语言，实现起来比较容易。


![image.png](https://p6-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/93a25fffe8b2491cabf7f93cd990d4e6~tplv-k3u1fbpfcp-watermark.image)

1995年，Sun公司将Oak语言更名为Java并推向市场，并宣称“Write Once, Run Anywhere”。网景公司深受Java的影响，网景公司高层都非常信赖Java，所以网景公司决定要蹭Java的流量，新开发一门语言，用于浏览器的交互。

### JavaScript诞生

  1995年4月，**BrendanEich（布兰登·艾奇）** 加入网景公司。Brenden原本研究方向是函数式编程与Scheme语言。但是1995年5月，网景公司指定Brenden成为了“新语言”的设计师。并且要求这个“新语言”要和Java足够的相似（面向对象思想），但是要比Java能够更加简单地上手。

  Brenden志不在此，而且对Java完全不感兴趣，为了完成任务他花了10天时间便把这门“新语言”的最初版本设计了出来。总的来说他的设计思路是这样的：
> （1）借鉴C语言的基本语法；
> 
> （2）借鉴Java语言的数据类型和内存管理；
> 
> （3）借鉴Scheme语言，将函数提升到"第一等公民"（first class）的地位；
> 
> （4）借鉴Self语言，使用基于原型（prototype）的继承机制。
所以，Javascript语言实际上是两种语言风格的混合产物——（简化的）函数式编程+（简化的）面向对象编程。

#### JavaScript名字的由来

  最初为了紧贴Java（有一种咖啡也叫Java），这门“新语言”被命名为Mocha（有一种咖啡也叫Mocha）。

  但由于商标的问题，以及网景公司很多产品已经使用了“Live”作为产品名前缀，Mocha更名为LiveScript。

  由于网景公司与Sun公司有一些合作（网景公司允许Java程序以applet（小程序）的形式，直接在浏览器中运行；甚至还考虑直接将Java作为脚本语言嵌入网页），Sun把Java这个商标授权给了网景公司，于是LiveScript更名为**JavaScript**。
## 浏览器发展史

### 早期浏览器大战

  由于互联网刚兴起，各种浏览器也层出不穷，而各个商家的浏览器支持的浏览器脚本也不太一样。其中微软在1996年8月发布了自己的浏览器IE3。IE3 并不支持JavaScript，而是支持自家研发的脚本语言JScript。

### 网景提交JS标准

  1996年11月，网景向ECMA提交语言标准，由于版权问题，JS语言标准不叫JavaScript，而是ECMAScript。

  JavaScript与ECMAScript的区别在于，ECMAScript是标准，JavaScript是实现，实现的功能不一定会出现在标准里面。实际上JavaScript是由ECMAScript，DOM和BOM三者组成的

### 网景之死

  为了推广自家浏览器，微软将IE浏览器直接捆绑进了Windows系统中。这一举动，直接让IE浏览器占据了市场绝大部分的份额。1998年，为了抗衡IE浏览器，网景公司直接把自家的浏览器开源（FireFox前身），但是仍然难逃被收购的命运。Brenden之后一直在协助维护这个网景开源的浏览器。
### IE6如日中天

  2001年，IE6和Windows XP系统一起发布。至2004年，IE6已经占据了市场的80%以上。然而这款浏览器却不兼容W3C标准（主要是CSS）。

  看见IE6独霸一方，无人可敌，微软直接把IE6开发团队给解雇了一大部分，导致IE6不断爆出安全漏洞。这种情况下，FireFox重新出山，希望打败IE。

  看到FireFox的东山再起，微软重新组建的团队开发IE7。2005年，IE7发布，但是由于开发团队能力不如IE6的团队，IE7也干不过自家兄弟IE6。

  2006年，主流浏览器除了IE6还有一个FireFox。但由于盗版XP系统在中国横行，直至2010年中国浏览器市场仍然被IE6占据。这也成为了中国前端开发的噩梦（需要不断兼容IE），大大阻碍了中国前端的发展。

### Chrome横空出世

   2004年，**谷歌**雇用了一些FireFox和IE的开发者进行自己浏览器Chrome的开发。

   2008年，Chrome浏览器发布，并迅速拿下1%的市场份额。由于Chrome浏览器非常快，越来越受到市场的欢迎。

   2011年，Chrome浏览器的市场份额超越FireFox。

   2016年，Chrome浏览器的市场份额达到62%。Chrome的腾飞结束了中国前端开发者被IE折磨的日子。2016年，淘宝天猫宣布不再支持IE6、7；同年年底，宣布不再支持IE8。

### 移动市场颠覆格局

  2010年iPhone4发布，宣告智能手机时代来临。但是无论是IOS系统（Safari），还是Android系统（chrome）都不支持IE浏览器。

  微软见此情况和Nokia联合起来，但最终还是Nokia在手机行业宣告失败，手机业务被微软收购。可以认为，手机上基本见不到IE了。

  至此，前端开发者可以不再需要考虑IE用户的需求，摆脱了被IE支配的日子，前端从此极速发展。

## ECMAScript标准

### ECMAScript各个版本

  1997年6月，第一版ECMAScript发布。

  1999年12月，第三版ECMAScript发布，这也是**应用最广泛**的ECMAScript版本。

  第四版流产。

  第三版发布后，经过了10年，20019年12月第五版ECMAScript才发布，这正是因为这段时间IE浏览器正制霸着市场。

  随着Chrome的崛起，这些新的浏览器的JS引擎都根据ECMAScript标准进行实现。所以除了IE，其他浏览器与浏览器之间的兼容性得到大大提高。

  2015年6月，ECMAScript第六版（ES6）发布。并在之后每一年都发布一版。可见JS地位在不断提高。

  JavaScript与ECMAScript的区别在于，ECMAScript是标准，JavaScript是实现（实际上JavaScript是由ECMAScript，DOM和BOM三者组成的），实现的功能不一定会出现在标准里面，不同的浏览器也有自己独特的JS实现。

## JS的发展

### JS的兴起--Gmail的诞生

   2004年愚人节，谷歌发布Gmail。Gmail是谷歌开发的一款具有发送接收邮件功能的在线网页。在Gmail出现以前，所有人都认为浏览器只能用于浏览阅读。但是Gmail让用户重新认识了浏览器的功能。

  2005年，Jesse将谷歌实现Gmail的技术命名为AJAX。从此前端技术正式出现。

  2006年，JQuery发布，JQuery是最长寿的JS库，其主要是兼容IE，但随着IE的落寞，JQuery也逐渐淡出前端开发者的视野。

### JS的爆发--V8引擎

  Chrome的JS引擎是V8（V1~V7是不同语言的引擎），V8引擎超快的速度让chrome成为了最主流的浏览器。

  2009年，Ryan基于V8，创建了Node.js；2010年Issac基于Node.js写出了npm。有了node.js，前端工程师实现了在浏览器之外执行JS。

  2010年，TJ受Sinatra的启发，发布了Express.js。Node.js与Express.js让前端工程师可以完成后端的内容。虽然还比不上Java，但是至少也具备了手段。

  借助Chrome的风，期间也爆发除了很多前端的技术：gulp、grunt、yeoman、require.js、webpack、Angular、React、Vue等。当然其中一些技术也已经过时了。

