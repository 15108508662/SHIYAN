# SHIYAN
大数据181
张宏建
2018310997
掌握字符串String及其方法的使用 掌握异常处理结构

实验要求：

内容：利用已学的字符串处理知识编程完成《长恨歌》古诗的整理对齐工作，写出功能函数，并运行。达到如下功能：

    每7个汉字加入一个标点符号，奇数时加“，”，偶数时加“。”
    允许提供输入参数，统计古诗中某个字或词出现的次数
    考虑操作中可能出现的异常，在程序中设计异常处理程序

输入：汉皇重色思倾国御宇多年求不得杨家有女初长成养在深闺人未识天生丽质难自弃一朝选在君王侧回眸一笑百媚生六宫粉黛无颜色春寒赐浴华清池温泉水滑洗凝脂侍儿扶起娇无力始是新承恩泽时云鬓花颜金步摇芙蓉帐暖度春宵春宵苦短日高起从此君王不早朝承欢侍宴无闲暇春从春游夜专夜后宫佳丽三千人三千宠爱在一身金屋妆成娇侍夜玉楼宴罢醉和春姊妹弟兄皆列士可怜光采生门户遂令天下父母心不重生男重生女骊宫高处入青云仙乐风飘处处闻缓歌慢舞凝丝竹尽日君王看不足渔阳鼙鼓动地来惊破霓裳羽衣曲九重城阙烟尘生千乘万骑西南行<未完，待续> 输出： 汉皇重色思倾国，御宇多年求不得。 杨家有女初长成，养在深闺人未识。 天生丽质难自弃，一朝选在君王侧。 回眸一笑百媚生，六宫粉黛无颜色。 春寒赐浴华清池，温泉水滑洗凝脂。 侍儿扶起娇无力，始是新承恩泽时。 云鬓花颜金步摇，芙蓉帐暖度春宵。 春宵苦短日高起，从此君王不早朝。 …………

注意： 输入的内容，利用main方法中的args数组传递

建立一个main，输入排版的文章。System.out.print("输入排版的文章:"); Scanner input=new Scanner(System.in); String str=input.next(); 把输入的内容转为字符串数组。char ss[] = str.toCharArray();计算数组整除7的商。int count = ss.length/7; 利用for循环，循环次数是除以7的商。每次输出7个字，接着判断次数是奇数还是偶数，奇数加','，偶数加'.'。 for (int i=0; i<count; i++) { System.out.print(chs[(i7)]); System.out.print(chs[(i7)+1]); System.out.print(chs[(i7)+2]); System.out.print(chs[(i7)+3]); System.out.print(chs[(i7)+4]); System.out.print(chs[(i7)+5]); System.out.print(chs[(i*7)+6]); if (i % 2 == 0) System.out.print(','); else System.out.println('.'); } 查找文字部分，计算出整篇文章的长度。利用循环，次数是文字个数。判断输入文字的索引是否和0相同，如果不同就判断是否和1相同，之后也一样。如果相同，删除掉这个字符并计数count+1。最后输出次数。 int length=str.length(); int count = 0; int k = 0; for(int i= 0; i<=length; i++){ if(str.indexOf(s) == (i-k)){ str = str.substring(i-k+1,str.length()); count++; k = i+1; } 感想： 了解了循环的思想还有判断的方法，掌握字符串String及其方法的使用。
