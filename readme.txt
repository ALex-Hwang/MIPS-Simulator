MIPS虚拟机
--version 1.0
1.支持汇编以及反汇编
2. 汇编支持指令支持ZPC中的42的基本指令
3. 反汇编支持寄存器操作以及LW和SW的内存操作
4. 支持debug指令

存在问题：
1. 没有对输入数据的格式进行检查
2. 机器码的输入必须为十六进制

--version 0.2
修复问题：
1. 修复只能输入正数的问题。（现在可以接收负数作为参数）
2. 修复offset的值，将其转变为接受参数的1/2 - 1，以保持和非常天空编译器的一致


--version 0.1
支持的操作：ZPC中的前43条
输入格式：参数之间用逗号分隔，有无空格都无所谓。其中dat和offset等请使用十进制输入
目前存在的问题：
1. 指令支持太少
2. 无法处理dat和offset为负的情况
3. 只能处理单条语句
4. 只能实现命令行及时输入输出

