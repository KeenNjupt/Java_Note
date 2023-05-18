## java文档注释
文档注释格式:  
/**  
*javadoc标签 标签内容  
*/

举例说明：
```
//文档注释, 使用方式: javadoc -d 放置文档注释文件的文件夹名 -x -y test.java
//x，y表示test.java中使用的javadoc标签， test.java表示java源文件
//举例 javadoc -d E:\Code\Code_Java_VSCode\escape_character\javadocdir -author -version escape_char.java
//将生成的index.html在浏览器中打开即可
/**
 * @author keen
 * @version 1.0
 */

public class escape_char {
    public static void main(String[] args){
        System.out.println("你好\t 你们好\t");
    }
}
```
