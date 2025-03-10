# 🦖的python板子

## 快读和递归深度

```python
import sys
sys.setrecursionlimit(1000000)#栈的最大深度
input=lambda:sys.stdin.readline().strip()
write=lambda x:sys.stdout.write(str(x)+'\n')
```

Python内置函数
--------------

| [abs()](https://www.runoob.com/python3/python3-func-number-abs.html)        | [dict()](https://www.runoob.com/python/python-func-dict.html)             | [help()](https://www.runoob.com/python/python-func-help.html)             | [min()](https://www.runoob.com/python3/python3-func-number-min.html)     | [setattr()](https://www.runoob.com/python/python-func-setattr.html)           |
| --------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------ | ----------------------------------------------------------------------------- |
| [all()](https://www.runoob.com/python/python-func-all.html)                 | [dir()](https://www.runoob.com/python/python-func-dir.html)               | [hex()](https://www.runoob.com/python3/python3-func-hex.html)             | [next()](https://www.runoob.com/python/python-func-next.html)            | [slice()](https://www.runoob.com/python/python-func-slice.html)               |
| [any()](https://www.runoob.com/python/python-func-any.html)                 | [divmod()](https://www.runoob.com/python3/python3-func-divmod.html)       | [id()](https://www.runoob.com/python/python-func-id.html)                 | [object()](https://www.runoob.com/python3/python-func-object.html)       | [sorted()](https://www.runoob.com/python3/python3-func-sorted.html)           |
| [ascii()](https://www.runoob.com/python3/python3-func-ascii.html)           | [enumerate()](https://www.runoob.com/python3/python3-func-enumerate.html) | [input()](https://www.runoob.com/python/python3-func-input.html)          | [oct()](https://www.runoob.com/python/python3-func-oct.html)             | [staticmethod()](https://www.runoob.com/python/python-func-staticmethod.html) |
| [bin()](https://www.runoob.com/python/python-func-bin.html)                 | [eval()](https://www.runoob.com/python/python-func-eval.html)             | [int()](https://www.runoob.com/python/python-func-int.html)               | [open()](https://www.runoob.com/python3/python3-func-open.html)          | [str()](https://www.runoob.com/python/python-func-str.html)                   |
| [bool()](https://www.runoob.com/python/python-func-bool.html)               | [exec()](https://www.runoob.com/python3/python3-func-exec.html)           | [isinstance()](https://www.runoob.com/python/python-func-isinstance.html) | [ord()](https://www.runoob.com/python3/python3-func-ord.html)            | [sum()](https://www.runoob.com/python/python-func-sum.html)                   |
| [bytearray()](https://www.runoob.com/python/python-func-bytearray.html)     | [filter()](https://www.runoob.com/python3/python3-func-filter.html)       | [issubclass()](https://www.runoob.com/python/python-func-issubclass.html) | [pow()](https://www.runoob.com/python3/python3-func-number-pow.html)     | [super()](https://www.runoob.com/python/python-func-super.html)               |
| [bytes()](https://www.runoob.com/python3/python3-func-bytes.html)           | [float()](https://www.runoob.com/python/python-func-float.html)           | [iter()](https://www.runoob.com/python/python-func-iter.html)             | [print()](https://www.runoob.com/python/python-func-print.html)          | [tuple()](https://www.runoob.com/python3/python3-func-tuple.html)             |
| [callable()](https://www.runoob.com/python/python-func-callable.html)       | [format()](https://www.runoob.com/python/att-string-format.html)          | [len()](https://www.runoob.com/python3/python3-string-len.html)           | [property()](https://www.runoob.com/python/python-func-property.html)    | [type()](https://www.runoob.com/python/python-func-type.html)                 |
| [chr()](https://www.runoob.com/python3/python3-func-chr.html)               | [frozenset()](https://www.runoob.com/python/python-func-frozenset.html)   | [list()](https://www.runoob.com/python3/python3-att-list-list.html)       | [range()](https://www.runoob.com/python3/python3-func-range.html)        | [vars()](https://www.runoob.com/python/python-func-vars.html)                 |
| [classmethod()](https://www.runoob.com/python/python-func-classmethod.html) | [getattr()](https://www.runoob.com/python/python-func-getattr.html)       | [locals()](https://www.runoob.com/python/python-func-locals.html)         | [repr()](https://www.runoob.com/python/python-func-repr.html)            | [zip()](https://www.runoob.com/python3/python3-func-zip.html)                 |
| [compile()](https://www.runoob.com/python/python-func-compile.html)         | [globals()](https://www.runoob.com/python/python-func-globals.html)       | [map()](https://www.runoob.com/python/python3-func-map.html)              | [reversed()](https://www.runoob.com/python3/python3-func-reversed.html)  | [__import__()](https://www.runoob.com/python/python-func-__import__.html)     |
| [complex()](https://www.runoob.com/python/python-func-complex.html)         | [hasattr()](https://www.runoob.com/python/python-func-hasattr.html)       | [max()](https://www.runoob.com/python3/python3-func-number-max.html)      | [round()](https://www.runoob.com/python3/python3-func-number-round.html) | [reload()](https://www.runoob.com/python3/python3-func-reload.html)           |
| [delattr()](https://www.runoob.com/python/python-func-delattr.html)         | [hash()](https://www.runoob.com/python/python-func-hash.html)             | [memoryview()](https://www.runoob.com/python/python-func-memoryview.html) | [set()](https://www.runoob.com/python/python-func-set.html)              | 参数可以help查一下                                                                   |

## math

Python **math** 模块提供了许多对浮点数的数学运算函数。**math** 模块下的函数，返回值均为浮点数，除非另有明确说明。

如果你需要计算复数，请使用 cmath 模块中的同名函数。要使用 math 函数必须先导入, 查看 math 模块中的内容:

>  import math   dir(math)  

### math 模块常量

| 常量                                                           | 描述                                                        |
| ------------------------------------------------------------ | --------------------------------------------------------- |
| [math.e](https://www.runoob.com/python3/ref-math-e.html)     | 返回欧拉数 (2.7182...)                                         |
| [math.inf](https://www.runoob.com/python3/ref-math-inf.html) | 返回正无穷大浮点数                                                 |
| [math.nan](https://www.runoob.com/python3/ref-math-nan.html) | 返回一个浮点值 NaN (not a number)                                |
| [math.pi](https://www.runoob.com/python3/ref-math-pi.html)   | π 一般指圆周率。 圆周率 PI (3.1415...)                              |
| [math.tau](https://www.runoob.com/python3/ref-math-tau.html) | 数学常数 τ = 6.283185...，精确到可用精度。Tau 是一个圆周常数，等于 2π，圆的周长与半径之比。 |

### math 模块方法

| 方法                                                                             | 描述                                                                                                             |
| ------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------- |
| [math.acos(x)](https://www.runoob.com/python3/ref-math-acos.html)              | 返回 x 的反余弦，结果范围在 0 到 pi 之间。                                                                                     |
| [math.acosh(x)](https://www.runoob.com/python3/ref-math-acosh.html)            | 返回 x 的反双曲余弦值。                                                                                                  |
| [math.asin(x)](https://www.runoob.com/python3/ref-math-asin.html)              | 返回 x 的反正弦值，结果范围在 -pi/2 到 pi/2 之间。                                                                              |
| [math.asinh(x)](https://www.runoob.com/python3/ref-math-asinh.html)            | 返回 x 的反双曲正弦值。                                                                                                  |
| [math.atan(x)](https://www.runoob.com/python3/ref-math-atan.html)              | 返回 x 的反正切值，结果范围在 -pi/2 到 pi/2 之间。                                                                              |
| [math.atan2(y, x)](https://www.runoob.com/python3/ref-math-atan2.html)         | 返回给定的 X 及 Y 坐标值的反正切值，结果是在 -pi 和 pi 之间。                                                                         |
| [math.atanh(x)](https://www.runoob.com/python3/ref-math-atanh.html)            | 返回 x 的反双曲正切值。                                                                                                  |
| [math.ceil(x)](https://www.runoob.com/python3/ref-math-ceil.html)              | 将 x 向上舍入到最接近的整数                                                                                                |
| [math.comb(n, k)](https://www.runoob.com/python3/ref-math-comb.html)           | 返回不重复且无顺序地从 n 项中选择 k 项的方式总数。                                                                                   |
| [math.copysign(x, y)](https://www.runoob.com/python3/ref-math-copysign.html)   | 返回一个基于 x 的绝对值和 y 的符号的浮点数。                                                                                      |
| [math.cos()](https://www.runoob.com/python3/ref-math-cos.html)                 | 返回 x 弧度的余弦值。                                                                                                   |
| [math.cosh(x)](https://www.runoob.com/python3/ref-math-cosh.html)              | 返回 x 的双曲余弦值。                                                                                                   |
| [math.degrees(x)](https://www.runoob.com/python3/ref-math-degrees.html)        | 将角度 x 从弧度转换为度数。                                                                                                |
| [math.dist(p, q)](https://www.runoob.com/python3/ref-math-dist.html)           | 返回 p 与 q 两点之间的欧几里得距离，以一个坐标序列（或可迭代对象）的形式给出。 两个点必须具有相同的维度。                                                       |
| [math.erf(x)](https://www.runoob.com/python3/ref-math-erf.html)                | 返回一个数的误差函数                                                                                                     |
| [math.erfc(x)](https://www.runoob.com/python3/ref-math-erfc.html)              | 返回 x 处的互补误差函数                                                                                                  |
| [math.exp(x)](https://www.runoob.com/python3/ref-math-exp.html)                | 返回 e 的 x 次幂，Ex， 其中 e = 2.718281... 是自然对数的基数。                                                                   |
| [math.expm1()](https://www.runoob.com/python3/ref-math-expm1.html)             | 返回 Ex - 1， e 的 x 次幂，Ex，其中 e = 2.718281... 是自然对数的基数。这通常比 math.e ** x 或 pow(math.e, x) 更精确。                      |
| [math.fabs(x)](https://www.runoob.com/python3/ref-math-fabs.html)              | 返回 x 的绝对值。                                                                                                     |
| [math.factorial(x)](https://www.runoob.com/python3/ref-math-factorial.html)    | 返回 x 的阶乘。 如果 x 不是整数或为负数时则将引发 ValueError。                                                                       |
| [math.floor()](https://www.runoob.com/python3/ref-math-floor.html)             | 将数字向下舍入到最接近的整数                                                                                                 |
| [math.fmod(x, y)](https://www.runoob.com/python3/ref-math-fmod.html)           | 返回 x/y 的余数                                                                                                     |
| [math.frexp(x)](https://www.runoob.com/python3/ref-math-frexp.html)            | 以 (m, e) 对的形式返回 x 的尾数和指数。 m 是一个浮点数， e 是一个整数，正好是 x == m * 2**e 。 如果 x 为零，则返回 (0.0, 0) ，否则返回 0.5 <= abs(m) < 1 。 |
| [math.fsum(iterable)](https://www.runoob.com/python3/ref-math-fsum.html)       | 返回可迭代对象 (元组, 数组, 列表, 等)中的元素总和，是浮点值。                                                                            |
| [math.gamma(x)](https://www.runoob.com/python3/ref-math-gamma.html)            | 返回 x 处的伽马函数值。                                                                                                  |
| [math.gcd()](https://www.runoob.com/python3/ref-math-gcd.html)                 | 返回给定的整数参数的最大公约数。                                                                                               |
| [math.hypot()](https://www.runoob.com/python3/ref-math-hypot.html)             | 返回欧几里得范数，sqrt(sum(x**2 for x in coordinates))。 这是从原点到坐标给定点的向量长度。                                               |
| [math.isclose(a,b)](https://www.runoob.com/python3/ref-math-isclose.html)      | 检查两个值是否彼此接近，若 a 和 b 的值比较接近则返回 True，否则返回 False。。                                                                |
| [math.isfinite(x)](https://www.runoob.com/python3/ref-math-isfinite.html)      | 判断 x 是否有限，如果 x 既不是无穷大也不是 NaN，则返回 True ，否则返回 False 。                                                            |
| [math.isinf(x)](https://www.runoob.com/python3/ref-math-isinf.html)            | 判断 x 是否是无穷大，如果 x 是正或负无穷大，则返回 True ，否则返回 False 。                                                                |
| [math.isnan()](https://www.runoob.com/python3/ref-math-isnan.html)             | 判断数字是否为 NaN，如果 x 是 NaN（不是数字），则返回 True ，否则返回 False 。                                                            |
| [math.isqrt()](https://www.runoob.com/python3/ref-math-isqrt.html)             | 将平方根数向下舍入到最接近的整数                                                                                               |
| [math.ldexp(x, i)](https://www.runoob.com/python3/ref-math-ldexp.html)         | 返回 x * (2**i) 。 这基本上是函数 [math.frexp() 的反函数。](https://www.runoob.com/python3/ref-math-frexp.html)               |
| [math.lgamma()](https://www.runoob.com/python3/ref-math-lgamma.html)           | 返回伽玛函数在 x 绝对值的自然对数。                                                                                            |
| [math.log(x[, base])](https://www.runoob.com/python3/ref-math-log.html)        | 使用一个参数，返回 x 的自然对数（底为 e ）。                                                                                      |
| [math.log10(x)](https://www.runoob.com/python3/ref-math-log10.html)            | 返回 x 底为 10 的对数。                                                                                                |
| [math.log1p(x)](https://www.runoob.com/python3/ref-math-log1p.html)            | 返回 1+x 的自然对数（以 e 为底）。                                                                                          |
| [math.log2(x)](https://www.runoob.com/python3/ref-math-log2.html)              | 返回 x 以 2 为底的对数                                                                                                 |
| [math.perm(n, k=None)](https://www.runoob.com/python3/ref-math-perm.html)      | 返回不重复且有顺序地从 n 项中选择 k 项的方式总数。                                                                                   |
| [math.pow(x, y)](https://www.runoob.com/python3/ref-math-pow.html)             | 将返回 x 的 y 次幂。                                                                                                  |
| [math.prod(iterable)](https://www.runoob.com/python3/ref-math-prod.html)       | 计算可迭代对象中所有元素的积。                                                                                                |
| [math.radians(x)](https://www.runoob.com/python3/ref-math-radians.html)        | 将角度 x 从度数转换为弧度。                                                                                                |
| [math.remainder(x, y)](https://www.runoob.com/python3/ref-math-remainder.html) | 返回 IEEE 754 风格的 x 除于 y 的余数。                                                                                    |
| [math.sin(x)](https://www.runoob.com/python3/ref-math-sin.html)                | 返回 x 弧度的正弦值。                                                                                                   |
| [math.sinh(x)](https://www.runoob.com/python3/ref-math-sinh.html)              | 返回 x 的双曲正弦值。                                                                                                   |
| [math.sqrt(x)](https://www.runoob.com/python3/ref-math-sqrt.html)              | 返回 x 的平方根。                                                                                                     |
| [math.tan(x)](https://www.runoob.com/python3/ref-math-tan.html)                | 返回 x 弧度的正切值。                                                                                                   |
| [math.tanh(x)](https://www.runoob.com/python3/ref-math-tanh.html)              | 返回 x 的双曲正切值。                                                                                                   |
| [math.trunc(x)](https://www.runoob.com/python3/ref-math-trunc.html)            | 返回 x 截断整数的部分，即返回整数部分，删除小数部分                                                                                    |

## calendar

此模块的函数都是日历相关的，例如打印某月的字符月历。

星期一是默认的每周第一天，星期天是默认的最后一天。更改设置需调用calendar.setfirstweekday()函数。模块包含了以下内置函数：

| 序号  | 函数及描述                                                                                                                                                                                                                     |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1   | **calendar.calendar(year,w=2,l=1,c=6)**<br>返回一个多行字符串格式的 year 年年历，3 个月一行，间隔距离为 c。 每日宽度间隔为w字符。每行长度为 21* W+18+2* C。**l** 是每星期行数。                                                                                             |
| 2   | **calendar.firstweekday( )**<br>返回当前每周起始日期的设置。默认情况下，首次载入 calendar 模块时返回 0，即星期一。                                                                                                                                           |
| 3   | **calendar.isleap(year)**<br>是闰年返回 True，否则为 False。<br><br>>>> import calendar<br>>>> print(calendar.isleap(2000))<br>True<br>                                                                                             |
| 4   | **calendar.leapdays(y1,y2)**<br>返回在Y1，Y2两年之间的闰年总数。                                                                                                                                                                        |
| 5   | **calendar.month(year,month,w=2,l=1)**<br>返回一个多行字符串格式的year年month月日历，两行标题，一周一行。每日宽度间隔为w字符。每行的长度为7* w+6。l是每星期的行数。                                                                                                           |
| 6   | **calendar.monthcalendar(year,month)**<br>返回一个整数的单层嵌套列表。每个子列表装载代表一个星期的整数。Year年month月外的日期都设为0;范围内的日子都由该月第几日表示，从1开始。                                                                                                        |
| 7   | **calendar.monthrange(year,month)**<br>返回两个整数。第一个是该月的星期几，第二个是该月有几天。星期几是从0（星期一）到 6（星期日）。<br>>>> import calendar<br>>>> calendar.monthrange(2014, 11)<br>(5, 30)<br>解释：5 表示 2014 年 11 月份的第一天是周六，30 表示 2014 年 11 月份总共有 30 天。 |
| 8   | **calendar.prcal(year, w=0, l=0, c=6, m=3)**<br>相当于 print (calendar.calendar(year, w=0, l=0, c=6, m=3))。                                                                                                                  |
| 9   | **calendar.prmonth(theyear, themonth, w=0, l=0)**<br>相当于 print(calendar.month(theyear, themonth, w=0, l=0))。                                                                                                              |
| 10  | **calendar.setfirstweekday(weekday)**<br>设置每周的起始日期码。0（星期一）到6（星期日）。                                                                                                                                                        |
| 11  | **calendar.timegm(tupletime)**<br>和time.gmtime相反：接受一个时间元组形式，返回该时刻的时间戳（1970纪元后经过的浮点秒数）。                                                                                                                                    |
| 12  | **calendar.weekday(year,month,day)**<br>返回给定日期的日期码。0（星期一）到6（星期日）。月份为 1（一月） 到 12（12月）。                                                                                                                                     |

## datetime

python中时间日期格式化符号：

* %y 两位数的年份表示（00-99）
* %Y 四位数的年份表示（000-9999）
* %m 月份（01-12）
* %d 月内中的一天（0-31）
* %H 24小时制小时数（0-23）
* %I 12小时制小时数（01-12）
* %M 分钟数（00=59）
* %S 秒（00-59）
* %a 本地简化星期名称
* %A 本地完整星期名称
* %b 本地简化的月份名称
* %B 本地完整的月份名称
* %c 本地相应的日期表示和时间表示
* %j 年内的一天（001-366）
* %p 本地A.M.或P.M.的等价符
* %U 一年中的星期数（00-53）星期天为星期的开始
* %w 星期（0-6），星期天为星期的开始
* %W 一年中的星期数（00-53）星期一为星期的开始
* %x 本地相应的日期表示
* %X 本地相应的时间表示
* %Z 当前时区的名称
* %% %号本身

### datetime.date

```python
d = datetime.date(2019, 4, 13)
d = date.fromtimestamp(156244364)
print("日期 =", d)#日期 = 2019-12-13
from datetime import date
today = date.today() 
print(today.year, today.month, today.day)
```

### datetime.time

```python
from datetime import time
# time(hour, minute and second)
b = time(11, 34, 56)
c = time(hour = 11, minute = 34, second = 56)
# time(hour, minute, second, microsecond)
d = time(11, 34, 56, 234566)
print("d =", d)
#输出为：
d = 11:34:56.234566
#创建time对象后，您可以轻松打印其属性，例如小时，分钟等。
a = time(11, 34, 56)
print("小时=", a.hour)
print("分钟=", a.minute)
print("秒=", a.second)
```

### datetime.datetime

```python
from datetime import datetime
#datetime(year, month, day)
a = datetime(2019, 11, 28)
# datetime(year, month, day, hour, minute, second, microsecond)
b = datetime(2019, 11, 28, 23, 55, 59, 342380)
print(b)#2019-11-28 23:55:59.342380
print(a.minute)#55
print(a.timestamp())#1577548559.34238
```

### datetime.timedelta

```python
t4 = datetime(year = 2018, month = 7, day = 12, hour = 7, minute = 9, second = 33)
t5 = datetime(year = 2019, month = 6, day = 10, hour = 5, minute = 55, second = 13)
t6 = t4 - t5
print("t6 =", t6)#t6 = -333 days, 1:14:20

t1 = timedelta(weeks = 2, days = 5, hours = 1, seconds = 33)
t2 = timedelta(days = 4, hours = 11, minutes = 4, seconds = 54)
t3 = t1 - t2
print("t3 =", t3)#t3 = 14 days, 13:55:39
print("t3 =", abs(t3))#取绝对值
print("total seconds =", t3.total_seconds())#获得timedelta对象中的总秒数

```

### Python格式日期时间

```python
s1 = now.strftime("%m/%d/%Y, %H:%M:%S")
# mm/dd/YY H:M:S format
print("s1:", s1)#s1: 12/26/2018, 04:34:52
#strptime()方法从一个给定的字符串(表示日期和时间)创建一个datetime对象
date_string = "21 June, 2018"
date_object = datetime.strptime(date_string, "%d %B, %Y")
print("date_object =", date_object)#date_object = 2018-06-21 00:00:00
#strftime()方法使用date，time或datetime对象返回表示日期和时间的字符串
now = datetime.now()
date_time = now.strftime("%m/%d/%Y, %H:%M:%S")
print("日期和时间:",date_time)#日期和时间: 04/13/2020, 17:35:22
```

## collections

| 子类           | 简介                                       |
| ------------ | ---------------------------------------- |
| namedtuple() | 创建命名元组子类的工厂函数，生成可以使用名字来访问元素内容的tuple子类    |
| deque        | 类似列表(list)的容器，实现了在两端快速添加(append)和弹出(pop) |
| ChainMap     | 类似字典(dict)的容器类，将多个映射集合到一个视图里面            |
| Counter      | 字典的子类，提供了可哈希对象的计数功能                      |
| OrderedDict  | 字典的子类，保存了他们被添加的顺序，有序字典                   |
| defaultdict  | 字典的子类，提供了一个工厂函数，为字典查询提供一个默认值             |
| UserDict     | 封装了字典对象，简化了字典子类化                         |
| UserList     | 封装了列表对象，简化了列表子类化                         |
| UserString   | 封装了字符串对象，简化了字符串子类化                       |

### Counter

Counter是一个dict的子类，用于**计数可哈希对象**

```python
#计算top10的单词
from collections import Counter
import re
text = 'remove an existing key one level down remove an existing key one level down'
words = re.findall(r'\w+', text)
Counter(words).most_common(10)
#[('remove', 2),('an', 2),('existing', 2),('key', 2),('one', 2)('level', 2),('down', 2)] 


#计算列表中单词的个数
cnt = Counter()
for word in ['red', 'blue', 'red', 'green', 'blue', 'blue']:
    cnt[word] += 1
cnt
#Counter({'red': 2, 'blue': 3, 'green': 1})

#下面的方法更简单，直接计算就行
L = ['red', 'blue', 'red', 'green', 'blue', 'blue'] 
Counter(L)
#Counter({'red': 2, 'blue': 3, 'green': 1})

#字符串计数
c = Counter('programming')
#Counter({'g': 2, 'm': 2, 'r': 2, 'a': 1, 'i': 1, 'o': 1, 'n': 1, 'p': 1})
c.update('hello') # 也可以一次性update
#Counter({'r': 2, 'o': 2, 'g': 2, 'm': 2, 'l': 2, 'p': 1, 'a': 1, 'i': 1, 'n': 1, 'h': 1, 'e': 1})
#subtract从迭代对象或映射对象减去元素。输入和输出都可以是0或者负数。
c = Counter(a=4, b=2, c=0, d=-2)
d = Counter(a=1, b=2, c=3, d=4)
c.subtract(d)
c
#Counter({'a': 3, 'b': 0, 'c': -3, 'd': -6})
c = Counter(a=3, b=1)
d = Counter(a=1, b=2)
c + d                       # add two counters together:  c[x] + d[x] (keeping only positive counts)
#Counter({'a': 4, 'b': 3})
c - d                       # subtract (keeping only positive counts)
#Counter({'a': 2})
c & d                       # intersection:  min(c[x], d[x]) 
#Counter({'a': 1, 'b': 1})
c | d                       # union:  max(c[x], d[x])
#Counter({'a': 3, 'b': 2})
```

### deque

```python
from collections import deque
q = deque(['a', 'b', 'c'])
q.append('x')
q.appendleft('y')
print(q)#deque(['y', 'a', 'b', 'c', 'x'])
print(q.pop())#x
print(q.popleft())#y
q.clear()#移除所有元素，使其长度为0

d = deque('ghi') # 创建一个deque
list(reversed(d))#['i', 'h', 'g']
d.extend('jkl')  # 一次添加多个元素
#rotate
d = deque('ghijkl')
d.rotate(1)                      
d
#deque(['l', 'g', 'h', 'i', 'j', 'k']
d.rotate(-1)                     
d
#deque(['g', 'h', 'i', 'j', 'k', 'l'])
```

### defaultdict

```python
from collections import defaultdict
a=defaultdict(int)#设置default_factory为int，使得defaultdict可以用于计数
print(a[1])#0
dd = defaultdict(lambda: 'N/A')
dd['key1'] = 'abc'
dd['key1'] # key1存在
#'abc'
dd['key2'] # key2不存在，返回默认值
#'N/A' 

#使用list作为default_factory，很容易将一个key-value的序列转换为list字典；
s = [('yellow', 1), ('blue', 2), ('yellow', 3), ('blue', 4), ('red', 1)]
d = defaultdict(list)#将default_factory设置为set，可以建立一个集合字典
for k, v in s:
    d[k].append(v)
a = d.items()
print(a)
b = sorted(d.items())
print(b)
"""
dict_items([('yellow', [1, 3]), ('blue', [2, 4]), ('red', [1])])
[('blue', [2, 4]), ('red', [1]), ('yellow', [1, 3])]
"""


```

### ChainMap

```python
from collections import ChainMap
baseline = {'music': 'bach', 'art': 'rembrandt'}
adjustments = {'art': 'van gogh', 'opera': 'carmen'}
combined = ChainMap(adjustments, baseline)
```

### namedtuple

```python
from collections import namedtuple
# 定义一个namedtuple类型User，并包含name，sex和age属性
User = namedtuple('User', ['name', 'sex', 'age'])
# 创建一个User对象
user = User(name='Runoob', sex='male', age=12)
# 获取所有字段名
print(user._fields)
# 通过一个列表创建一个User对象，需要使用"_make"方法
user = User._make(['Runoob', 'male', 12])
# 获取用户的属性
print(user.name)
print(user.sex)
print(user.age)
# 修改对象属性，使用"_replace"方法
user = user._replace(age=22)
print(user)
# 将User对象转换成字典，使用"_asdict"
print(user._asdict())2)
```

## heapq

```python
import heapq
a = []   #创建一个空堆
#heapq.heappush()是往堆中添加新值，此时自动建立了小根堆
heapq.heappush(a,18)
heapq.heappush(a,1)
heapq.heappush(a,20)
heapq.heappush(a,10)
heapq.heappush(a,5)
print(a)#[1, 5, 20, 18, 10]

#但heapq里面没有直接提供建立大根堆的方法，可以采取如下方法：每次push时给元素加一个负号（即取相反数）
a = []
for i in [1, 5, 20, 18, 10, 200]:
    heapq.heappush(a,-i)
print(list(map(lambda x:-x,a)))#[200, 18, 20, 1, 10, 5]

#heapq.heapfy()是以线性时间将一个列表转化为小根堆
a = [1, 5, 20, 18, 10, 200]
heapq.heapify(a)#[1, 5, 20, 18, 10, 200]

#heapq.heappop()是从堆中弹出并返回最小的值
def heap_sort(arr):
    if not arr:
        return []
    h = []  #建立空堆
    for i in arr:
        heapq.heappush(h,i) #heappush自动建立小根堆
    return [heapq.heappop(h) for i in range(len(h))]  #heappop每次删除并返回列表中最小的值
```

## queue

```python
from queue import Queue   # 队列，FIFO
from queue import PriorityQueue  #优先级队列，优先级高的先输出

###############队列（Queue）的使用###############
q = Queue(maxsize)     #构建一个队列对象，maxsize初始化默认为零，此时队列无穷大
q.empty()        #判断队列是否为空(取数据之前要判断一下)
q.full()        #判断队列是否满了
q.put()            #向队列存放数据
q.get()            #从队列取数据
q.qsize()        #获取队列大小，

###用法示例：
>>> q = Queue(3)>>> for i in range(3):
>>>    q.put(i)
>>> q.full()
True
>>> while not q.empty():
>>>     print(q.get())
0
1
2
###############优先队列（PriorityQueue）的使用###############
"""
队列的变体，按优先级顺序（最低优先）检索打开的条目。
条目通常是以下格式的元组：
插入格式：q.put((priority number, data))
特点：priority number 越小，优先级越高
其他的操作和队列相同
"""
>>> q = PriorityQueue()
>>> q.put((2, "Lisa"))
>>> q.put((1, "Lucy"))
>>> q.put((0, "Tom"))

>>> i = 0
>>> while i < q.qsize()：
>>>     print(q.get())
(0，"Tom")
(1，"Lucy")
(2，"Lisa")

#如果我们需要根据自定义的规则进行排序，可以通过重载类的 __lt__ 方法来实现。
import queue
class person(object):
    def __init__(self,name,score):
        self.name = name
        self.score = score
    def __lt__(self, other):
        return self.score > other.score
p1 = person("张三",15)
p2 = person("李四",23)
p3 = person("王五",12)
p4 = person("朱五",32)
que = queue.PriorityQueue()
que.put(p1)
que.put(p2)
que.put(p4)
que.put(p3)
print(que.get().name)
```

## bisect

| 名称                       | 功能                                    |
| ------------------------ | ------------------------------------- |
| **bisect_left(list,x)**  | **查找** 如果插入目标元素x，插入在可行位置最左侧，插入后的index |
| **bisect_right(list,x)** | **查找** 如果插入目标元素x，插入在可行位置最右侧，插入后的index |
| **bisect(list,x)**       | 同 bisect_right()                      |
| **insort_left(list,x)**  | 查找左侧插入点，并保序地 **插入** 元素x               |
| **insort_right(list,x)** | 查找右侧插入点，并保序地 **插入** 元素x               |
| **insort(list,x)**       | 同 insort_right()                      |

```python
>>> from bisect import *
>>> def grade(score, breakpoints=[60, 70, 80, 90], grades='FDCBA'):
...     i = bisect(breakpoints, score)
...     return grades[i]
... 
>>> [grade(score) for score in [33, 99, 77, 70, 89, 90, 100]]  # 列表解析式 按成绩划分等级
['F', 'A', 'C', 'C', 'B', 'A', 'A']
```

## functools

```python
from functools import cmp_to_key
#将 旧式的比较函数 转换为 关键字函数
def compare(ele1, ele2):
    return ele2 - ele1
a = [2, 3, 1]
print(sorted(a, key=cmp_to_key(compare)))#相当于reverse=True
'''
[3, 2, 1]
'''
from functools import cache,lru_cache,reduce
@cache
def fibonacci(n):
    if n < 2:
        return n
    else:
        return fibonacci(n-1) + fibonacci(n-2)
print(fibonacci(100))
# 清空缓存
fibonacci.cache_clear()

@lru_cache(maxsize=128)
def fibonacci(n):
    if n < 2:
        return n
    else:
        return fibonacci(n-1) + fibonacci(n-2)
print(fibonacci(10))

# 将数字列表组合成单个数字
digits = [3, 4, 2, 5]
number = reduce(lambda x, y: x * 10 + y, digits)#reduce会将一个函数应用于序列中的元素，从左到右。
print(number) # 输出: 3425
```

## itertools

| 迭代器                             | 实参                   | 结果                  |
| ------------------------------- | -------------------- | ------------------- |
| product()                       | p, q, ... [repeat=1] | 笛卡尔积，相当于嵌套的for循环    |
| permutations()                  | p[, r]               | 长度r元组，所有可能的排列，无重复元素 |
| combinations()                  | p, r                 | 长度r元组，有序，无重复元素      |
| combinations_with_replacement() | p, r                 | 长度r元组，有序，元素可重复      |

| 例子                                       | 结果                                              |
| ---------------------------------------- | ----------------------------------------------- |
| product('ABCD', repeat=2)                | AA AB AC AD BA BB BC BD CA CB CC CD DA DB DC DD |
| permutations('ABCD', 2)                  | AB AC AD BA BC BD CA CB CD DA DB DC             |
| combinations('ABCD', 2)                  | AB AC AD BC BD CD                               |
| combinations_with_replacement('ABCD', 2) | AA AB AC AD BB BC BD CC CD DD                   |

有限迭代器

| 迭代器          | 实参                     | 结果                       | 示例                                      |
| ------------ | ---------------------- | ------------------------ | --------------------------------------- |
| accumulate() | p [,func=operator.add] | p0, p0+p1, p0+p1+p2, ... | accumulate([1,2,3,4,5]) --> 1 3 6 10 15 |

## operator

标准运算符对应函数，可用于accumulate()

| 运算     | 语法           | 函数                   | 运算     | 语法            | 函数                   |
| ------ | ------------ | -------------------- | ------ | ------------- | -------------------- |
| 加法     | `a + b`      | `add(a, b)`          | 字符串拼接  | `seq1 + seq2` | `concat(seq1, seq2)` |
| 包含测试   | `obj in seq` | `contains(seq, obj)` | 除法     | `a / b`       | `truediv(a, b)`      |
| 除法     | `a // b`     | `floordiv(a, b)`     | 按位与    | `a & b`       | `and_(a, b)`         |
| 按位异或   | `a ^ b`      | `xor(a, b)`          | 按位取反   | `~ a`         | `invert(a)`          |
| 按位或    | `a \| b`     | `or_(a, b)`          | 取幂     | `a ** b`      | `pow(a, b)`          |
| 左移     | `a << b`     | `lshift(a, b)`       | 取模     | `a % b`       | `mod(a, b)`          |
| 乘法     | `a * b`      | `mul(a, b)`          | 矩阵乘法   | `a @ b`       | `matmul(a, b)`       |
| 取反（算术） | `- a`        | `neg(a)`             | 取反（逻辑） | `not a`       | `not_(a)`            |
| 正数     | `+ a`        | `pos(a)`             | 右移     | `a >> b`      | `rshift(a, b)`       |
| 字符串格式化 | `s % obj`    | `mod(s, obj)`        | 减法     | `a - b`       | `sub(a, b)`          |
| 真值测试   | `obj`        | `truth(obj)`         | 比较     | `a < b`       | `lt(a, b)`           |
| 比较     | `a <= b`     | `le(a, b)`           | 相等     | `a == b`      | `eq(a, b)`           |
| 不等     | `a != b`     | `ne(a, b)`           | 比较     | `a >= b`      | `ge(a, b)`           |
| 比较     | `a > b`      | `gt(a, b)`           |        |               |                      |

key不用 lambda 函数，而使用 itemgetter 函数，速度更快

```python
import operator
#多级排序。先按第二个元素排序，再按第一个元素排序：
data = [(1, 'b'), (2, 'a'), (3, 'b')]
sorted_data = sorted(data, key=operator.itemgetter(1, 0))
print(sorted_data) # 输出: [(2, 'a'), (1, 'b'), (3, 'b')] 
#attrgetter 可以 获取 对象的属性, 然后进行 排序 操作 
print(sorted(students, key=attrgetter('age'), reverse=True))
```

## 常用数据结构

```python
1. 列表（List）
列表是Python中最常用的数据结构之一，支持动态大小，能够以简单的方式存储多个项目。以下是一些基本操作：
fruits = ['apple', 'banana', 'cherry']
# 添加元素
fruits.append('orange')
# 删除元素
fruits.remove('banana')
# 查找元素
if 'apple' in fruits:
    print("Apple is in the list!")
新手易踩坑：在使用列表时，注意索引从0开始。如果你试图访问一个超出范围的索引，Python会抛出IndexError。

2. 字典（Dictionary）
字典是一种无序的键值对集合，适合用于快速查找。它的查找速度非常快，通常是O(1)。
student = {'name': 'Alice', 'age': 20}
# 添加元素
student['grade'] = 'A'
# 删除元素
del student['age']
# 查找元素
print(student.get('name'))
新手易踩坑：字典的键必须是不可变类型（如字符串、数字、元组），而值可以是任意类型。

3. 集合（Set）
集合是一种无序且不重复的元素集合，适合用于去重和集合运算。
numbers = {1, 2, 3, 4, 5}
# 添加元素
numbers.add(6)
# 删除元素
numbers.discard(3)
# 集合运算
even_numbers = {2, 4, 6}
print(numbers.intersection(even_numbers))
新手易踩坑：集合中的元素是无序的，因此不能通过索引访问。

4. 栈（Stack）
栈是一种后进先出（LIFO）的数据结构。我们可以使用列表来实现栈的功能。
stack = []
# 入栈
stack.append(1)
# 出栈
top = stack.pop()
新手易踩坑：在使用栈时，确保在出栈之前栈中有元素，否则会抛出IndexError。

5. 队列（Queue）
队列是一种先进先出（FIFO）的数据结构。我们可以使用collections模块中的deque来实现队列。
from collections import deque
queue = deque()
# 入队
queue.append(1)
# 出队
first = queue.popleft()
新手易踩坑：使用列表实现队列时，出队操作会导致O(n)的时间复杂度，因此推荐使用deque。

常用算法
1. 排序算法
排序是数据处理中的基本操作之一。Python内置的sorted()函数和列表的sort()方法都可以轻松实现排序
sorted_list = sorted([3, 1, 4, 1, 5, 9])# 使用sorted()函数
numbers = [3, 1, 4, 1, 5, 9]# 使用sort()方法
numbers.sort()
新手易踩坑：注意sorted()返回一个新列表，而sort()是在原地排序。

2. 查找算法
查找算法用于在数据结构中查找特定元素。最常用的查找算法是线性查找和二分查找。
# 二分查找
def binary_search(arr, target):
    left, right = 0, len(arr) - 1
    while left <= right:
        mid = (left + right) // 2
        if arr[mid] == target:
            return mid
        elif arr[mid] < target:
            left = mid + 1
        else:
            right = mid - 1
    return -1
新手易踩坑：在使用二分查找时，确保数据是有序的，否则结果将不可靠。
```
