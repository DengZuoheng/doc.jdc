##JDC技术成员面试##

###1.面试对象###
原则上对所有报名成员面试,包括但不限于:

- MM
    + 主程(原则上是三年级及以上)
    + 测试(原则上二年级及以上)
    + 美术(年级不限,有完美主义,强迫症者优先)
    + 产品设计(原则上二年级及以上,有完美主义,强迫症者优先)
- JDC
    + 主程(年级不限)
    + 测试(年级不限)
    + 生力军(一年级)

###2.面试准则###
- MM对主程,美术和测试设技术要求
- JDC不设技术要求
- 一般情况下,对没有设技术要求的职位,面试不影响录取结果
- 缺席面试者一律不予技术成员资格

###3.面试策略###
- 面试官
    + JDC技术负责人/管理员:邓作恒
    + JDC/JDC技术负责人:杨雅希
- 场地
    + 由JDC执行委员会安排
- 时间
    + 由JDC执行委员会安排
- 面试环境
    + 尽量以轻松自由的气氛面试
    <!--毕竟主要是面主程序员,太严肃是没有意义的,正装完全没必要,短裤拖鞋也是允许的-->
- 必须物料
    + 黑板或白板
    + 粉笔或白板笔
    + 饮用水(面试官及面试者)<!--天晓得面多久,水都没得喝太没人道了== -->
    + 草稿纸<!--给面试者整理思路的-->
- **每次面一人**

###4.提问
- 主程
    + 计算机科学
        - 数据结构
            + 数组与链表的差异
            + 解释哈希表的简单实现及冲突处理
            + 红黑树使用例子,优点与缺点
        - 算法(不问)
        - 编程体系
            + 编译器,连接器,解释器的区别
            + 多线程
    + 软件工程
        - 版本控制
            + 通过日期备份文件夹有何优劣
            + CVS有何优劣
            + Git有何特点
            + SVN与Git对比
        - 自动化编译
            + IDE与编译器的区别
        - 自动化测试
            + 对测试的理解
            + 单元测试的使用体验
            + 什么叫测试驱动开发
            + 自动UI测试是否靠谱
    + 经验
        - 写过的最长最复杂的程序是干什么的
            + 根据回答取其中细节询问 
                - 比如用了什么第三方库,开源否,怎么测试
                - 其中某一特性是什么实现的
        - 没写过
            + 临时构思一个项目
                - 比如空课表的储存与空课同学的检索
                - 比如统计项目源码行数的软件
                - 比如电费到期通知的服务
    + 程序设计
        - C++(异常与智能指针)
            <pre><code>
                void Foo(Male* programer)
                {
                    
                    if(!programer.has_girlfriend())
                    {
                        beauty = new Female();
                        Blind_date(programer,beauty);
                    }
                    
                }
                void Blind_date(Male* male,Female* female)
                {
                    if(male->career==Humen::PROGRAMER)
                    {
                        throw logic_error("Programmers condemned to a life of loneliness!");
                    }
                    ...
                }
            </code></pre>
        - C(函数指针)
            <pre>
                int foo(double,char);
                void bar(const char *);
                //现在要定义一个foobar函数,调用时参数为foo,返回值为bar
            </pre>
            正解:
            <pre><code>
                int foo(double,char);
                void bar(const char*);
                void(*foobar(int(*)(double,char)))(const char *);
                //用typedef就容易了
                int main()
                {
                    void(*pf)(const char*)=foobar(foo);
                }
            </code></pre>
    + 聊人生
        - 对开源的看法

- 测试
    + java单元测试
    + cpp 单元测试
    + python 单元测试
    + UI测试
- 美术
    + 常用的图片编辑工具
    + 鼠绘和板绘能力
- 产品设计
    + 
       
**参考**  
\[1]:程序员能力矩阵.http://static.icybear.net/%5BCN%5DProgrammer%20competency%20matrix.htm