运行环境需求：

安装gmssl库即可在pycharm中运行

实现方式：

这段代码是一个实现椭圆曲线密码算法（Elliptic Curve Cryptography，ECC）的Python程序。

首先，代码导入了一些必要的模块，包括math用于数学运算，random用于生成随机数，gmssl用于计算哈希值。

代码中定义了一些函数：

epoint_mod(a, n)：对a进行模n运算。

epoint_modmult(a, b, n)：计算(a * b) % n，其中b为二进制形式。

epoint_add(P, Q, a, p)：计算椭圆曲线上点P和点Q的相加结果，其中a和p为曲线参数。

epoint_mult(k, P, a, p)：计算椭圆曲线上点P和整数k的乘法结果，其中a和p为曲线参数。

keygen(a, p, n, G)：生成椭圆曲线密码的公钥和私钥，其中a和p为曲线参数，n为曲线阶数，G为基点。

isQR(n, p)：判断n是否为p的二次剩余。

QR(n, p)：计算n在模p下的平方根。

_hash(S)：计算一系列输入字符串S的哈希值。

在代码的主函数中，定义了一些曲线参数和一个基点G。然后调用keygen函数生成公钥和私钥，并打印出来。接下来，定义了一个输入字符串数组s，并调用_hash函数计算其哈希值，并打印出来。

运行结果：

<img width="415" alt="image" src="https://github.com/TraceAJ/project13/assets/110471272/77fbacb5-6dcf-4828-ae30-a2b3d12aca45">
