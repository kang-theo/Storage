编写了一个tree.dot文件：
graph g {
    graph[ordering="out"];
    A--B;
    A--C;
    B--D;
    B--E;
    C--F;
    C--NULL[style="invis"];
    A[shape="circle"];
    B[shape="circle"];
    C[shape="circle"];
    D[shape="circle"];
    E[shape="circle"];
    F[shape="circle"];
    NULL[style="invis"];
}

Github上还有有人做了相关工作的 GraphViz formatting script for binary trees。 
 下载上面链接中的代码文件，然后对自己的原始dot文件执行如下命令： 
 （假设下载的代码文件名称为binarytree.gvpr，自己的dot文件名称为tree.dot，输出文件为tree.png）

dot tree.dot | gvpr -c -f binarytree.gvpr | neato -n -Tpng -o tree.png

file:///Users/kangchangyu/kiwichangyu/文件/mac_backup/DEVONthink/Kiwi_personal_3.dtBase2/Files.noindex/webarchive/4/使用graphviz绘制二叉树（二）%20-%20云+社区%20-%20腾讯云.webarchive