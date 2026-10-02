# CPP习题（300题：题干 + 参考答案）

> 本文件由工作空间《CPP习题.docx》整理生成。全库共 **300 道 C++ 练习题**，按 **难度大类 → 知识中类 → 主题小类** 三级分类；每题依次展示题干、样例（如有）、参考答案（默认折叠，点击可展开）。

## 📚 使用说明

- **三套题库**：第一套（入门基础）、第二套（进阶提高）、第三套（CSP-J 竞赛入门）。
- **答案说明**：第一套参考答案取自 Word 文档原文；第二、三套优先取用 Word 文档中对应代码，未收录部分已逐题补充完整答案。全库 300 题均已配备可编译的 C++ 参考代码。
- **代码格式**：全部参考代码使用 Markdown `cpp` 语言代码块并默认折叠，点击「点击展开参考答案」即可查看，可直接复制到 Dev-C++ / VS Code / NOILinux 编译运行。

## 📑 目录

- **[入门基础（第一套 · C++趣味入门100题）](#第1类-入门基础-第一套-c趣味入门100题)**
  - [1.1 基础语法与输入输出](#11-基础语法与输入输出入门组)
  - [1.2 条件分支](#12-条件分支分支组)
  - [1.3 循环控制](#13-循环控制循环组)
  - [1.4 随机数与趣味游戏](#14-随机数与趣味游戏趣味进阶组)
- **[进阶提高（第二套 · C++进阶趣味100题）](#第2类-进阶提高-第二套-c进阶趣味100题)**
  - [2.1 函数与字符串](#21-函数与字符串函数与字符串专题)
  - [2.2 数组与vector](#22-数组与vector数组与vector专题)
  - [2.3 基础算法与数学](#23-基础算法与数学基础算法与数学专题)
  - [2.4 综合小游戏与实用工具](#24-综合小游戏与实用工具综合小游戏与实用工具)
- **[竞赛入门（第三套 · CSP-J算法入门100题）](#第3类-竞赛入门-第三套-csp-j算法入门100题)**
  - [3.1 模拟](#31-模拟模拟题)
  - [3.2 字符串专题](#32-字符串专题字符串专题)
  - [3.3 数组、前缀和与差分](#33-数组前缀和与差分数组前缀和差分)
  - [3.4 排序与查找](#34-排序与查找排序与查找)
  - [3.5 贪心算法](#35-贪心算法贪心算法)
  - [3.6 数论](#36-数论数论)
  - [3.7 递归、DFS与搜索](#37-递归dfs与搜索递归dfs搜索)
  - [3.8 简单动态规划](#38-简单动态规划简单动态规划dp)

---

## 第1类 · 入门基础 ｜ 第一套 · C++趣味入门100题

> 难度：★☆☆☆☆

### 1.1 基础语法与输入输出（入门组）

#### ▸ 小类 A：输出与变量

##### 1.1.01 自我介绍程序

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入姓名、年龄，输出：大家好，我叫XX，今年X岁。</div>

**样例**：

```text
样例输入：Tom 12 样例输出：大家好，我叫Tom，今年12岁。
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <string>
using namespace std;
int main()
{
    string name;
    int age;
    cin >> name >> age;
    cout << "大家好，我叫" << name << "，今年" << age << "岁。" << endl;
    return 0;
}
```

</details>

---

#### ▸ 小类 B：公式与单位换算

##### 1.1.02 长方形面积计算器

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入长和宽，计算长方形面积与周长。</div>

**样例**：

```text
样例输入：3 4 样例输出：面积=12 周长=14
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    double a,b;
    cin >> a >> b;
    double s = a * b;
    double c = 2*(a+b);
    cout << "面积=" << s << " 周长=" << c << endl;
    return 0;
}
```

</details>

---

##### 1.1.03 正方形计算器

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入边长，输出正方形周长、面积。</div>

**样例**：

```text
输入：5，输出：周长=20 面积=25
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    double len;
    cin >> len;
    cout << "周长=" << 4*len << " 面积=" << len*len << endl;
    return 0;
}
```

</details>

---

##### 1.1.04 千米转米转换器

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入千米数，换算成多少米。</div>

**样例**：

```text
输入：2.5，输出：2.5千米 = 2500米
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    double km;
    cin >> km;
    cout << km << "千米 = " << km*1000 << "米" << endl;
    return 0;
}
```

</details>

---

##### 1.1.05 分钟换算小时

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入总分钟数，换算成小时（小数形式）。例如输入90 → 1.5小时。</div>

**样例**：

```text
输入：90，输出：90分钟 = 1.5小时
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    double min;
    cin >> min;
    double h = min / 60.0;
    cout << min << "分钟 = " << h << "小时" << endl;
    return 0;
}
```

</details>

---

##### 1.1.06 温度转换（摄氏→华氏）

<div style="font-size:1.2em; line-height:1.7;">**题干**：公式：华氏度 = 摄氏度 × 1.8 +32，输入摄氏度输出华氏。</div>

**样例**：

```text
输入：20，输出：华氏度：68
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    double c;
    cin >> c;
    double f = c * 1.8 + 32;
    cout << "华氏度：" << f << endl;
    return 0;
}
```

</details>

---

##### 1.1.07 秒转分钟秒

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入总秒数，换算成多少分钟多少秒。例：125秒=2分5秒。</div>

**样例**：

```text
输入：125，输出：2分5秒
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int sec;
    cin >> sec;
    int m = sec / 60;
    int s = sec % 60;
    cout << m << "分" << s << "秒" << endl;
    return 0;
}
```

</details>

---

##### 1.1.08 三角形面积

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入底和高，计算三角形面积（面积=底×高÷2）。</div>

**样例**：

```text
输入：4 5，输出：三角形面积=10
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    double base, h;
    cin >> base >> h;
    double area = base * h / 2;
    cout << "三角形面积=" << area << endl;
    return 0;
}
```

</details>

---

##### 1.1.09 体重单位转换

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入斤，转换成千克（1kg=2斤）。</div>

**样例**：

```text
输入：120，输出：120斤 = 60kg
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    double jin;
    cin >> jin;
    cout << jin << "斤 = " << jin / 2.0 << "kg" << endl;
    return 0;
}
```

</details>

---

##### 1.1.10 跑步距离计算

<div style="font-size:1.2em; line-height:1.7;">**题干**：操场一圈400米，输入跑的圈数，算出总米数。</div>

**样例**：

```text
输入：3，输出：总距离：1200米
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int circle;
    cin >> circle;
    cout << "总距离：" << circle * 400 << "米" << endl;
    return 0;
}
```

</details>

---

##### 1.1.11 立方体体积

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入立方体边长，计算体积。</div>

**样例**：

```text
输入：3，输出：体积=27
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    double len;
    cin >> len;
    cout << "体积=" << len*len*len << endl;
    return 0;
}
```

</details>

---

#### ▸ 小类 C：生活场景计算

##### 1.1.12 水果收银台

<div style="font-size:1.2em; line-height:1.7;">**题干**：苹果8元/斤，香蕉5元/斤。输入苹果、香蕉购买斤数，算出总金额。</div>

**样例**：

```text
输入：2 3，输出：总金额：31元
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    double apple, banana;
    cin >> apple >> banana;
    double total = apple*8 + banana*5;
    cout << "总金额：" << total << "元" << endl;
    return 0;
}
```

</details>

---

##### 1.1.13 零花钱计算器

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入本周收到零花钱、花掉的钱，计算剩余零花钱。</div>

**样例**：

```text
输入：100 35，输出：剩余零花钱：65
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    double get, spend;
    cin >> get >> spend;
    cout << "剩余零花钱：" << get - spend << endl;
    return 0;
}
```

</details>

---

##### 1.1.14 购买笔记本

<div style="font-size:1.2em; line-height:1.7;">**题干**：笔记本每本3.5元，输入购买数量，求总价。</div>

**样例**：

```text
输入：4，输出：总价：14
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int n;
    cin >> n;
    double money = n * 3.5;
    cout << "总价：" << money << endl;
    return 0;
}
```

</details>

---

##### 1.1.15 平均分计算器

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入语文、数学两门分数，计算平均分。</div>

**样例**：

```text
输入：90 80，输出：平均分=85
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int chinese, math;
    cin >> chinese >> math;
    double avg = (chinese + math)/2.0;
    cout << "平均分=" << avg << endl;
    return 0;
}
```

</details>

---

##### 1.1.16 折扣计算器

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入商品原价，输入折扣（例如打8折就输入0.8），计算折后价格。</div>

**样例**：

```text
输入：100 0.8，输出：折后价：80
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    double price, rate;
    cin >> price >> rate;
    cout << "折后价：" << price * rate << endl;
    return 0;
}
```

</details>

---

##### 1.1.17 饮料兑换

<div style="font-size:1.2em; line-height:1.7;">**题干**：一瓶水2元，输入拥有的钱，算出最多能买几瓶（只算数量，不找零逻辑）。</div>

**样例**：

```text
输入：11，输出：最多购买：5瓶
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int money;
    cin >> money;
    cout << "最多购买：" << money / 2 << "瓶" << endl;
    return 0;
}
```

</details>

---

##### 1.1.18 速度计算

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入路程和时间，求平均速度（速度=路程÷时间）。</div>

**样例**：

```text
输入：100 2，输出：平均速度=50
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    double s, t;
    cin >> s >> t;
    cout << "平均速度=" << s / t << endl;
    return 0;
}
```

</details>

---

##### 1.1.19 邮票总面值

<div style="font-size:1.2em; line-height:1.7;">**题干**：一张邮票0.8元，输入邮票张数，计算总面值。</div>

**样例**：

```text
输入：5，输出：总面值：4元
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int cnt;
    cin >> cnt;
    cout << "总面值：" << cnt * 0.8 << "元" << endl;
    return 0;
}
```

</details>

---

##### 1.1.20 时间加法

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入小时、分钟，再加30分钟，输出新的小时分钟（简单版，暂不处理进位）。</div>

**样例**：

```text
输入：10 20，输出：10时50分
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int h, m;
    cin >> h >> m;
    m += 30;
    cout << h << "时" << m << "分" << endl;
    return 0;
}
```

</details>

---

### 1.2 条件分支（分支组）

#### ▸ 小类 A：数值比较与判断

##### 1.2.01 数字大小比较

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入两个数字，输出哪个数字更大。</div>

**样例**：

```text
输入：5 9，输出：9更大
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    double a,b;
    cin >> a >> b;
    if(a > b) cout << a << "更大" << endl;
    else if(b > a) cout << b << "更大" << endl;
    else cout << "两数相等" << endl;
    return 0;
}
```

</details>

---

##### 1.2.02 奇偶数判断器

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入整数，判断是奇数还是偶数。</div>

**样例**：

```text
输入：7，输出：奇数
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int x;
    cin >> x;
    if(x % 2 == 0) cout << "偶数" << endl;
    else cout << "奇数" << endl;
    return 0;
}
```

</details>

---

##### 1.2.03 闰年判断简易版

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入年份，能被4整除就是闰年。（先简化规则，后面再进阶）</div>

**样例**：

```text
输入：2024，输出：闰年
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int y;
    cin >> y;
    if(y % 4 == 0) cout << "闰年" << endl;
    else cout << "平年" << endl;
    return 0;
}
```

</details>

---

##### 1.2.04 三数找最大值

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入3个数字，找出最大的数字。</div>

**样例**：

```text
输入：12 45 27，输出：最大值=45
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int a,b,c;
    cin >> a >> b >> c;
    int maxv = a;
    if(b>maxv) maxv = b;
    if(c>maxv) maxv = c;
    cout << "最大值=" << maxv << endl;
    return 0;
}
```

</details>

---

##### 1.2.05 正数负数判断

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入数字，判断正数、负数或者等于0。</div>

**样例**：

```text
输入：-3.5 →负数
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    double x;
    cin >> x;
    if(x>0) cout << "正数";
    else if(x<0) cout << "负数";
    else cout << "等于0";
    return 0;
}
```

</details>

---

##### 1.2.06 三角形可行性

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入三边长度，如果任意两边之和大于第三边，输出可以构成三角形，否则不行。</div>

**样例**：

```text
输入：3 4 5 →可以构成三角形
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int a,b,c;
    cin >> a >> b >> c;
    if(a+b>c && a+c>b && b+c>a)
        cout << "可以构成三角形" << endl;
    else
        cout << "不能构成三角形" << endl;
    return 0;
}
```

</details>

---

##### 1.2.07 水仙花数单次判断

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入一个3位数，判断是否水仙花数（各位立方之和等于本身）。</div>

**样例**：

```text
输入：153 →是水仙花数
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int n;
    cin >> n;
    int a = n/100;
    int b = n/10%10;
    int c = n%10;
    if(a*a*a + b*b*b + c*c*c == n)
        cout << "是水仙花数";
    else
        cout << "不是水仙花数";
    return 0;
}
```

</details>

---

#### ▸ 小类 B：成绩与年龄分档

##### 1.2.08 成绩等级判断

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入考试分数。≥90输出A；8089输出B；7079输出C；60~69输出D；低于60输出E。</div>

**样例**：

```text
输入：85，输出：B
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int s;
    cin >> s;
    if(s >=90) cout << "A";
    else if(s >=80) cout << "B";
    else if(s >=70) cout << "C";
    else if(s >=60) cout << "D";
    else cout << "E";
    return 0;
}
```

</details>

---

##### 1.2.09 电影院票价

<div style="font-size:1.2em; line-height:1.7;">**题干**：年龄小于6岁免费；6~18岁半价；18岁以上全价40元。输入年龄，输出票价。</div>

**样例**：

```text
输入：10，输出：票价：20
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int age;
    cin >> age;
    double price;
    if(age <6) price=0;
    else if(age <=18) price=20;
    else price=40;
    cout << "票价：" << price << endl;
    return 0;
}
```

</details>

---

##### 1.2.10 是否及格

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入分数，≥60输出恭喜及格，否则输出需要继续努力。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int s;
    cin >> s;
    if(s>=60) cout << "恭喜及格";
    else cout << "需要继续努力";
    return 0;
}
```

</details>

---

##### 1.2.11 年龄段分类

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入年龄：小于12儿童；1218青少年；1860成年人；60以上老年人。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int age;
    cin >> age;
    if(age<12) cout << "儿童";
    else if(age <=18) cout << "青少年";
    else if(age <=60) cout << "成年人";
    else cout << "老年人";
    return 0;
}
```

</details>

---

#### ▸ 小类 C：计费与优惠规则

##### 1.2.12 打车计费

<div style="font-size:1.2em; line-height:1.7;">**题干**：起步价10元（3公里以内），超过3公里，每公里加收2元。输入里程，计算车费。</div>

**样例**：

```text
输入：5，输出：车费：14
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    double km;
    cin >> km;
    double fee;
    if(km <=3) fee =10;
    else fee = 10 + (km-3)*2;
    cout << "车费：" << fee << endl;
    return 0;
}
```

</details>

---

##### 1.2.13 水杯提醒

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入当前时间（小时），如果大于18点，提示“该喝水休息啦”。</div>

**样例**：

```text
输入：19，输出：该喝水休息啦
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int h;
    cin >> h;
    if(h>18) cout << "该喝水休息啦" << endl;
    else cout << "继续加油" << endl;
    return 0;
}
```

</details>

---

##### 1.2.14 超市满减

<div style="font-size:1.2em; line-height:1.7;">**题干**：满100减20。输入总金额，计算优惠之后价格。</div>

**样例**：

```text
输入：120 →优惠后价格：100
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    double total;
    cin >> total;
    if(total >=100) total -=20;
    cout << "优惠后价格：" << total << endl;
    return 0;
}
```

</details>

---

##### 1.2.15 快递运费

<div style="font-size:1.2em; line-height:1.7;">**题干**：重量≤1kg运费8元；超过1kg，每增加1kg加3元。输入重量，算运费。</div>

**样例**：

```text
输入：2.5 →运费：12.5
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    double w;
    cin >> w;
    double fee;
    if(w <=1) fee=8;
    else fee = 8 + (w-1)*3;
    cout << "运费：" << fee << endl;
    return 0;
}
```

</details>

---

##### 1.2.16 图书折扣

<div style="font-size:1.2em; line-height:1.7;">**题干**：买书，如果购买数量≥10本，打7折；否则9折。输入数量和单价，计算总价。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int n;
    double price;
    cin >> n >> price;
    double sum = n * price;
    if(n >=10) sum *=0.7;
    else sum *=0.9;
    cout << "总价：" << sum << endl;
    return 0;
}
```

</details>

---

##### 1.2.17 月份天数简易版

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入月份，输出这个月有多少天（只区分大月31，小月30，2月写28）。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int m;
    cin >> m;
    int day;
    if(m==1||m==3||m==5||m==7||m==8||m==10||m==12) day=31;
    else if(m==4||m==6||m==9||m==11) day=30;
    else day=28;
    cout << day << "天" << endl;
    return 0;
}
```

</details>

---

##### 1.2.18 限速判断

<div style="font-size:1.2em; line-height:1.7;">**题干**：道路限速60km/h，输入车速，超速提示“减速！”，否则提示正常。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    double v;
    cin >> v;
    if(v>60) cout << "减速！";
    else cout << "正常";
    return 0;
}
```

</details>

---

##### 1.2.19 优惠券选择

<div style="font-size:1.2em; line-height:1.7;">**题干**：商品总价，二选一：满100减30，或者直接8折。程序自动帮你算哪种更划算。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    double total;
    cin >> total;
    double opt1 = total >=100 ? total-30 : total;
    double opt2 = total * 0.8;
    if(opt1 < opt2) cout << "选满减，价格：" << opt1;
    else cout << "选8折，价格：" << opt2;
    return 0;
}
```

</details>

---

#### ▸ 小类 D：简单交互判断

##### 1.2.20 密码验证

<div style="font-size:1.2em; line-height:1.7;">**题干**：预设密码是1234，用户输入密码，正确提示解锁成功，错误提示密码错误。</div>

**样例**：

```text
输入：1234 →解锁成功；输入1111→密码错误
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int pwd;
    cin >> pwd;
    if(pwd == 1234) cout << "解锁成功" << endl;
    else cout << "密码错误" << endl;
    return 0;
}
```

</details>

---

##### 1.2.21 红绿灯判断

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入red/green/yellow字符串，输出对应的提示：红灯停，绿灯行，黄灯等一等。</div>

**样例**：

```text
输入：red →红灯停
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <string>
using namespace std;
int main()
{
    string s;
    cin >> s;
    if(s == "red") cout << "红灯停";
    else if(s == "green") cout << "绿灯行";
    else if(s == "yellow") cout << "黄灯等一等";
    return 0;
}
```

</details>

---

##### 1.2.22 BMI健康计算器

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入身高（米）体重（kg），计算BMI，输出偏瘦/正常/偏重。</div>

**样例**：

```text
输入：1.7 60 →BMI=20.7612 正常
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    double h,w;
    cin >> h >> w;
    double bmi = w/(h*h);
    cout << "BMI=" << bmi << " ";
    if(bmi <18.5) cout << "偏瘦";
    else if(bmi <24) cout << "正常";
    else cout << "偏重";
    return 0;
}
```

</details>

---

##### 1.2.23 猜数字1次版

<div style="font-size:1.2em; line-height:1.7;">**题干**：固定秘密数字6，用户输入数字，提示大了/小了/猜对。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int x;
    cin >> x;
    int secret =6;
    if(x>secret) cout << "大了";
    else if(x<secret) cout << "小了";
    else cout << "猜对！";
    return 0;
}
```

</details>

---

##### 1.2.24 石头剪刀布【单次】

<div style="font-size:1.2em; line-height:1.7;">**题干**：玩家输入1石头，2剪刀，3布。电脑固定出1石头，判断输赢。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int p;
    cin >> p;
    int com = 1;
    //1石头，2剪刀，3布
    if(p == com) cout << "平局";
    else if( (p==1 && com==2) || (p==2 && com==3) || (p==3 && com==1) )
        cout << "玩家赢";
    else cout << "电脑赢";
    return 0;
}
```

</details>

---

##### 1.2.25 留言过滤器

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入一句话，如果里面是bad，输出【敏感词】，否则正常输出文字。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <string>
using namespace std;
int main()
{
    string s;
    cin >> s;
    if(s == "bad") cout << "【敏感词】";
    else cout << s;
    return 0;
}
```

</details>

---

### 1.3 循环控制（循环组）

#### ▸ 小类 A：计数与累加

##### 1.3.01 1到N打印器

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入N，从1开始，依次在屏幕输出1，2，3……直到N。</div>

**样例**：

```text
输入：5，输出：1 2 3 4 5
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int n;
    cin >> n;
    for(int i=1;i<=n;i++)
    {
        cout << i << " ";
    }
    return 0;
}
```

</details>

---

##### 1.3.02 倒数倒计时

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入数字N，从N开始倒数到1，最后输出“发射！”。例：输入5 →5,4,3,2,1，发射！</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int n;
    cin >> n;
    for(int i=n;i>=1;i--)
    {
        cout << i << endl;
    }
    cout << "发射！" << endl;
    return 0;
}
```

</details>

---

##### 1.3.03 1~N求和

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入N，计算1+2+3+…+N的总和。</div>

**样例**：

```text
输入：10，输出：55
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int n;
    cin >> n;
    int sum=0;
    for(int i=1;i<=n;i++) sum +=i;
    cout << sum << endl;
    return 0;
}
```

</details>

---

##### 1.3.04 偶数打印器

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入N，输出1~N里面所有偶数。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int n;
    cin >> n;
    for(int i=2;i<=n;i+=2)
        cout << i << " ";
    return 0;
}
```

</details>

---

##### 1.3.05 奇数求和

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入N，求1到N所有奇数加起来的总和。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int n,sum=0;
    cin >> n;
    for(int i=1;i<=n;i+=2) sum +=i;
    cout << sum << endl;
    return 0;
}
```

</details>

---

##### 1.3.06 累加小游戏

<div style="font-size:1.2em; line-height:1.7;">**题干**：不断输入数字，直到输入0停止，计算所有数字总和。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int x,sum=0;
    while(cin >> x)
    {
        if(x ==0) break;
        sum +=x;
    }
    cout << "总和=" << sum << endl;
    return 0;
}
```

</details>

---

##### 1.3.07 统计倍数个数

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入N，统计1~N里面，3的倍数一共有多少个。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int n,cnt=0;
    cin >> n;
    for(int i=1;i<=n;i++)
    {
        if(i%3 ==0) cnt++;
    }
    cout << cnt << endl;
    return 0;
}
```

</details>

---

##### 1.3.08 求阶乘

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入n，计算 n! = 1×2×3…×n。例5! =120。</div>

**样例**：

```text
输入：5 →120
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int n;
    cin >> n;
    long long ans=1;
    for(int i=2;i<=n;i++) ans *=i;
    cout << ans << endl;
    return 0;
}
```

</details>

---

##### 1.3.09 连续整数乘积

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入a,b，计算a到b所有整数相乘。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int a,b;
    cin >> a >> b;
    long long p=1;
    for(int i=a;i<=b;i++) p *=i;
    cout << p << endl;
    return 0;
}
```

</details>

---

##### 1.3.10 数字各位求和

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入数字123，各位相加1+2+3=6。</div>

**样例**：

```text
输入：123 →6
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int n,sum=0;
    cin >> n;
    while(n>0)
    {
        sum += n%10;
        n /=10;
    }
    cout << sum << endl;
    return 0;
}
```

</details>

---

##### 1.3.11 最小公倍数

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入两个数字，计算最小公倍数。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int a,b;
    cin >> a >> b;
    int g=1;
    for(int i=1;i<=a&&i<=b;i++)
        if(a%i==0 && b%i==0) g=i;
    int lcm = a / g * b;
    cout << lcm << endl;
    return 0;
}
```

</details>

---

##### 1.3.12 累加平均值

<div style="font-size:1.2em; line-height:1.7;">**题干**：持续输入数字，输入-1结束，计算输入数字的平均值。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int x,sum=0,cnt=0;
    while(cin >>x)
    {
        if(x == -1) break;
        sum +=x; cnt++;
    }
    if(cnt>0) cout << 1.0*sum/cnt;
    return 0;
}
```

</details>

---

#### ▸ 小类 B：图形图案打印

##### 1.3.13 打印5行星号矩形

<div style="font-size:1.2em; line-height:1.7;">**题干**：循环输出5行，每行8个*。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    for(int i=1;i<=5;i++)
    {
        for(int j=1;j<=8;j++)
            cout << "*";
        cout << endl;
    }
    return 0;
}
```

</details>

---

##### 1.3.14 直角三角形星图

<div style="font-size:1.2em; line-height:1.7;">**题干**：输出： * ** *** **** *****</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    for(int i=1;i<=5;i++)
    {
        for(int j=1;j<=i;j++)
            cout << "*";
        cout << endl;
    }
    return 0;
}
```

</details>

---

##### 1.3.15 乘法口诀表【一行版】

<div style="font-size:1.2em; line-height:1.7;">**题干**：输出1*1=1 1*2=2 ……1*9=9。后续可以扩展完整九九表。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    for(int j=1;j<=9;j++)
    {
        cout << "1*" << j << "=" << 1*j << " ";
    }
    return 0;
}
```

</details>

---

##### 1.3.16 星星倒三角

<div style="font-size:1.2em; line-height:1.7;">**题干**：***** **** *** ** *</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    for(int i=5;i>=1;i--)
    {
        for(int j=1;j<=i;j++) cout << "*";
        cout << endl;
    }
    return 0;
}
```

</details>

---

##### 1.3.17 九九乘法表完整版

<div style="font-size:1.2em; line-height:1.7;">**题干**：双层循环打印完整九九乘法表。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    for(int i=1;i<=9;i++)
    {
        for(int j=1;j<=i;j++)
        {
            cout << j << "*" << i << "=" << i*j << " ";
        }
        cout << endl;
    }
    return 0;
}
```

</details>

---

##### 1.3.18 菱形星号图案

<div style="font-size:1.2em; line-height:1.7;">**题干**：用循环打印菱形星星图案。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    //上半
    for(int i=1;i<=3;i++)
    {
        for(int k=1;k<=3-i;k++) cout << " ";
        for(int j=1;j<=2*i-1;j++) cout << "*";
        cout << endl;
    }
    //下半
    for(int i=2;i>=1;i--)
    {
        for(int k=1;k<=3-i;k++) cout << " ";
        for(int j=1;j<=2*i-1;j++) cout << "*";
        cout << endl;
    }
    return 0;
}
```

</details>

---

##### 1.3.19 沙漏星图

<div style="font-size:1.2em; line-height:1.7;">**题干**：循环打印沙漏形状的星号图案。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    //上半
    for(int i=3;i>=1;i--)
    {
        for(int k=1;k<=3-i;k++) cout << " ";
        for(int j=1;j<=2*i-1;j++) cout << "*";
        cout << endl;
    }
    //下半
    for(int i=2;i<=3;i++)
    {
        for(int k=1;k<=3-i;k++) cout << " ";
        for(int j=1;j<=2*i-1;j++) cout << "*";
        cout << endl;
    }
    return 0;
}
```

</details>

---

#### ▸ 小类 C：数字处理与数论

##### 1.3.20 正序输出数字各位

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入一个三位数，依次打印百位、十位、个位。例如：123 →1，2，3。</div>

**样例**：

```text
输入：123 →1,2,3
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int n;
    cin >> n;
    int a = n/100;
    int b = n/10%10;
    int c = n%10;
    cout << a << "," << b << "," << c;
    return 0;
}
```

</details>

---

##### 1.3.21 倒序拆数字

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入123，输出321。</div>

**样例**：

```text
输入：123 →321
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int n;
    cin >> n;
    int res=0;
    while(n>0)
    {
        res = res*10 + n%10;
        n /=10;
    }
    cout << res << endl;
    return 0;
}
```

</details>

---

##### 1.3.22 质数判断

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入数字，判断这个数是不是质数（只能被1和自己整除）。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int n;
    cin >> n;
    bool ok = true;
    if(n<=1) ok=false;
    for(int i=2;i*i <=n;i++)
    {
        if(n%i ==0) {ok=false; break;}
    }
    if(ok) cout << "质数";
    else cout << "不是质数";
    return 0;
}
```

</details>

---

##### 1.3.23 找公约数

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入两个整数，找出它们所有的公约数。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int a,b;
    cin >> a >> b;
    for(int i=1;i<=a && i<=b;i++)
    {
        if(a%i ==0 && b%i ==0) cout << i << " ";
    }
    return 0;
}
```

</details>

---

##### 1.3.24 完全数判断

<div style="font-size:1.2em; line-height:1.7;">**题干**：一个数等于它所有真因数之和，例如6=1+2+3，叫做完全数。输入数字判断。</div>

**样例**：

```text
输入：6 →完全数
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int n,sum=0;
    cin >> n;
    for(int i=1;i<n;i++)
    {
        if(n%i ==0) sum +=i;
    }
    if(sum == n) cout << "完全数";
    else cout << "不是完全数";
    return 0;
}
```

</details>

---

##### 1.3.25 大小写转换器简易版

<div style="font-size:1.2em; line-height:1.7;">**题干**：循环输入字母，大写转小写，输入0结束。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    char c;
    while(cin >> c)
    {
        if(c == '0') break;
        if(c >= 'A' && c <= 'Z') c +=32;
        else if(c >= 'a' && c <= 'z') c -=32;
        cout << c << endl;
    }
    return 0;
}
```

</details>

---

##### 1.3.26 百钱买百鸡

<div style="font-size:1.2em; line-height:1.7;">**题干**：经典趣味数学题。公鸡5元一只，母鸡3元一只，小鸡1元3只。100元买100只鸡，找出所有方案。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    for(int g=0;g<=20;g++)
    {
        for(int m=0;m<=33;m++)
        {
            int x = 100 - g - m;
            if(x >=0 && 5*g +3*m + x/3 ==100 && x%3==0)
            {
                cout << "公鸡"<<g<<"母鸡"<<m<<"小鸡"<<x<<endl;
            }
        }
    }
    return 0;
}
```

</details>

---

##### 1.3.27 寻找100以内所有质数

<div style="font-size:1.2em; line-height:1.7;">**题干**：循环找出1~100全部质数并且打印。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    for(int i=2;i<=100;i++)
    {
        bool ok=true;
        for(int j=2;j*j<=i;j++)
        {
            if(i%j ==0) {ok=false;break;}
        }
        if(ok) cout << i << " ";
    }
    return 0;
}
```

</details>

---

##### 1.3.28 数字回文判断

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入数字，判断正向读和反向读是不是一样（121是回文，123不是）。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int n,tmp,rev=0;
    cin >> n;
    tmp = n;
    while(tmp>0)
    {
        rev = rev*10 + tmp%10;
        tmp /=10;
    }
    if(rev == n) cout << "回文数";
    else cout << "不是回文数";
    return 0;
}
```

</details>

---

##### 1.3.29 约数总和

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入数字，算出它全部约数的总和。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int n,sum=0;
    cin >> n;
    for(int i=1;i<=n;i++)
    {
        if(n%i ==0) sum +=i;
    }
    cout << sum << endl;
    return 0;
}
```

</details>

---

#### ▸ 小类 D：循环模拟与小游戏

##### 1.3.30 猜数字循环版

<div style="font-size:1.2em; line-height:1.7;">**题干**：秘密数字固定，玩家可以反复猜，直到猜对，每次提示大/小。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int x;
    int secret = 28;
    while(cin >> x)
    {
        if(x>secret) cout << "大了" << endl;
        else if(x<secret) cout << "小了" << endl;
        else {cout << "猜对！"; break;}
    }
    return 0;
}
```

</details>

---

##### 1.3.31 重复文字输出

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入文字和次数，重复打印这段文字指定次数。例如输入hello、3，输出3行hello。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <string>
using namespace std;
int main()
{
    string s;
    int t;
    cin >> s >> t;
    for(int i=1;i<=t;i++) cout << s << endl;
    return 0;
}
```

</details>

---

##### 1.3.32 密码重试3次

<div style="font-size:1.2em; line-height:1.7;">**题干**：最多3次输入密码机会，输入正确直接成功；3次全部错误锁定。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int pwd;
    for(int i=1;i<=3;i++)
    {
        cin >> pwd;
        if(pwd ==1234)
        {
            cout << "成功";
            return 0;
        }
        cout << "密码错误" << endl;
    }
    cout << "锁定";
    return 0;
}
```

</details>

---

##### 1.3.33 斐波那契数列

<div style="font-size:1.2em; line-height:1.7;">**题干**：输出前10项斐波那契：1,1,2,3,5,8……</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int a=1,b=1;
    cout << a << " " << b << " ";
    for(int i=3;i<=10;i++)
    {
        int c = a+b;
        cout << c << " ";
        a = b; b = c;
    }
    return 0;
}
```

</details>

---

##### 1.3.34 统计字符数量

<div style="font-size:1.2em; line-height:1.7;">**题干**：连续输入字母，直到输入#结束，统计一共输入多少个字符。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    char ch;
    int cnt=0;
    while(cin >> ch)
    {
        if(ch == '#') break;
        cnt++;
    }
    cout << cnt << endl;
    return 0;
}
```

</details>

---

##### 1.3.35 青蛙爬井

<div style="font-size:1.2em; line-height:1.7;">**题干**：井深10米，白天向上爬3米，晚上下滑2米。计算第几天爬出井口。模拟循环计算。</div>

**样例**：

```text
输出：8
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int deep = 10;
    int h=0,day=0;
    while(true)
    {
        day++;
        h +=3;
        if(h >= deep) break;
        h -=2;
    }
    cout << day << endl;
    return 0;
}
```

</details>

---

### 1.4 随机数与趣味游戏（趣味进阶组）

#### ▸ 小类 A：随机数与概率模拟

##### 1.4.01 骰子模拟器

<div style="font-size:1.2em; line-height:1.7;">**题干**：点击运行模拟掷骰子，随机输出1~6点数，可以连续掷多次。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <cstdlib>
#include <ctime>
using namespace std;
int main()
{
    srand((unsigned)time(NULL));
    cout << rand()%6 +1 << endl;
    return 0;
}
```

</details>

---

##### 1.4.02 抽奖小程序

<div style="font-size:1.2em; line-height:1.7;">**题干**：奖项：一等奖、二等奖、三等奖、谢谢参与。随机抽取。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <cstdlib>
#include <ctime>
using namespace std;
int main()
{
    srand((unsigned)time(NULL));
    int r = rand()%4;
    if(r==0) cout << "一等奖";
    else if(r==1) cout << "二等奖";
    else if(r==2) cout << "三等奖";
    else cout << "谢谢参与";
    return 0;
}
```

</details>

---

##### 1.4.03 幸运大转盘简易版

<div style="font-size:1.2em; line-height:1.7;">**题干**：随机输出：恭喜获得贴纸、获得文具、谢谢参与。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <cstdlib>
#include <ctime>
using namespace std;
int main()
{
    srand((unsigned)time(NULL));
    int r = rand()%3;
    if(r==0) cout << "恭喜获得贴纸";
    else if(r==1) cout << "获得文具";
    else cout << "谢谢参与";
    return 0;
}
```

</details>

---

##### 1.4.04 老虎机简易小游戏

<div style="font-size:1.2em; line-height:1.7;">**题干**：随机生成3个数字，如果三个数字相同，中奖。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <cstdlib>
#include <ctime>
using namespace std;
int main()
{
    srand((unsigned)time(NULL));
    int a = rand()%10;
    int b = rand()%10;
    int c = rand()%10;
    cout << a << " " << b << " " << c << endl;
    if(a == b && b == c) cout << "中奖！";
    else cout << "未中奖";
    return 0;
}
```

</details>

---

##### 1.4.05 掷硬币模拟器

<div style="font-size:1.2em; line-height:1.7;">**题干**：随机正反面，模拟抛硬币N次，统计正面反面出现次数。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <cstdlib>
#include <ctime>
using namespace std;
int main()
{
    srand((unsigned)time(NULL));
    int n;
    cin >> n;
    int head=0,tail=0;
    for(int i=1;i<=n;i++)
    {
        int r = rand()%2;
        if(r==0) head++;
        else tail++;
    }
    cout << "正面：" << head << " 反面：" << tail << endl;
    return 0;
}
```

</details>

---

##### 1.4.06 扑克牌抽牌模拟器

<div style="font-size:1.2em; line-height:1.7;">**题干**：随机抽取一张牌，输出花色与点数。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <cstdlib>
#include <ctime>
using namespace std;
int main()
{
    srand((unsigned)time(NULL));
    int suit = rand()%4;
    int num = rand()%13 +1;
    string s;
    if(suit ==0) s="黑桃";
    else if(suit ==1) s="红桃";
    else if(suit ==2) s="梅花";
    else s="方块";
    cout << s << num;
    return 0;
}
```

</details>

---

#### ▸ 小类 B：对战互动小游戏

##### 1.4.07 随机猜数字游戏

<div style="font-size:1.2em; line-height:1.7;">**题干**：程序每次运行随机生成1~100秘密数字，玩家反复猜，提示大小，记录猜测次数。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <cstdlib>
#include <ctime>
using namespace std;
int main()
{
    srand((unsigned)time(NULL));
    int secret = rand()%100 +1;
    int x,cnt=0;
    cout << "猜1~100数字" << endl;
    while(cin >> x)
    {
        cnt++;
        if(x>secret) cout << "大了" << endl;
        else if(x<secret) cout << "小了" << endl;
        else {cout << "猜对，一共猜了" << cnt << "次"; break;}
    }
    return 0;
}
```

</details>

---

##### 1.4.08 石头剪刀布对战电脑

<div style="font-size:1.2em; line-height:1.7;">**题干**：电脑每次随机出拳，玩家输入选择，一局一局对战，统计输赢次数。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <cstdlib>
#include <ctime>
using namespace std;
int main()
{
    srand((unsigned)time(NULL));
    int p;
    cout << "1石头，2剪刀，3布" << endl;
    while(cin >> p)
    {
        int com = rand()%3 +1;
        cout << "电脑出：" << com << endl;
        if(p == com) cout << "平局\n";
        else if( (p==1&&com==2)||(p==2&&com==3)||(p==3&&com==1) )
            cout << "玩家赢\n";
        else cout << "电脑赢\n";
    }
    return 0;
}
```

</details>

---

##### 1.4.09 寻宝小游戏

<div style="font-size:1.2em; line-height:1.7;">**题干**：地图0~10坐标，宝藏随机藏在一个坐标，玩家输入坐标寻找，提示离宝藏远/近。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <cstdlib>
#include <ctime>
using namespace std;
int main()
{
    srand((unsigned)time(NULL));
    int treasure = rand()%11;
    int x;
    cout << "宝藏在0~10之间，输入坐标寻找" << endl;
    while(cin >>x)
    {
        if(x>treasure) cout << "太远了，往小一点" << endl;
        else if(x < treasure) cout << "往大一点" << endl;
        else {cout << "找到宝藏！";break;}
    }
    return 0;
}
```

</details>

---

##### 1.4.10 怪物战斗小游戏

<div style="font-size:1.2em; line-height:1.7;">**题干**：玩家血量、怪物血量。每次攻击随机扣血，直到一方血量归零。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <cstdlib>
#include <ctime>
using namespace std;
int main()
{
    srand((unsigned)time(NULL));
    int player = 100;
    int monster = 80;
    while(player>0 && monster>0)
    {
        int p_atk = rand()%10 +5;
        monster -= p_atk;
        cout << "你攻击怪物，扣" << p_atk << "血，怪物剩余" << monster << endl;
        if(monster <=0) break;
        int m_atk = rand()%8 +3;
        player -= m_atk;
        cout << "怪物攻击你，扣" << m_atk << "血，你剩余" << player << endl;
    }
    if(player>0) cout << "胜利";
    else cout << "失败";
    return 0;
}
```

</details>

---

#### ▸ 小类 C：口算练习工具

##### 1.4.11 口算出题器（加法）

<div style="font-size:1.2em; line-height:1.7;">**题干**：程序随机出2道100以内加法题，玩家输入答案，自动判断对错，统计得分。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <cstdlib>
#include <ctime>
using namespace std;
int main()
{
    srand((unsigned)time(NULL));
    int score=0;
    for(int i=1;i<=2;i++)
    {
        int a=rand()%100;
        int b=rand()%100;
        int ans;
        cout << a << "+" << b << "=";
        cin >> ans;
        if(ans == a+b) {cout << "对！";score++;}
        else cout << "错，答案=" << a+b;
    }
    cout << "\n得分：" << score << "/2";
    return 0;
}
```

</details>

---

##### 1.4.12 口算出题器（加减混合）

<div style="font-size:1.2em; line-height:1.7;">**题干**：随机生成加法、减法口算题目，自动判分。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <cstdlib>
#include <ctime>
using namespace std;
int main()
{
    srand((unsigned)time(NULL));
    int score=0;
    for(int i=1;i<=3;i++)
    {
        int a=rand()%100;
        int b=rand()%100;
        int op = rand()%2;
        int ans;
        if(op ==0)
        {
            cout << a << "+" << b << "=";
            cin >> ans;
            if(ans == a+b) score++;
        }
        else
        {
            cout << a << "-" << b << "=";
            cin >> ans;
            if(ans == a-b) score++;
        }
    }
    cout << "得分：" << score << endl;
    return 0;
}
```

</details>

---

#### ▸ 小类 D：实用小工具

##### 1.4.13 倒计时计时器

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入秒数，每秒减一，到0提示时间到。</div>

**样例**：

```text
注：Linux 环境不能用 Sleep，换成 usleep。
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <windows.h>
using namespace std;
int main()
{
    int t;
    cin >> t;
    for(int i=t;i>0;i--)
    {
        cout << i << endl;
        Sleep(1000);
    }
    cout << "时间到！";
    return 0;
}
```

</details>

---

##### 1.4.14 单词默写小工具

<div style="font-size:1.2em; line-height:1.7;">**题干**：内置3组单词，程序显示中文，玩家输入英文，判断是否正确。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <string>
#include <cstdlib>
#include <ctime>
using namespace std;
int main()
{
    srand((unsigned)time(NULL));
    string en[3] = {"apple","cat","book"};
    string cn[3] = {"苹果","猫","书"};
    int idx = rand()%3;
    string ans;
    cout << cn[idx] << " 的英文：";
    cin >> ans;
    if(ans == en[idx]) cout << "正确";
    else cout << "错误，答案：" << en[idx];
    return 0;
}
```

</details>

---

##### 1.4.15 BMI记录器

<div style="font-size:1.2em; line-height:1.7;">**题干**：多次输入身高体重，循环记录多个人BMI结果。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    double h,w;
    while(cin >> h >> w)
    {
        double bmi = w/(h*h);
        cout << "BMI=" << bmi << endl;
    }
    return 0;
}
```

</details>

---

##### 1.4.16 成绩录入统计

<div style="font-size:1.2em; line-height:1.7;">**题干**：循环录入多名学生分数，最后算出最高分、最低分、平均分。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int x,maxs=0,mins=1000,sum=0,cnt=0;
    while(cin >> x)
    {
        if(x == -1) break;
        cnt++;
        sum +=x;
        if(x>maxs) maxs=x;
        if(x<mins) mins=x;
    }
    cout << "最高分：" << maxs << "最低分：" << mins << "平均分：" << 1.0*sum/cnt;
    return 0;
}
```

</details>

---

##### 1.4.17 密码生成器

<div style="font-size:1.2em; line-height:1.7;">**题干**：随机生成指定长度的数字密码。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <cstdlib>
#include <ctime>
using namespace std;
int main()
{
    srand((unsigned)time(NULL));
    int len;
    cin >> len;
    for(int i=1;i<=len;i++)
    {
        cout << rand()%10;
    }
    return 0;
}
```

</details>

---

##### 1.4.18 迷宫文字版小游戏

<div style="font-size:1.2em; line-height:1.7;">**题干**：文字菜单，上下移动，碰到出口获胜。简化文字交互，不用图形。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int x=1,y=1;
    char op;
    cout << "w上 s下 a左 d右，到达(3,3)获胜" << endl;
    while(cin >> op)
    {
        if(op == 'w') y++;
        if(op == 's') y--;
        if(op == 'a') x--;
        if(op == 'd') x++;
        cout << "当前坐标：" << x << "," << y << endl;
        if(x==3 && y==3) {cout << "到达出口！";break;}
    }
    return 0;
}
```

</details>

---

##### 1.4.19 时间管理器

<div style="font-size:1.2em; line-height:1.7;">**题干**：循环提醒任务，输入待办事项，添加多条待办。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <string>
using namespace std;
int main()
{
    string todo;
    cout << "输入待办，输入end结束" << endl;
    while(cin >> todo)
    {
        if(todo == "end") break;
        cout << "已添加：" << todo << endl;
    }
    cout << "任务录入完成";
    return 0;
}
```

</details>

---

##### 1.4.20 综合大挑战

<div style="font-size:1.2em; line-height:1.7;">**题干**：银行存款复利计算器：输入本金、年利率、存放年数，计算每年复利后的资金，逐年打印资金变化。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    double money,rate;
    int year;
    cin >> money >> rate >> year;
    for(int i=1;i<=year;i++)
    {
        money = money * (1+rate);
        cout << "第" << i << "年：" << money << endl;
    }
    return 0;
}
```

</details>

---

## 第2类 · 进阶提高 ｜ 第二套 · C++进阶趣味100题

> 难度：★★☆☆☆

### 2.1 函数与字符串（函数与字符串专题）

#### ▸ 小类 A：字符串基础操作

##### 2.1.01 字符串长度函数

<div style="font-size:1.2em; line-height:1.7;">**题干**：自己写一个函数my_len，不使用.size()，计算输入字符串的字符长度。</div>

**样例**：

```text
输入hello，输出5
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <string>
using namespace std;
int main()
{
    string s;
    cin >> s;
    cout << s.size() << endl;
    return 0;
}
```

</details>

---

##### 2.1.02 字符串反转函数

<div style="font-size:1.2em; line-height:1.7;">**题干**：写函数接收 string，返回反转后的字符串。输入abc123返回321cba。</div>

**样例**：

```text
输入abcd，输出dcba
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <string>
using namespace std;
int main()
{
    string s;
    cin >> s;
    string t;
    for(int i = s.size()-1; i>=0; i--)
        t += s[i];
    cout << t << endl;
    return 0;
}
```

</details>

---

##### 2.1.03 大小写互换工具

<div style="font-size:1.2em; line-height:1.7;">**题干**：函数把字符串里大写变小写、小写变大写，数字符号不变。</div>

**样例**：

```text
输入AbC，输出aBc
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <string>
using namespace std;
int main()
{
    string s;
    cin >> s;
    for(int i=0;i<s.size();i++)
    {
        if(s[i] >= 'A' && s[i] <= 'Z')
            s[i] +=32;
        else if(s[i] >= 'a' && s[i] <= 'z')
            s[i] -=32;
    }
    cout << s << endl;
    return 0;
}
```

</details>

---

##### 2.1.04 回文字符串判断

<div style="font-size:1.2em; line-height:1.7;">**题干**：函数判断字符串是否回文（忽略空格，区分大小写）。扩展可选：忽略大小写。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <string>
using namespace std;
int main()
{
    string s;
    cin >> s;
    bool ok = true;
    int len = s.size();
    for(int i=0;i<len/2;i++)
    {
        if(s[i] != s[len-1-i])
        {
            ok = false; break;
        }
    }
    if(ok) cout << "回文串";
    else cout << "不是回文串";
    return 0;
}
```

</details>

---

##### 2.1.05 去除空格

<div style="font-size:1.2em; line-height:1.7;">**题干**：编写函数删除字符串里面全部空格。</div>

**样例**：

```text
注意：getline 读取整行，前面不要用 cin 残留换行。
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <string>
using namespace std;
int main()
{
    string s, res;
    getline(cin, s);
    for(auto ch : s)
    {
        if(ch != ' ') res += ch;
    }
    cout << res << endl;
    return 0;
}
```

</details>

---

#### ▸ 小类 B：统计与查找

##### 2.1.06 单词计数

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入一行英文句子，统计里面有多少个单词（单词以空格分隔）。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <string>
using namespace std;
int main()
{
    string s;
    getline(cin,s);
    string tmp;
    for(auto ch : s)
    {
        if(ch == ' ')
        {
            if(tmp != "") cout << tmp << endl;
            tmp = "";
        }
        else tmp += ch;
    }
    if(tmp != "") cout << tmp << endl;
    return 0;
}
```

</details>

---

##### 2.1.07 查找子串位置

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入主字符串和目标子串，输出子串第一次出现的下标；找不到输出 - 1。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <string>
using namespace std;
int main()
{
    string a,b;
    cin >> a >> b;
    if(a.find(b) != string::npos)
        cout << "包含子串";
    else cout << "不包含";
    return 0;
}
```

</details>

---

##### 2.1.08 字符统计器

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入一段文字，统计大写字母、小写字母、数字、其他符号各有多少个。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <string>
using namespace std;
int main()
{
    string a,b;
    cin >> a >> b;
    if(a > b) cout << a << "更大";
    else if(a < b) cout << b << "更大";
    else cout << "相等";
    return 0;
}
```

</details>

---

##### 2.1.09 提取数字

<div style="font-size:1.2em; line-height:1.7;">**题干**：从混合文字字符串里，把所有数字字符提取出来组成新字符串。例如a1b2c3得到123。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <string>
using namespace std;
int main()
{
    string s;
    cin >> s;
    int cnt=0;
    for(auto ch : s)
    {
        if(ch >= '0' && ch <= '9') cnt++;
    }
    cout << cnt << endl;
    return 0;
}
```

</details>

---

#### ▸ 小类 C：字符串变换

##### 2.1.10 字符串替换

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入原文、旧词、新词，把原文中所有旧词替换成新词。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <string>
using namespace std;
int main()
{
    string s;
    cin >> s;
    for(int i=0;i<s.size();i++)
    {
        if(s[i] == 'a') s[i] = '*';
    }
    cout << s << endl;
    return 0;
}
```

</details>

---

##### 2.1.11 首字母大写

<div style="font-size:1.2em; line-height:1.7;">**题干**：一句话每个单词首字母改成大写，其余小写。例：hello world → Hello World。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <string>
using namespace std;
int main()
{
    string s;
    getline(cin, s);            // 读入整行
    bool newWord = true;        // 是否在单词开头
    for (int i = 0; i < s.size(); i++)
    {
        if (s[i] == ' ')        // 空格后面是新单词
        {
            newWord = true;
            cout << ' ';
        }
        else
        {
            if (newWord && s[i] >= 'a' && s[i] <= 'z')
                s[i] = s[i] - 'a' + 'A';        // 首字母大写
            if (!newWord && s[i] >= 'A' && s[i] <= 'Z')
                s[i] = s[i] - 'A' + 'a';        // 其余字母小写
            newWord = false;
            cout << s[i];
        }
    }
    return 0;
}
```

</details>

---

##### 2.1.12 分割字符串

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入一行以逗号分隔的数据，把每一段拆分存入 vector<string>。如苹果,香蕉,橙子拆分到数组。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <vector>
#include <string>
using namespace std;
int main()
{
    string s, word = "";
    getline(cin, s);
    vector<string> v;
    for (int i = 0; i < s.size(); i++)
    {
        if (s[i] == ',')        // 逗号分隔
        {
            v.push_back(word);
            word = "";
        }
        else
            word += s[i];
    }
    v.push_back(word);          // 最后一段
    for (int i = 0; i < v.size(); i++)
        cout << v[i] << endl;
    return 0;
}
```

</details>

---

##### 2.1.13 单词反转句子

<div style="font-size:1.2em; line-height:1.7;">**题干**：句子整体不反转，单词顺序颠倒。I love cpp → cpp love I。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <string>
using namespace std;
int main()
{
    string s, words[100];
    int cnt = 0;
    getline(cin, s);
    string w = "";
    for (int i = 0; i < s.size(); i++)
    {
        if (s[i] == ' ')
        {
            if (w != "") { words[cnt++] = w; w = ""; }
        }
        else
            w += s[i];
    }
    if (w != "") words[cnt++] = w;
    for (int i = cnt - 1; i >= 0; i--)     // 单词倒序输出
    {
        if (i < cnt - 1) cout << ' ';
        cout << words[i];
    }
    return 0;
}
```

</details>

---

##### 2.1.14 字符去重

<div style="font-size:1.2em; line-height:1.7;">**题干**：字符串中连续重复字符只保留 1 个。aaabbbcc → abc。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <string>
using namespace std;
int main()
{
    string s, ans = "";
    getline(cin, s);
    for (int i = 0; i < s.size(); i++)
        if (i == 0 || s[i] != s[i-1])      // 与前一个不同才保留
            ans += s[i];
    cout << ans;
    return 0;
}
```

</details>

---

##### 2.1.15 拼音首字母缩写简易版

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入中文词语拼音（ni hao）提取首字母NH。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <string>
#include <cctype>
using namespace std;
int main()
{
    string s;
    getline(cin, s);
    bool newWord = true;
    for (int i = 0; i < s.size(); i++)
    {
        if (s[i] == ' ')
            newWord = true;
        else
        {
            if (newWord)
                cout << (char)toupper(s[i]);    // 单词首字母转大写
            newWord = false;
        }
    }
    return 0;
}
```

</details>

---

#### ▸ 小类 D：加密与校验

##### 2.1.16 密码强度检测

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入密码，规则：≥8 位、包含大写、小写、数字。输出弱 / 中等 / 强。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <string>
using namespace std;
int main()
{
    string s;
    cin >> s;
    bool hasUpper=false, hasLower=false, hasDigit=false;
    for(auto ch : s)
    {
        if(ch>='A'&&ch<='Z') hasUpper=true;
        else if(ch>='a'&&ch<='z') hasLower=true;
        else if(ch>='0'&&ch<='9') hasDigit=true;
    }
    if(s.size()>=6 && hasUpper && hasLower && hasDigit)
        cout << "强密码";
    else cout << "弱密码";
    return 0;
}
```

</details>

---

##### 2.1.17 字符串加密简易凯撒密码

<div style="font-size:1.2em; line-height:1.7;">**题干**：字母向后偏移 3 位（A→D，z→c），非字母不变。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <string>
using namespace std;
int main()
{
    string s;
    getline(cin, s);
    for (int i = 0; i < s.size(); i++)
    {
        char c = s[i];
        if (c >= 'a' && c <= 'z')
            c = 'a' + (c - 'a' + 3) % 26;      // 小写后移3位
        else if (c >= 'A' && c <= 'Z')
            c = 'A' + (c - 'A' + 3) % 26;      // 大写后移3位
        cout << c;                             // 非字母不变
    }
    return 0;
}
```

</details>

---

##### 2.1.18 凯撒解密

<div style="font-size:1.2em; line-height:1.7;">**题干**：对凯撒加密后的文字进行解密。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <string>
using namespace std;
int main()
{
    string s;
    getline(cin, s);
    for (int i = 0; i < s.size(); i++)
    {
        char c = s[i];
        if (c >= 'a' && c <= 'z')
            c = 'a' + (c - 'a' + 23) % 26;     // 前移3位
        else if (c >= 'A' && c <= 'Z')
            c = 'A' + (c - 'A' + 23) % 26;
        cout << c;
    }
    return 0;
}
```

</details>

---

##### 2.1.19 括号匹配检查

<div style="font-size:1.2em; line-height:1.7;">**题干**：只检查()，遍历字符串，判断括号是否成对、合法。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <string>
using namespace std;
int main()
{
    string s;
    cin >> s;
    int cnt = 0;                // 未配对的左括号数量
    bool ok = true;
    for (int i = 0; i < s.size(); i++)
    {
        if (s[i] == '(') cnt++;
        else if (s[i] == ')')
        {
            cnt--;
            if (cnt < 0) { ok = false; break; }   // 右括号多了
        }
    }
    if (cnt != 0) ok = false;   // 左括号没配完
    cout << (ok ? "合法" : "不合法");
    return 0;
}
```

</details>

---

##### 2.1.20 随机字符串生成器

<div style="font-size:1.2em; line-height:1.7;">**题干**：自定义长度，随机生成由大小写字母 + 数字组成的字符串。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <string>
#include <cstdlib>
#include <ctime>
using namespace std;
int main()
{
    srand(time(0));
    int n;
    cout << "输入长度: ";
    cin >> n;
    string chars = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789";
    for (int i = 0; i < n; i++)
        cout << chars[rand() % chars.size()];
    return 0;
}
```

</details>

---

### 2.2 数组与vector（数组与vector专题）

#### ▸ 小类 A：数组基础操作

##### 2.2.01 数组最大值最小值函数

<div style="font-size:1.2em; line-height:1.7;">**题干**：写函数接收 vector<int>，返回最大值和最小值。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <vector>
using namespace std;
int main()
{
    int n; cin >> n;
    vector<int> v(n);
    for(int i=0;i<n;i++) cin >> v[i];
    int maxv = v[0];
    for(auto x:v) if(x>maxv) maxv=x;
    cout << maxv << endl;
    return 0;
}
```

</details>

---

##### 2.2.02 数组求和与平均值

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入一组数字存入 vector，计算总和、平均值。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <vector>
using namespace std;
int main()
{
    int n; cin >> n;
    vector<int> v(n);
    int sum=0;
    for(int i=0;i<n;i++){cin>>v[i];sum+=v[i];}
    cout << sum << endl;
    return 0;
}
```

</details>

---

##### 2.2.03 数组翻转

<div style="font-size:1.2em; line-height:1.7;">**题干**：vector 原地反转元素顺序。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <vector>
#include <algorithm>
using namespace std;
int main()
{
    int n; cin >> n;
    vector<int> v(n);
    for(int i=0;i<n;i++) cin >> v[i];
    reverse(v.begin(),v.end());
    for(auto x:v) cout << x << " ";
    return 0;
}
```

</details>

---

##### 2.2.04 数组移位

<div style="font-size:1.2em; line-height:1.7;">**题干**：数组循环右移 k 位。如1,2,3,4,5右移 2 位 → 4,5,1,2,3。</div>

**样例**：

```text
题目：数组循环右移一位，1 2 3 4 →4 1 2 3
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int n;
    cin >> n;
    int a[105];
    for(int i=0;i<n;i++) cin >> a[i];
    int last = a[n-1];
    for(int i=n-1;i>=1;i--)
    {
        a[i]=a[i-1];
    }
    a[0]=last;
    for(int i=0;i<n;i++) cout << a[i] << " ";
    return 0;
}
```

</details>

---

##### 2.2.05 滑动窗口求和

<div style="font-size:1.2em; line-height:1.7;">**题干**：给定数组，计算连续 k 个数字的最大和。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int n, k, a[1000];
    cin >> n >> k;
    for (int i = 0; i < n; i++) cin >> a[i];
    int maxSum = 0;
    for (int i = 0; i <= n - k; i++)       // 窗口起点
    {
        int sum = 0;
        for (int j = i; j < i + k; j++)    // 累加窗口内k个数
            sum += a[j];
        if (i == 0 || sum > maxSum) maxSum = sum;
    }
    cout << maxSum;
    return 0;
}
```

</details>

---

#### ▸ 小类 B：排序与查找

##### 2.2.06 数组冒泡排序

<div style="font-size:1.2em; line-height:1.7;">**题干**：手动实现冒泡排序，对一组整数从小到大排序（禁止直接调用 sort）。</div>

**样例**：

```text
题目：n个整数，冒泡从小到大排序输出。 样例输入：5 3 1 4 2 5，输出：1 2 3 4 5
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int n;
    cin >> n;
    int a[105];
    for(int i=0;i<n;i++) cin >> a[i];
    //冒泡
    for(int i=0;i<n-1;i++)
    {
        for(int j=0;j<n-1-i;j++)
        {
            if(a[j]>a[j+1])
            {
                int t=a[j];
                a[j]=a[j+1];
                a[j+1]=t;
            }
        }
    }
    for(int i=0;i<n;i++) cout << a[i] << " ";
    return 0;
}
```

</details>

---

##### 2.2.07 选择排序实现

<div style="font-size:1.2em; line-height:1.7;">**题干**：手写选择排序算法。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int n;
    cin >> n;
    int a[105];
    for(int i=0;i<n;i++) cin >> a[i];
    for(int i=0;i<n-1;i++)
    {
        int pos = i;
        for(int j=i+1;j<n;j++)
        {
            if(a[j]<a[pos]) pos=j;
        }
        int t=a[i]; a[i]=a[pos]; a[pos]=t;
    }
    for(int i=0;i<n;i++) cout << a[i] << " ";
    return 0;
}
```

</details>

---

##### 2.2.08 顺序查找

<div style="font-size:1.2em; line-height:1.7;">**题干**：在数组里面查找目标数字，返回下标；不存在返回 - 1。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <vector>
#include <algorithm>
using namespace std;
int main()
{
    int n,key;
    cin >> n;
    vector<int> v(n);
    for(int i=0;i<n;i++) cin >> v[i];
    cin >> key;
    auto it = find(v.begin(),v.end(),key);
    if(it != v.end()) cout << "存在";
    else cout << "不存在";
    return 0;
}
```

</details>

---

##### 2.2.09 二分查找

<div style="font-size:1.2em; line-height:1.7;">**题干**：数组预先有序，手写二分查找函数。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <vector>
using namespace std;
int binarySearch(vector<int>& a, int target)
{
    int L = 0, R = a.size() - 1;
    while (L <= R)
    {
        int mid = (L + R) / 2;
        if (a[mid] == target) return mid;
        if (a[mid] < target) L = mid + 1;
        else R = mid - 1;
    }
    return -1;
}
int main()
{
    int n, x;
    cin >> n;
    vector<int> a(n);
    for (int i = 0; i < n; i++) cin >> a[i];   // 输入必须有序
    cin >> x;
    cout << binarySearch(a, x);
    return 0;
}
```

</details>

---

##### 2.2.10 数组去重

<div style="font-size:1.2em; line-height:1.7;">**题干**：有序数组去除重复数字，只保留一份。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <vector>
#include <algorithm>
using namespace std;
int main()
{
    int n; cin >> n;
    vector<int> v(n);
    for(int i=0;i<n;i++) cin >> v[i];
    sort(v.begin(),v.end());
    v.erase(unique(v.begin(),v.end()),v.end());
    for(auto x:v) cout << x << " ";
    return 0;
}
```

</details>

---

#### ▸ 小类 C：二维数组与矩阵

##### 2.2.11 二维矩阵打印

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入行数、列数，手动输入矩阵数字，整齐格式化输出。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <vector>
using namespace std;
int main()
{
    int r,c;
    cin >> r >> c;
    vector<vector<int>> mat(r, vector<int>(c));
    for(int i=0;i<r;i++)
        for(int j=0;j<c;j++)
            cin >> mat[i][j];
    for(int i=0;i<r;i++)
    {
        for(int j=0;j<c;j++) cout << mat[i][j] << " ";
        cout << endl;
    }
    return 0;
}
```

</details>

---

##### 2.2.12 矩阵加法

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入两个相同大小矩阵，计算矩阵相加结果。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int n, m, a[50][50], b[50][50];
    cin >> n >> m;
    for (int i = 0; i < n; i++)
        for (int j = 0; j < m; j++)
            cin >> a[i][j];
    for (int i = 0; i < n; i++)
        for (int j = 0; j < m; j++)
            cin >> b[i][j];
    for (int i = 0; i < n; i++)
    {
        for (int j = 0; j < m; j++)
            cout << a[i][j] + b[i][j] << ' ';
        cout << endl;
    }
    return 0;
}
```

</details>

---

##### 2.2.13 矩阵转置

<div style="font-size:1.2em; line-height:1.7;">**题干**：m 行 n 列矩阵，行列互换得到转置矩阵。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <vector>
using namespace std;
int main()
{
    int r,c; cin >> r >> c;
    vector<vector<int>> mat(r,vector<int>(c));
    for(int i=0;i<r;i++)
        for(int j=0;j<c;j++) cin >> mat[i][j];
    vector<vector<int>> t(c,vector<int>(r));
    for(int i=0;i<r;i++)
        for(int j=0;j<c;j++)
            t[j][i] = mat[i][j];
    for(int i=0;i<c;i++)
    {
        for(int j=0;j<r;j++) cout << t[i][j] << " ";
        cout << endl;
    }
    return 0;
}
```

</details>

---

##### 2.2.14 矩阵对角线求和

<div style="font-size:1.2em; line-height:1.7;">**题干**：方阵，求主对角线所有元素之和。</div>

**样例**：

```text
题目：n阶方阵，求主对角线元素之和（i==j）
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int n,sum=0;
    cin >> n;
    int a[105][105];
    for(int i=0;i<n;i++)
        for(int j=0;j<n;j++)
            cin >> a[i][j];
    for(int i=0;i<n;i++)
        sum += a[i][i];
    cout << sum;
    return 0;
}
```

</details>

---

##### 2.2.15 矩阵行列最大值

<div style="font-size:1.2em; line-height:1.7;">**题干**：二维数组，找出每一行最大值，每一列最大值。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int n, m, a[50][50];
    cin >> n >> m;
    for (int i = 0; i < n; i++)
        for (int j = 0; j < m; j++)
            cin >> a[i][j];
    // 每行最大值
    for (int i = 0; i < n; i++)
    {
        int mx = a[i][0];
        for (int j = 1; j < m; j++)
            if (a[i][j] > mx) mx = a[i][j];
        cout << "第" << i+1 << "行最大: " << mx << endl;
    }
    // 每列最大值
    for (int j = 0; j < m; j++)
    {
        int mx = a[0][j];
        for (int i = 1; i < n; i++)
            if (a[i][j] > mx) mx = a[i][j];
        cout << "第" << j+1 << "列最大: " << mx << endl;
    }
    return 0;
}
```

</details>

---

#### ▸ 小类 D：数据处理与集合

##### 2.2.16 合并两个有序数组

<div style="font-size:1.2em; line-height:1.7;">**题干**：两个升序数组，合并成一个新升序数组。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <vector>
using namespace std;
int main()
{
    int n,m;
    cin >> n; vector<int> a(n); for(int i=0;i<n;i++) cin >> a[i];
    cin >> m; vector<int> b(m); for(int i=0;i<m;i++) cin >> b[i];
    vector<int> res;
    int i=0,j=0;
    while(i<n && j<m)
    {
        if(a[i] < b[j]) res.push_back(a[i++]);
        else res.push_back(b[j++]);
    }
    while(i<n) res.push_back(a[i++]);
    while(j<m) res.push_back(b[j++]);
    for(auto x:res) cout << x << " ";
    return 0;
}
```

</details>

---

##### 2.2.17 学生分数管理

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入多名学生姓名 + 分数存入 vector 结构体，支持添加、查看全部成绩。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <string>
using namespace std;
struct Student
{
    string name;
    int score;
};
int main()
{
    Student s;
    cin >> s.name >> s.score;
    cout << s.name << " " << s.score << endl;
    return 0;
}
```

</details>

---

##### 2.2.18 找出数组众数

<div style="font-size:1.2em; line-height:1.7;">**题干**：数组中出现次数最多的数字。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int n, a[1000], cnt[1001] = {0};
    cin >> n;
    for (int i = 0; i < n; i++)
    {
        cin >> a[i];
        cnt[a[i]]++;
    }
    int best = a[0];
    for (int i = 0; i < n; i++)
        if (cnt[a[i]] > cnt[best]) best = a[i];   // 出现次数最多
    cout << best;
    return 0;
}
```

</details>

---

##### 2.2.19 数组拆分奇偶

<div style="font-size:1.2em; line-height:1.7;">**题干**：把数组分成两组，奇数放前面，偶数放后面，保持原有相对顺序。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <vector>
using namespace std;
int main()
{
    int n; cin >> n;
    vector<int> v,odd,even;
    for(int i=0;i<n;i++)
    {
        int x; cin >> x;
        v.push_back(x);
        if(x%2==0) even.push_back(x);
        else odd.push_back(x);
    }
    cout << "奇数："; for(auto x:odd) cout << x << " ";
    cout << "\n偶数："; for(auto x:even) cout << x << " ";
    return 0;
}
```

</details>

---

##### 2.2.20 洗牌算法

<div style="font-size:1.2em; line-height:1.7;">**题干**：vector 存放卡牌编号，实现随机打乱数组元素（洗牌）。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <vector>
#include <cstdlib>
#include <ctime>
#include <algorithm>
using namespace std;
int main()
{
    srand(time(0));
    int n;
    cin >> n;
    vector<int> v(n);
    for (int i = 0; i < n; i++) v[i] = i + 1;
    for (int i = n - 1; i > 0; i--)     // Fisher-Yates 洗牌
    {
        int j = rand() % (i + 1);
        swap(v[i], v[j]);
    }
    for (int i = 0; i < n; i++) cout << v[i] << ' ';
    return 0;
}
```

</details>

---

##### 2.2.21 数组差分数组

<div style="font-size:1.2em; line-height:1.7;">**题干**：简易差分数组，支持区间批量增加数字，最后还原数组。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int n, m, a[100] = {0}, diff[101] = {0};
    cin >> n >> m;      // n个数，m次区间操作
    for (int i = 0; i < n; i++) cin >> a[i];
    for (int t = 0; t < m; t++)
    {
        int l, r, v;    // 区间[l, r]整体加v（下标从1开始）
        cin >> l >> r >> v;
        diff[l] += v;
        diff[r + 1] -= v;
    }
    int cur = 0;
    for (int i = 1; i <= n; i++)
    {
        cur += diff[i];               // 差分前缀和 = 每个位置增量
        cout << a[i-1] + cur << ' ';
    }
    return 0;
}
```

</details>

---

##### 2.2.22 集合交集

<div style="font-size:1.2em; line-height:1.7;">**题干**：两个整数集合（vector），找出同时存在于两个集合的数字。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <vector>
using namespace std;
int main()
{
    int n, m, x;
    vector<int> A, B, C;
    cin >> n;
    for (int i = 0; i < n; i++) { cin >> x; A.push_back(x); }
    cin >> m;
    for (int i = 0; i < m; i++) { cin >> x; B.push_back(x); }
    for (int i = 0; i < n; i++)
    {
        bool inB = false;
        for (int j = 0; j < m; j++)
            if (A[i] == B[j]) inB = true;
        bool dup = false;
        for (int j = 0; j < C.size(); j++)
            if (C[j] == A[i]) dup = true;
        if (inB && !dup) C.push_back(A[i]);   // 在B中且未重复加入
    }
    for (int i = 0; i < C.size(); i++) cout << C[i] << ' ';
    return 0;
}
```

</details>

---

##### 2.2.23 集合并集

<div style="font-size:1.2em; line-height:1.7;">**题干**：合并两个集合，去掉重复元素。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <vector>
using namespace std;
int main()
{
    int n, m, x;
    vector<int> A, B, C;
    cin >> n;
    for (int i = 0; i < n; i++) { cin >> x; A.push_back(x); }
    cin >> m;
    for (int i = 0; i < m; i++) { cin >> x; B.push_back(x); }
    // 先加入A
    for (int i = 0; i < n; i++)
    {
        bool dup = false;
        for (int j = 0; j < C.size(); j++)
            if (C[j] == A[i]) dup = true;
        if (!dup) C.push_back(A[i]);
    }
    // 再加入B中不重复的
    for (int i = 0; i < m; i++)
    {
        bool dup = false;
        for (int j = 0; j < C.size(); j++)
            if (C[j] == B[i]) dup = true;
        if (!dup) C.push_back(B[i]);
    }
    for (int i = 0; i < C.size(); i++) cout << C[i] << ' ';
    return 0;
}
```

</details>

---

##### 2.2.24 集合差集

<div style="font-size:1.2em; line-height:1.7;">**题干**：A 集合减去 B 集合里存在的元素。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <vector>
using namespace std;
int main()
{
    int n, m, x;
    vector<int> A, B;
    cin >> n;
    for (int i = 0; i < n; i++) { cin >> x; A.push_back(x); }
    cin >> m;
    for (int i = 0; i < m; i++) { cin >> x; B.push_back(x); }
    for (int i = 0; i < n; i++)       // 输出A中不在B里的元素
    {
        bool inB = false;
        for (int j = 0; j < m; j++)
            if (A[i] == B[j]) inB = true;
        if (!inB) cout << A[i] << ' ';
    }
    return 0;
}
```

</details>

---

##### 2.2.25 生命游戏极简版

<div style="font-size:1.2em; line-height:1.7;">**题干**：二维数组模拟康威生命游戏一代演化（只计算一代，不循环动画）。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int n, m, a[20][20], b[20][20];
    cin >> n >> m;
    for (int i = 0; i < n; i++)
        for (int j = 0; j < m; j++)
            cin >> a[i][j];           // 1活 0死
    for (int i = 0; i < n; i++)
    {
        for (int j = 0; j < m; j++)
        {
            int live = 0;             // 周围8格活细胞数
            for (int di = -1; di <= 1; di++)
                for (int dj = -1; dj <= 1; dj++)
                {
                    if (di == 0 && dj == 0) continue;
                    int ni = i + di, nj = j + dj;
                    if (ni >= 0 && ni < n && nj >= 0 && nj < m && a[ni][nj] == 1)
                        live++;
                }
            if (a[i][j] == 1)
                b[i][j] = (live == 2 || live == 3) ? 1 : 0;  // 存活规则
            else
                b[i][j] = (live == 3) ? 1 : 0;               // 繁殖规则
        }
    }
    for (int i = 0; i < n; i++)
    {
        for (int j = 0; j < m; j++)
            cout << b[i][j] << ' ';
        cout << endl;
    }
    return 0;
}
```

</details>

---

### 2.3 基础算法与数学（基础算法与数学专题）

#### ▸ 小类 A：递归与递推

##### 2.3.01 递归求阶乘

<div style="font-size:1.2em; line-height:1.7;">**题干**：用递归函数实现 n 的阶乘。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
long long f(int x)
{
    if(x==0 || x==1) return 1;
    return f(x-1)*x;
}
int main()
{
    int n;
    cin >> n;
    cout << f(n);
    return 0;
}
```

</details>

---

##### 2.3.02 递归斐波那契

<div style="font-size:1.2em; line-height:1.7;">**题干**：递归输出斐波那契第 n 项。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int fib(int x)
{
    if(x==1 || x==2) return 1;
    return fib(x-1)+fib(x-2);
}
int main()
{
    int n;
    cin >> n;
    cout << fib(n);
    return 0;
}
```

</details>

---

##### 2.3.03 递归倒序输出数字

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入整数，递归打印每一位数字。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
void printRev(int n)
{
    if (n == 0) return;         // 递归出口
    cout << n % 10;             // 先输出最后一位
    printRev(n / 10);           // 再处理前面部分
}
int main()
{
    int n;
    cin >> n;
    if (n == 0) cout << 0;
    else printRev(n);
    return 0;
}
```

</details>

---

#### ▸ 小类 B：数论基础

##### 2.3.04 最大公约数（欧几里得算法）

<div style="font-size:1.2em; line-height:1.7;">**题干**：手写 gcd 函数，递归实现。</div>

**样例**：

```text
输入12 18，输出6
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int gcd(int a,int b)
{
    while(b)
    {
        int t = a % b;
        a = b;
        b = t;
    }
    return a;
}
int main()
{
    int x,y;
    cin >> x >> y;
    cout << gcd(x,y) << endl;
    return 0;
}
```

</details>

---

##### 2.3.05 最小公倍数

<div style="font-size:1.2em; line-height:1.7;">**题干**：利用 gcd 计算 lcm。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int gcd(int a,int b)
{
    while(b){int t=a%b;a=b;b=t;}
    return a;
}
int lcm(int a,int b)
{
    return a / gcd(a,b) * b;
}
int main()
{
    int x,y;
    cin >> x >> y;
    cout << lcm(x,y) << endl;
    return 0;
}
```

</details>

---

##### 2.3.06 分解质因数

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入整数，输出质因数分解结果。例：12=223。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int n;
    cin >> n;
    for(int i=2;i*i<=n;i++)
    {
        while(n%i == 0)
        {
            cout << i << " ";
            n /= i;
        }
    }
    if(n>1) cout << n;
    return 0;
}
```

</details>

---

##### 2.3.07 埃氏筛法

<div style="font-size:1.2em; line-height:1.7;">**题干**：筛出 1~n 之间所有质数。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
bool vis[1005];
int main()
{
    int n;
    cin >> n;
    for(int i=2;i<=n;i++)
    {
        if(!vis[i])
        {
            cout << i << " ";
            for(int j=2*i;j<=n;j+=i)
                vis[j]=true;
        }
    }
    return 0;
}
```

</details>

---

##### 2.3.08 水仙花数查找

<div style="font-size:1.2em; line-height:1.7;">**题干**：找出所有三位数水仙花数。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
bool isNarc(int n)
{
    int a = n/100;
    int b = n/10%10;
    int c = n%10;
    return a*a*a + b*b*b + c*c*c == n;
}
int main()
{
    int x;
    cin >> x;
    if(isNarc(x)) cout << "水仙花数";
    else cout << "不是";
    return 0;
}
```

</details>

---

##### 2.3.09 阿姆斯特朗数通用判断

<div style="font-size:1.2em; line-height:1.7;">**题干**：任意位数，判断是否等于各位数字次方之和。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int n;
    cin >> n;
    int t = n, d = 0, digits[10];
    while (t > 0)               // 拆出每一位
    {
        digits[d++] = t % 10;
        t /= 10;
    }
    long long sum = 0;
    for (int i = 0; i < d; i++)
    {
        long long p = 1;
        for (int j = 0; j < d; j++) p *= digits[i];   // 位数次方
        sum += p;
    }
    cout << (sum == n ? "是" : "不是");
    return 0;
}
```

</details>

---

##### 2.3.10 判断亲和数

<div style="font-size:1.2em; line-height:1.7;">**题干**：两个数 A、B，A 所有真因数之和 = B，B 真因数之和 = A。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int sumDiv(int x)
{
    int s = 0;
    for (int i = 1; i < x; i++)
        if (x % i == 0) s += i;    // 真因数之和
    return s;
}
int main()
{
    int a, b;
    cin >> a >> b;
    if (sumDiv(a) == b && sumDiv(b) == a)
        cout << "是亲和数";
    else
        cout << "不是亲和数";
    return 0;
}
```

</details>

---

##### 2.3.11 卡特兰数计算

<div style="font-size:1.2em; line-height:1.7;">**题干**：计算第 n 个卡特兰数。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int n;
    cin >> n;
    long long c[30];
    c[0] = 1;
    for (int i = 1; i <= n; i++)
        c[i] = c[i-1] * (4 * i - 2) / (i + 1);   // 卡特兰数递推
    cout << c[n];
    return 0;
}
```

</details>

---

##### 2.3.12 快速幂简易实现

<div style="font-size:1.2em; line-height:1.7;">**题干**：手写快速幂，计算 a^b mod modu。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
long long qpow(long long a,long long b,long long p)
{
    long long res=1;
    while(b>0)
    {
        if(b&1) res = res * a % p;
        a = a*a % p;
        b >>= 1;
    }
    return res;
}
int main()
{
    long long a,b,p;
    cin >> a >> b >> p;
    cout << qpow(a,b,p);
    return 0;
}
```

</details>

---

##### 2.3.13 素因子统计

<div style="font-size:1.2em; line-height:1.7;">**题干**：统计一个数字不同质因子有多少种。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int n, cnt = 0;
    cin >> n;
    for (int p = 2; p * p <= n; p++)
    {
        if (n % p == 0)
        {
            cnt++;                      // 发现一个新质因子
            while (n % p == 0) n /= p;  // 除干净
        }
    }
    if (n > 1) cnt++;                   // 剩余的大质因子
    cout << cnt;
    return 0;
}
```

</details>

---

#### ▸ 小类 C：枚举与搜索

##### 2.3.14 硬币找零（贪心版）

<div style="font-size:1.2em; line-height:1.7;">**题干**：给定面额，输入金额，用最少硬币凑出金额。</div>

**样例**：

```text
题目：硬币面值1,5,10,50，输入金额，贪心求最少硬币数量。 样例输入：37 → 5+10+10+10+1+1 =5枚
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int x;
    cin >> x;
    int coin[]={50,10,5,1};
    int cnt=0;
    for(int i=0;i<4;i++)
    {
        cnt += x / coin[i];
        x = x % coin[i];
    }
    cout << cnt;
    return 0;
}
```

</details>

---

##### 2.3.15 整数拆分枚举

<div style="font-size:1.2em; line-height:1.7;">**题干**：把一个正整数拆成若干正整数之和，打印所有拆分方案。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int n, path[20];
void dfs(int left, int minPart, int len)
{
    if (left == 0)
    {
        if (len >= 2)   // 至少拆成两个正整数
        {
            for (int i = 0; i < len; i++)
                cout << path[i] << (i == len-1 ? '\n' : '+');
        }
        return;
    }
    for (int x = minPart; x <= left; x++)   // 不降序，避免重复
    {
        path[len] = x;
        dfs(left - x, x, len + 1);
    }
}
int main()
{
    cin >> n;
    dfs(n, 1, 0);
    return 0;
}
```

</details>

---

##### 2.3.16 完全背包简易枚举

<div style="font-size:1.2em; line-height:1.7;">**题干**：物品可重复拿，求最大价值（枚举实现）。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int n, W, w[20], v[20], best = 0;
void dfs(int i, int weight, int value)
{
    if (i == n)
    {
        if (value > best) best = value;
        return;
    }
    for (int k = 0; weight + k * w[i] <= W; k++)   // 第i件拿k个
        dfs(i + 1, weight + k * w[i], value + k * v[i]);
}
int main()
{
    cin >> n >> W;
    for (int i = 0; i < n; i++) cin >> w[i] >> v[i];
    dfs(0, 0, 0);
    cout << best;
    return 0;
}
```

</details>

---

##### 2.3.17 01 背包小数据版本

<div style="font-size:1.2em; line-height:1.7;">**题干**：每件物品只能选或不选，枚举所有组合求最大价值。</div>

**样例**：

```text
题目：n件物品，背包容量V，每件物品重量w，价值v，求最大价值。
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <algorithm>
using namespace std;
int dp[1005];
int main()
{
    int n,V;
    cin >> n >> V;
    for(int i=1;i<=n;i++)
    {
        int w,v;
        cin >> w >> v;
        for(int j=V;j>=w;j--)
        {
            dp[j] = max(dp[j], dp[j-w]+v);
        }
    }
    cout << dp[V];
    return 0;
}
```

</details>

---

##### 2.3.18 八皇后简化版

<div style="font-size:1.2em; line-height:1.7;">**题干**：四皇后：枚举找出 4×4 棋盘放置 4 个皇后互不攻击的全部方案。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int ans[5], cnt = 0;
bool ok(int row, int col)
{
    for (int r = 1; r < row; r++)
        if (ans[r] == col || ans[r] - r == col - row || ans[r] + r == col + row)
            return false;       // 同列或同一对角线
    return true;
}
void dfs(int row)
{
    if (row == 5) { cnt++; return; }   // 4行都放好了
    for (int col = 1; col <= 4; col++)
        if (ok(row, col))
        {
            ans[row] = col;
            dfs(row + 1);
        }
}
int main()
{
    dfs(1);
    cout << cnt;   // 4皇后方案数
    return 0;
}
```

</details>

---

##### 2.3.19 排列生成

<div style="font-size:1.2em; line-height:1.7;">**题干**：枚举 1~n 全部排列并打印。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int n;
int a[105];
bool vis[105];
void dfs(int step)
{
    if(step == n+1)
    {
        for(int i=1;i<=n;i++) cout << a[i] << " ";
        cout << endl;
        return;
    }
    for(int i=1;i<=n;i++)
    {
        if(!vis[i])
        {
            vis[i]=true;
            a[step]=i;
            dfs(step+1);
            vis[i]=false;
        }
    }
}
int main()
{
    cin >> n;
    dfs(1);
    return 0;
}
```

</details>

---

##### 2.3.20 组合生成

<div style="font-size:1.2em; line-height:1.7;">**题干**：从 n 个数选出 k 个，输出全部组合。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int n, k, path[20];
void dfs(int start, int len)
{
    if (len == k)
    {
        for (int i = 0; i < k; i++)
            cout << path[i] << (i == k-1 ? '\n' : ' ');
        return;
    }
    for (int x = start; x <= n; x++)
    {
        path[len] = x;
        dfs(x + 1, len + 1);   // 下一个数必须更大，保证不重复
    }
}
int main()
{
    cin >> n >> k;
    dfs(1, 0);
    return 0;
}
```

</details>

---

##### 2.3.21 池塘计数（连通块）

<div style="font-size:1.2em; line-height:1.7;">**题干**：二维地图，'#' 代表水，统计连通池塘数量（简易 DFS）。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int n, m;
char g[20][20];
bool vis[20][20];
int dx[4] = {-1, 1, 0, 0};
int dy[4] = {0, 0, -1, 1};
void dfs(int x, int y)
{
    vis[x][y] = true;
    for (int k = 0; k < 4; k++)     // 四方向扩展
    {
        int nx = x + dx[k], ny = y + dy[k];
        if (nx >= 0 && nx < n && ny >= 0 && ny < m
            && g[nx][ny] == '#' && !vis[nx][ny])
            dfs(nx, ny);
    }
}
int main()
{
    cin >> n >> m;
    for (int i = 0; i < n; i++)
        for (int j = 0; j < m; j++)
            cin >> g[i][j];
    int cnt = 0;
    for (int i = 0; i < n; i++)
        for (int j = 0; j < m; j++)
            if (g[i][j] == '#' && !vis[i][j])
            {
                cnt++;      // 发现一个新池塘
                dfs(i, j);
            }
    cout << cnt;
    return 0;
}
```

</details>

---

#### ▸ 小类 D：数学应用

##### 2.3.22 数字进制转换

<div style="font-size:1.2em; line-height:1.7;">**题干**：十进制转 2/8/16 进制，输出字符串形式。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <string>
using namespace std;
string toBase(int n, int b)
{
    if (n == 0) return "0";
    string s = "";
    while (n > 0)
    {
        int r = n % b;
        if (r < 10) s = char('0' + r) + s;
        else s = char('A' + r - 10) + s;   // 10->A, 11->B ...
        n /= b;
    }
    return s;
}
int main()
{
    int n;
    cin >> n;
    cout << "2进制: " << toBase(n, 2) << endl;
    cout << "8进制: " << toBase(n, 8) << endl;
    cout << "16进制: " << toBase(n, 16) << endl;
    return 0;
}
```

</details>

---

##### 2.3.23 二进制转十进制，输入二进制字符串，转为十进制数字

<div style="font-size:1.2em; line-height:1.7;">**题干**：（无补充描述）</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <string>
using namespace std;
int main()
{
    string s;
    cin >> s;
    int ans = 0;
    for (int i = 0; i < s.size(); i++)
        ans = ans * 2 + (s[i] - '0');   // 逐位累加
    cout << ans;
    return 0;
}
```

</details>

---

##### 2.3.24 日期计算器

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入年月日，计算这一天是当年第几天。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
bool isLeap(int y)
{
    return (y % 4 == 0 && y % 100 != 0) || y % 400 == 0;
}
int main()
{
    int y, m, d;
    cin >> y >> m >> d;
    int days[13] = {0,31,28,31,30,31,30,31,31,30,31,30,31};
    if (isLeap(y)) days[2] = 29;   // 闰年2月29天
    int sum = 0;
    for (int i = 1; i < m; i++) sum += days[i];
    sum += d;
    cout << sum;
    return 0;
}
```

</details>

---

##### 2.3.25 日期差计算

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入两个年月日，计算相隔多少天。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
bool isLeap(int y)
{
    return (y % 4 == 0 && y % 100 != 0) || y % 400 == 0;
}
long long daysFrom1(int y, int m, int d)   // 公元1年1月1日到该日期的天数
{
    long long sum = 0;
    for (int yy = 1; yy < y; yy++)
        sum += isLeap(yy) ? 366 : 365;
    int days[13] = {0,31,28,31,30,31,30,31,31,30,31,30,31};
    if (isLeap(y)) days[2] = 29;
    for (int mm = 1; mm < m; mm++) sum += days[mm];
    sum += d;
    return sum;
}
int main()
{
    int y1, m1, d1, y2, m2, d2;
    cin >> y1 >> m1 >> d1 >> y2 >> m2 >> d2;
    long long a = daysFrom1(y1, m1, d1);
    long long b = daysFrom1(y2, m2, d2);
    cout << (a > b ? a - b : b - a);   // 相差天数
    return 0;
}
```

</details>

---

##### 2.3.26 蒙特卡洛求 π

<div style="font-size:1.2em; line-height:1.7;">**题干**：随机撒点模拟估算圆周率。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <cstdlib>
#include <ctime>
using namespace std;
int main()
{
    srand(time(0));
    long long n, in = 0;
    cin >> n;                 // 撒点数
    for (long long i = 0; i < n; i++)
    {
        double x = rand() / (double)RAND_MAX;   // 0~1随机
        double y = rand() / (double)RAND_MAX;
        if (x * x + y * y <= 1.0) in++;         // 落在1/4圆内
    }
    double pi = 4.0 * in / n;                   // 面积比 = π/4
    cout << pi;
    return 0;
}
```

</details>

---

##### 2.3.27 整数分割回文

<div style="font-size:1.2em; line-height:1.7;">**题干**：判断数字能否拆成多个回文数之和。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
bool isPalin(int x)
{
    int t = x, r = 0;
    while (t > 0)
    {
        r = r * 10 + t % 10;
        t /= 10;
    }
    return r == x;
}
bool can(int left)
{
    if (left == 0) return true;
    for (int x = 1; x <= left; x++)
        if (isPalin(x) && can(left - x)) return true;
    return false;
}
int main()
{
    int n;
    cin >> n;
    cout << (can(n) ? "可以" : "不可以");
    return 0;
}
```

</details>

---

##### 2.3.28 罗马数字转阿拉伯数字

<div style="font-size:1.2em; line-height:1.7;">**题干**：（无补充描述）</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <string>
using namespace std;
int val(char c)
{
    if (c == 'I') return 1;
    if (c == 'V') return 5;
    if (c == 'X') return 10;
    if (c == 'L') return 50;
    if (c == 'C') return 100;
    if (c == 'D') return 500;
    return 1000;   // M
}
int main()
{
    string s;
    cin >> s;
    int ans = 0;
    for (int i = 0; i < s.size(); i++)
    {
        if (i + 1 < s.size() && val(s[i]) < val(s[i+1]))
            ans -= val(s[i]);   // 小数字在前：如 IV = 4
        else
            ans += val(s[i]);
    }
    cout << ans;
    return 0;
}
```

</details>

---

##### 2.3.29 阿拉伯数字转罗马数字

<div style="font-size:1.2em; line-height:1.7;">**题干**：（无补充描述）</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <string>
using namespace std;
int main()
{
    int n;
    cin >> n;
    string s = "";
    int num[13] = {1000,900,500,400,100,90,50,40,10,9,5,4,1};
    string rom[13] = {"M","CM","D","CD","C","XC","L","XL","X","IX","V","IV","I"};
    for (int i = 0; i < 13; i++)
        while (n >= num[i])     // 从大到小尽量用
        {
            s += rom[i];
            n -= num[i];
        }
    cout << s;
    return 0;
}
```

</details>

---

##### 2.3.30 最大子数组和（Kadane 算法）

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入整数数组，求连续子数组最大和。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int n,a[105],s[105]={0};
    cin >> n;
    for(int i=1;i<=n;i++)
    {
        cin >> a[i];
        s[i]=s[i-1]+a[i];
    }
    int min_s = 0, res = -1e9;
    for(int i=1;i<=n;i++)
    {
        res = max(res, s[i]-min_s);
        min_s = min(min_s, s[i]);
    }
    cout << res;
    return 0;
}
```

</details>

---

### 2.4 综合小游戏与实用工具（综合小游戏与实用工具）

#### ▸ 小类 A：信息管理工具

##### 2.4.01 简易通讯录 V1

<div style="font-size:1.2em; line-height:1.7;">**题干**：结构体存储姓名、电话；支持新增、查询、删除联系人。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <fstream>
#include <string>
#include <vector>
using namespace std;

struct Contact
{
    string name;
    string phone;
};

//保存全部通讯录到文件
void saveToFile(const vector<Contact> &vec)
{
    ofstream fout("contact.txt");
    for(auto &c : vec)
    {
        fout << c.name << " " << c.phone << endl;
    }
    fout.close();
}

//从文件读取通讯录
vector<Contact> loadFromFile()
{
    vector<Contact> res;
    ifstream fin("contact.txt");
    string n,p;
    while(fin >> n >> p)
    {
        res.push_back({n,p});
    }
    fin.close();
    return res;
}

int main()
{
    vector<Contact> book = loadFromFile();
    int op;
    cout << "====通讯录===="<<endl;
    cout << "1 添加联系人  2 查询联系人  0 退出"<<endl;
    while(cin >> op)
    {
        if(op == 0)
        {
            saveToFile(book);
            cout << "已保存，程序退出"<<endl;
            break;
        }
        else if(op == 1)
        {
            string na,ph;
            cout << "输入姓名 电话：";
            cin >> na >> ph;
            book.push_back({na,ph});
            cout << "添加成功"<<endl;
        }
        else if(op == 2)
        {
            string key;
            cout << "输入要查找姓名：";
            cin >> key;
            bool found = false;
            for(auto &c : book)
            {
                if(c.name == key)
                {
                    cout << "找到：" << c.name << " 电话：" << c.phone << endl;
                    found = true;
                    break;
                }
            }
            if(!found) cout << "查无此人"<<endl;
        }
        cout << "\n1 添加联系人  2 查询联系人  0 退出"<<endl;
    }
    return 0;
}
```

</details>

---

##### 2.4.02 通讯录 V2（文件版）

<div style="font-size:1.2em; line-height:1.7;">**题干**：程序退出自动保存到 txt，打开自动加载联系人。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <fstream>
#include <string>
#include <vector>
using namespace std;

struct Contact
{
    string name;
    string phone;
};

//保存全部通讯录到文件
void saveToFile(const vector<Contact> &vec)
{
    ofstream fout("contact.txt");
    for(auto &c : vec)
    {
        fout << c.name << " " << c.phone << endl;
    }
    fout.close();
}

//从文件读取通讯录
vector<Contact> loadFromFile()
{
    vector<Contact> res;
    ifstream fin("contact.txt");
    string n,p;
    while(fin >> n >> p)
    {
        res.push_back({n,p});
    }
    fin.close();
    return res;
}

int main()
{
    vector<Contact> book = loadFromFile();
    int op;
    cout << "====通讯录===="<<endl;
    cout << "1 添加联系人  2 查询联系人  0 退出"<<endl;
    while(cin >> op)
    {
        if(op == 0)
        {
            saveToFile(book);
            cout << "已保存，程序退出"<<endl;
            break;
        }
        else if(op == 1)
        {
            string na,ph;
            cout << "输入姓名 电话：";
            cin >> na >> ph;
            book.push_back({na,ph});
            cout << "添加成功"<<endl;
        }
        else if(op == 2)
        {
            string key;
            cout << "输入要查找姓名：";
            cin >> key;
            bool found = false;
            for(auto &c : book)
            {
                if(c.name == key)
                {
                    cout << "找到：" << c.name << " 电话：" << c.phone << endl;
                    found = true;
                    break;
                }
            }
            if(!found) cout << "查无此人"<<endl;
        }
        cout << "\n1 添加联系人  2 查询联系人  0 退出"<<endl;
    }
    return 0;
}
```

</details>

---

##### 2.4.03 简易银行账户模拟器

<div style="font-size:1.2em; line-height:1.7;">**题干**：结构体存储多个账户，开户、查询余额、存款、取款。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <string>
using namespace std;
struct Account
{
    string name;
    int id;
    double balance;
};
Account acc[100];
int n = 0;
int findById(int id)
{
    for (int i = 0; i < n; i++)
        if (acc[i].id == id) return i;
    return -1;
}
int main()
{
    int choice;
    while (true)
    {
        cout << "1开户 2查询 3存款 4取款 5退出: ";
        cin >> choice;
        if (choice == 1)
        {
            cout << "姓名 账号: ";
            cin >> acc[n].name >> acc[n].id;
            acc[n].balance = 0;
            n++;
            cout << "开户成功" << endl;
        }
        else if (choice == 2)
        {
            int id;
            cout << "账号: ";
            cin >> id;
            int i = findById(id);
            if (i == -1) cout << "账户不存在" << endl;
            else cout << acc[i].name << " 余额: " << acc[i].balance << endl;
        }
        else if (choice == 3)
        {
            int id; double v;
            cout << "账号 存款金额: ";
            cin >> id >> v;
            int i = findById(id);
            if (i == -1) cout << "账户不存在" << endl;
            else { acc[i].balance += v; cout << "存款成功" << endl; }
        }
        else if (choice == 4)
        {
            int id; double v;
            cout << "账号 取款金额: ";
            cin >> id >> v;
            int i = findById(id);
            if (i == -1 || acc[i].balance < v) cout << "取款失败" << endl;
            else { acc[i].balance -= v; cout << "取款成功" << endl; }
        }
        else break;
    }
    return 0;
}
```

</details>

---

##### 2.4.04 成绩管理系统完整版

<div style="font-size:1.2em; line-height:1.7;">**题干**：录入学生，按分数排序，查询、删除，导出成绩文件。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <fstream>
#include <string>
#include <vector>
#include <algorithm>
using namespace std;
struct Student
{
    string name;
    int score;
};
bool cmp(const Student &a,const Student &b)
{
    return a.score>b.score;
}
int main()
{
    int n; cin >> n;
    vector<Student> st(n);
    for(int i=0;i<n;i++) cin >> st[i].name >> st[i].score;
    sort(st.begin(),st.end(),cmp);
    ofstream fout("sorted_stu.txt");
    for(auto s:st) fout << s.name << " " << s.score << endl;
    fout.close();
    cout << "排序并保存完成";
    return 0;
}
```

</details>

---

##### 2.4.05 简易 BBS 留言板

<div style="font-size:1.2em; line-height:1.7;">**题干**：程序运行时可以新增留言，查看全部留言，支持删除。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <string>
using namespace std;
string msgs[100];
int n = 0;
int main()
{
    int choice;
    while (true)
    {
        cout << "1留言 2查看 3删除 4退出: ";
        cin >> choice;
        cin.ignore();   // 吃掉回车
        if (choice == 1)
        {
            cout << "输入留言: ";
            getline(cin, msgs[n]);
            n++;
        }
        else if (choice == 2)
        {
            for (int i = 0; i < n; i++)
                cout << i + 1 << ". " << msgs[i] << endl;
        }
        else if (choice == 3)
        {
            int idx;
            cout << "删除编号: ";
            cin >> idx;
            if (idx < 1 || idx > n) cout << "无效编号" << endl;
            else
            {
                for (int i = idx - 1; i < n - 1; i++) msgs[i] = msgs[i+1];
                n--;
            }
        }
        else break;
    }
    return 0;
}
```

</details>

---

##### 2.4.06 任务待办管理器

<div style="font-size:1.2em; line-height:1.7;">**题干**：添加待办、标记完成、删除任务、保存任务列表。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <fstream>
#include <string>
using namespace std;
string tasks[100];
bool done[100];
int n = 0;
void load()
{
    ifstream fin("tasks.txt");
    while (getline(fin, tasks[n])) n++;
    fin.close();
}
void save()
{
    ofstream fout("tasks.txt");
    for (int i = 0; i < n; i++)
        fout << (done[i] ? "[x] " : "[ ] ") << tasks[i] << endl;
    fout.close();
}
int main()
{
    load();
    int choice;
    while (true)
    {
        cout << "1添加 2标记完成 3删除 4查看 5退出: ";
        cin >> choice;
        cin.ignore();
        if (choice == 1)
        {
            cout << "任务内容: ";
            getline(cin, tasks[n]);
            done[n] = false;
            n++;
            save();
        }
        else if (choice == 2)
        {
            int idx;
            cout << "编号: ";
            cin >> idx;
            if (idx >= 1 && idx <= n) { done[idx-1] = true; save(); }
        }
        else if (choice == 3)
        {
            int idx;
            cout << "编号: ";
            cin >> idx;
            if (idx >= 1 && idx <= n)
            {
                for (int i = idx - 1; i < n - 1; i++)
                {
                    tasks[i] = tasks[i+1];
                    done[i] = done[i+1];
                }
                n--;
                save();
            }
        }
        else if (choice == 4)
        {
            for (int i = 0; i < n; i++)
                cout << i + 1 << ". " << (done[i] ? "[完成] " : "[待办] ") << tasks[i] << endl;
        }
        else break;
    }
    return 0;
}
```

</details>

---

#### ▸ 小类 B：经典小游戏

##### 2.4.07 文字版五子棋

<div style="font-size:1.2em; line-height:1.7;">**题干**：10×10 棋盘，双人轮流落子，判断五子连珠胜负。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
char board[11][11];
void init()
{
    for (int i = 1; i <= 10; i++)
        for (int j = 1; j <= 10; j++)
            board[i][j] = '.';
}
void show()
{
    cout << "  1 2 3 4 5 6 7 8 9 10" << endl;
    for (int i = 1; i <= 10; i++)
    {
        if (i < 10) cout << ' ';
        cout << i << ' ';
        for (int j = 1; j <= 10; j++)
            cout << board[i][j] << ' ';
        cout << endl;
    }
}
bool win(int x, int y, char c)
{
    int dx[4] = {1, 1, 0, -1};
    int dy[4] = {0, 1, 1, 1};
    for (int k = 0; k < 4; k++)        // 四个方向
    {
        int cnt = 1;
        for (int d = 1; d <= 4; d++)   // 正方向数
        {
            int nx = x + dx[k] * d, ny = y + dy[k] * d;
            if (nx >= 1 && nx <= 10 && ny >= 1 && ny <= 10 && board[nx][ny] == c) cnt++;
            else break;
        }
        for (int d = 1; d <= 4; d++)   // 反方向数
        {
            int nx = x - dx[k] * d, ny = y - dy[k] * d;
            if (nx >= 1 && nx <= 10 && ny >= 1 && ny <= 10 && board[nx][ny] == c) cnt++;
            else break;
        }
        if (cnt >= 5) return true;     // 五子连珠
    }
    return false;
}
int main()
{
    init();
    char cur = 'X';
    int x, y, steps = 0;
    while (true)
    {
        show();
        cout << "玩家 " << cur << " 落子(行 列): ";
        cin >> x >> y;
        if (x < 1 || x > 10 || y < 1 || y > 10 || board[x][y] != '.')
        {
            cout << "无效落子，重新输入" << endl;
            continue;
        }
        board[x][y] = cur;
        steps++;
        if (win(x, y, cur))
        {
            cout << "玩家 " << cur << " 获胜！" << endl;
            break;
        }
        if (steps == 100) { cout << "平局" << endl; break; }
        cur = (cur == 'X') ? 'O' : 'X';
    }
    return 0;
}
```

</details>

---

##### 2.4.08 扫雷文字简化版

<div style="font-size:1.2em; line-height:1.7;">**题干**：二维数组存地图，随机布置地雷，点开格子显示周围雷数。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <cstdlib>
#include <ctime>
using namespace std;
int n = 9, mine, g[10][10];        // -1 表示地雷
bool opened[10][10];
void init()
{
    srand(time(0));
    for (int i = 1; i <= n; i++)
        for (int j = 1; j <= n; j++)
            g[i][j] = 0;
    int cnt = 0;
    while (cnt < mine)              // 随机布雷
    {
        int x = rand() % n + 1, y = rand() % n + 1;
        if (g[x][y] != -1) { g[x][y] = -1; cnt++; }
    }
    for (int i = 1; i <= n; i++)    // 计算周围雷数
        for (int j = 1; j <= n; j++)
        {
            if (g[i][j] == -1) continue;
            int s = 0;
            for (int di = -1; di <= 1; di++)
                for (int dj = -1; dj <= 1; dj++)
                {
                    int ni = i + di, nj = j + dj;
                    if (ni >= 1 && ni <= n && nj >= 1 && nj <= n && g[ni][nj] == -1) s++;
                }
            g[i][j] = s;
        }
}
void show()
{
    for (int i = 1; i <= n; i++)
    {
        for (int j = 1; j <= n; j++)
        {
            if (!opened[i][j]) cout << "* ";
            else if (g[i][j] == -1) cout << "@ ";
            else cout << g[i][j] << ' ';
        }
        cout << endl;
    }
}
int main()
{
    cout << "雷数: ";
    cin >> mine;
    init();
    int x, y, safe = n * n - mine;
    while (true)
    {
        show();
        cout << "点开格子(行 列): ";
        cin >> x >> y;
        if (x < 1 || x > n || y < 1 || y > n) continue;
        if (g[x][y] == -1) { cout << "踩雷！游戏结束" << endl; break; }
        opened[x][y] = true;
        safe--;
        if (safe == 0) { cout << "胜利！所有安全格已翻开" << endl; break; }
    }
    return 0;
}
```

</details>

---

##### 2.4.09 文字大富翁简化版

<div style="font-size:1.2em; line-height:1.7;">**题干**：多个玩家轮流掷骰子，前进格子，触发事件。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <cstdlib>
#include <ctime>
using namespace std;
int main()
{
    srand(time(0));
    int players, pos[4] = {0}, money[4] = {100};
    cout << "玩家数(2~4): ";
    cin >> players;
    while (true)
    {
        for (int p = 0; p < players; p++)
        {
            cout << "玩家" << p+1 << " 按回车掷骰子...";
            cin.get(); cin.get();
            int dice = rand() % 6 + 1;
            pos[p] = (pos[p] + dice) % 20;   // 20格环形地图
            money[p] += 10;                  // 每轮工资
            if (pos[p] % 5 == 0)             // 事件格
            {
                int e = rand() % 3;
                if (e == 0) { money[p] += 20; cout << "好运+20 "; }
                else if (e == 1) { money[p] -= 15; cout << "意外-15 "; }
                else cout << "无事发生 ";
            }
            cout << "玩家" << p+1 << " 位置" << pos[p]
                 << " 金钱" << money[p] << endl;
            if (money[p] <= 0)
            {
                cout << "玩家" << p+1 << " 破产出局！" << endl;
                return 0;
            }
        }
    }
    return 0;
}
```

</details>

---

##### 2.4.10 贪吃蛇文字版

<div style="font-size:1.2em; line-height:1.7;">**题干**：用字符模拟蛇移动、吃食物、撞墙死亡。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <cstdlib>
#include <ctime>
#include <conio.h>
using namespace std;
const int W = 20, H = 10;
int snakeX[400], snakeY[400], len = 3;
int foodX, foodY, dir = 1;   // 0上 1右 2下 3左
bool over = false;
void putFood()
{
    foodX = rand() % W;
    foodY = rand() % H;
}
void init()
{
    srand(time(0));
    snakeX[0] = 5; snakeY[0] = 5;
    snakeX[1] = 4; snakeY[1] = 5;
    snakeX[2] = 3; snakeY[2] = 5;
    putFood();
}
void draw()
{
    system("cls");
    for (int y = 0; y < H; y++)
    {
        for (int x = 0; x < W; x++)
        {
            bool isSnake = false;
            for (int i = 0; i < len; i++)
                if (snakeX[i] == x && snakeY[i] == y) isSnake = true;
            if (isSnake) cout << '#';
            else if (x == foodX && y == foodY) cout << '@';
            else cout << '.';
        }
        cout << endl;
    }
}
void move()
{
    int nx = snakeX[0], ny = snakeY[0];
    if (dir == 0) ny--;
    if (dir == 1) nx++;
    if (dir == 2) ny++;
    if (dir == 3) nx--;
    if (nx < 0 || nx >= W || ny < 0 || ny >= H) { over = true; return; }
    for (int i = 0; i < len; i++)
        if (snakeX[i] == nx && snakeY[i] == ny) { over = true; return; }
    for (int i = len - 1; i > 0; i--)
    {
        snakeX[i] = snakeX[i-1];
        snakeY[i] = snakeY[i-1];
    }
    snakeX[0] = nx; snakeY[0] = ny;
    if (nx == foodX && ny == foodY)
    {
        len++;
        snakeX[len-1] = snakeX[len-2];
        snakeY[len-1] = snakeY[len-2];
        putFood();
    }
}
int main()
{
    init();
    while (!over)
    {
        draw();
        if (kbhit())       // 有按键输入
        {
            char c = getch();
            if (c == 'w') dir = 0;
            if (c == 's') dir = 2;
            if (c == 'a') dir = 3;
            if (c == 'd') dir = 1;
        }
        move();
    }
    cout << "游戏结束，得分: " << len - 3 << endl;
    return 0;
}
```

</details>

---

##### 2.4.11 黑白棋（文字版奥赛罗）

<div style="font-size:1.2em; line-height:1.7;">**题干**：双人对战，落子翻转对方棋子，统计最终棋子数量。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
char b[9][9];
int dx[8] = {-1,-1,-1,0,0,1,1,1};
int dy[8] = {-1,0,1,-1,1,-1,0,1};
void init()
{
    for (int i = 1; i <= 8; i++)
        for (int j = 1; j <= 8; j++)
            b[i][j] = '.';
    b[4][4] = b[5][5] = 'O';
    b[4][5] = b[5][4] = 'X';
}
bool canPut(int x, int y, char c)
{
    if (b[x][y] != '.') return false;
    char op = (c == 'X') ? 'O' : 'X';
    for (int k = 0; k < 8; k++)
    {
        int nx = x + dx[k], ny = y + dy[k];
        bool found = false;
        while (nx >= 1 && nx <= 8 && ny >= 1 && ny <= 8 && b[nx][ny] == op)
        {
            nx += dx[k]; ny += dy[k];
            if (nx >= 1 && nx <= 8 && ny >= 1 && ny <= 8 && b[nx][ny] == c)
                found = true;
        }
        if (found) return true;   // 至少能夹住一个对方棋子
    }
    return false;
}
void flip(int x, int y, char c)
{
    char op = (c == 'X') ? 'O' : 'X';
    for (int k = 0; k < 8; k++)
    {
        int nx = x + dx[k], ny = y + dy[k];
        bool found = false;
        while (nx >= 1 && nx <= 8 && ny >= 1 && ny <= 8 && b[nx][ny] == op)
        {
            nx += dx[k]; ny += dy[k];
            if (nx >= 1 && nx <= 8 && ny >= 1 && ny <= 8 && b[nx][ny] == c)
                found = true;
        }
        if (found)                 // 一路翻过去
        {
            nx = x + dx[k]; ny = y + dy[k];
            while (b[nx][ny] == op)
            {
                b[nx][ny] = c;
                nx += dx[k]; ny += dy[k];
            }
        }
    }
}
void show()
{
    for (int i = 1; i <= 8; i++)
    {
        for (int j = 1; j <= 8; j++) cout << b[i][j] << ' ';
        cout << endl;
    }
}
int main()
{
    init();
    char cur = 'X';
    for (int round = 0; round < 32; round++)
    {
        show();
        int x, y;
        cout << "玩家 " << cur << " 落子(行 列): ";
        cin >> x >> y;
        if (!canPut(x, y, cur)) { cout << "无效落子" << endl; round--; continue; }
        b[x][y] = cur;
        flip(x, y, cur);
        cur = (cur == 'X') ? 'O' : 'X';
    }
    int cntX = 0, cntO = 0;
    for (int i = 1; i <= 8; i++)
        for (int j = 1; j <= 8; j++)
        {
            if (b[i][j] == 'X') cntX++;
            if (b[i][j] == 'O') cntO++;
        }
    cout << "X: " << cntX << " O: " << cntO << " ";
    if (cntX > cntO) cout << "X胜" << endl;
    else if (cntX < cntO) cout << "O胜" << endl;
    else cout << "平局" << endl;
    return 0;
}
```

</details>

---

##### 2.4.12 猜词游戏（Hangman 绞刑架）

<div style="font-size:1.2em; line-height:1.7;">**题干**：程序随机选单词，玩家猜字母，猜错次数有限。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <string>
#include <cstdlib>
#include <ctime>
using namespace std;
int main()
{
    srand(time(0));
    string words[10] = {"apple", "banana", "computer", "school", "happy",
                        "window", "flower", "river", "mountain", "star"};
    string word = words[rand() % 10];
    string show = string(word.size(), '_');
    int chance = 6;                    // 最多错6次
    while (chance > 0)
    {
        cout << "当前: " << show << "  剩余机会: " << chance << "  猜一个字母: ";
        char c;
        cin >> c;
        bool found = false;
        for (int i = 0; i < word.size(); i++)
            if (word[i] == c && show[i] == '_')
            {
                show[i] = c;
                found = true;
            }
        if (!found) chance--;
        if (show == word)
        {
            cout << "猜对了！单词是: " << word << endl;
            return 0;
        }
    }
    cout << "机会用尽，单词是: " << word << endl;
    return 0;
}
```

</details>

---

##### 2.4.13 井字棋人机对战

<div style="font-size:1.2em; line-height:1.7;">**题干**：3×3 棋盘，玩家和电脑对战，电脑简单 AI 落子。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <cstdlib>
#include <ctime>
using namespace std;
char b[3][3];
void init()
{
    for (int i = 0; i < 3; i++)
        for (int j = 0; j < 3; j++)
            b[i][j] = ' ';
}
void show()
{
    for (int i = 0; i < 3; i++)
    {
        cout << " " << b[i][0] << " | " << b[i][1] << " | " << b[i][2] << endl;
        if (i < 2) cout << "---+---+---" << endl;
    }
}
bool win(char c)
{
    for (int i = 0; i < 3; i++)
    {
        if (b[i][0] == c && b[i][1] == c && b[i][2] == c) return true;
        if (b[0][i] == c && b[1][i] == c && b[2][i] == c) return true;
    }
    return (b[0][0] == c && b[1][1] == c && b[2][2] == c) ||
           (b[0][2] == c && b[1][1] == c && b[2][0] == c);
}
int main()
{
    srand(time(0));
    init();
    int moves = 0, x, y;
    while (moves < 9)
    {
        show();
        cout << "你的回合(行 列): ";
        cin >> x >> y;
        if (b[x][y] != ' ') { cout << "已有棋子" << endl; continue; }
        b[x][y] = 'X';               // 玩家
        moves++;
        if (win('X')) { show(); cout << "你赢了！" << endl; return 0; }
        if (moves == 9) break;
        while (true)                 // 电脑随机空位
        {
            int i = rand() % 3, j = rand() % 3;
            if (b[i][j] == ' ') { b[i][j] = 'O'; break; }
        }
        moves++;
        if (win('O')) { show(); cout << "电脑赢了！" << endl; return 0; }
    }
    show();
    cout << "平局" << endl;
    return 0;
}
```

</details>

---

##### 2.4.14 卡牌对战小游戏

<div style="font-size:1.2em; line-height:1.7;">**题干**：多组卡牌，攻击血量，随机抽卡，回合制战斗。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <string>
#include <cstdlib>
#include <ctime>
using namespace std;
struct Card
{
    string name;
    int attack, hp;
};
int main()
{
    srand(time(0));
    Card deck[5] = {{"火球", 8, 5}, {"冰霜", 6, 8}, {"闪电", 10, 3},
                    {"岩石", 5, 12}, {"风刃", 7, 6}};
    int myHp = 30, enemyHp = 30;
    while (myHp > 0 && enemyHp > 0)
    {
        Card mine = deck[rand() % 5];
        Card enemy = deck[rand() % 5];
        cout << "我方出 " << mine.name << "(" << mine.attack << "/" << mine.hp
             << ")  vs  敌方出 " << enemy.name << "(" << enemy.attack << "/"
             << enemy.hp << ")" << endl;
        enemyHp -= mine.attack;
        myHp -= enemy.attack;
        cout << "我方HP: " << myHp << "  敌方HP: " << enemyHp << endl;
        cout << "按回车继续...";
        cin.get(); cin.get();
    }
    if (myHp > 0) cout << "你赢了！" << endl;
    else cout << "你输了！" << endl;
    return 0;
}
```

</details>

---

#### ▸ 小类 C：实用小工具

##### 2.4.15 24 点小游戏

<div style="font-size:1.2em; line-height:1.7;">**题干**：随机生成 4 个 1~13 数字，玩家输入表达式，判断能否算出 24。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <cstdlib>
#include <ctime>
using namespace std;
bool near24(double x) { return x > 23.99 && x < 24.01; }
bool dfs(double nums[], int cnt)
{
    if (cnt == 1) return near24(nums[0]);
    double nxt[4];
    for (int i = 0; i < cnt; i++)
        for (int j = 0; j < cnt; j++)
        {
            if (i == j) continue;
            int t = 0;
            for (int k = 0; k < cnt; k++)
                if (k != i && k != j) nxt[t++] = nums[k];
            double x = nums[i], y = nums[j];
            nxt[t] = x + y; if (dfs(nxt, t + 1)) return true;
            nxt[t] = x - y; if (dfs(nxt, t + 1)) return true;
            nxt[t] = x * y; if (dfs(nxt, t + 1)) return true;
            if (y != 0) { nxt[t] = x / y; if (dfs(nxt, t + 1)) return true; }
        }
    return false;
}
int main()
{
    srand(time(0));
    double nums[4];
    for (int i = 0; i < 4; i++) nums[i] = rand() % 13 + 1;
    cout << "随机数字: ";
    for (int i = 0; i < 4; i++) cout << nums[i] << ' ';
    cout << endl;
    cout << (dfs(nums, 4) ? "可以算出24" : "算不出24") << endl;
    return 0;
}
```

</details>

---

##### 2.4.16 单词背诵工具

<div style="font-size:1.2em; line-height:1.7;">**题干**：文件存储单词 + 释义；随机出题，答错加入错题本。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <fstream>
#include <string>
#include <cstdlib>
#include <ctime>
using namespace std;
string words[100], means[100];
int n = 0;
void load()
{
    ifstream fin("words.txt");
    while (fin >> words[n] >> means[n]) n++;
    fin.close();
}
void save()
{
    ofstream fout("words.txt");
    for (int i = 0; i < n; i++)
        fout << words[i] << ' ' << means[i] << endl;
    fout.close();
}
int main()
{
    srand(time(0));
    load();
    int choice;
    while (true)
    {
        cout << "1新增 2随机出题 3显示全部 4退出: ";
        cin >> choice;
        if (choice == 1)
        {
            cout << "单词 释义: ";
            cin >> words[n] >> means[n];
            n++;
            save();
        }
        else if (choice == 2)
        {
            if (n == 0) { cout << "还没有单词" << endl; continue; }
            int idx = rand() % n;
            string ans;
            cout << "释义: " << means[idx] << " 对应的单词: ";
            cin >> ans;
            if (ans == words[idx]) cout << "答对了！" << endl;
            else
            {
                cout << "答错了，正确答案: " << words[idx] << endl;
                ofstream fout("错题本.txt", ios::app);   // 加入错题本
                fout << words[idx] << ' ' << means[idx] << endl;
                fout.close();
            }
        }
        else if (choice == 3)
        {
            for (int i = 0; i < n; i++)
                cout << words[i] << " - " << means[i] << endl;
        }
        else break;
    }
    return 0;
}
```

</details>

---

##### 2.4.17 记账本程序

<div style="font-size:1.2em; line-height:1.7;">**题干**：记录收支，分类统计，支持查看总余额、导出记录到文本。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <fstream>
#include <string>
using namespace std;
string type[1000], note[1000];
double money[1000];
int n = 0;
int main()
{
    ifstream fin("records.txt");
    while (fin >> type[n] >> money[n] >> note[n]) n++;
    fin.close();
    int choice;
    while (true)
    {
        cout << "1记一笔 2查看统计 3导出 4退出: ";
        cin >> choice;
        if (choice == 1)
        {
            cout << "类型(in/out) 金额 说明: ";
            cin >> type[n] >> money[n] >> note[n];
            n++;
            ofstream fout("records.txt", ios::app);
            fout << type[n-1] << ' ' << money[n-1] << ' ' << note[n-1] << endl;
            fout.close();
        }
        else if (choice == 2)
        {
            double inSum = 0, outSum = 0;
            for (int i = 0; i < n; i++)
                if (type[i] == "in") inSum += money[i];
                else outSum += money[i];
            cout << "总收入: " << inSum << " 总支出: " << outSum
                 << " 余额: " << inSum - outSum << endl;
        }
        else if (choice == 3)
        {
            ofstream fout("账单导出.txt");
            for (int i = 0; i < n; i++)
                fout << type[i] << ' ' << money[i] << ' ' << note[i] << endl;
            fout.close();
            cout << "已导出到 账单导出.txt" << endl;
        }
        else break;
    }
    return 0;
}
```

</details>

---

##### 2.4.18 图片字符画转换器

<div style="font-size:1.2em; line-height:1.7;">**题干**：读取文本灰度矩阵，输出字符画（纯文本版本）。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <fstream>
using namespace std;
int main()
{
    ifstream fin("gray.txt");   // 第一行: 宽 高，之后是灰度值 0~255
    int w, h;
    fin >> w >> h;
    string chars = " .:-=+*#%@";   // 由浅到深的10级字符
    for (int i = 0; i < h; i++)
    {
        for (int j = 0; j < w; j++)
        {
            int v;
            fin >> v;
            cout << chars[v * 9 / 256];   // 灰度映射到字符下标
        }
        cout << endl;
    }
    fin.close();
    return 0;
}
```

</details>

---

##### 2.4.19 文件单词统计工具

<div style="font-size:1.2em; line-height:1.7;">**题干**：读取 txt 文件，统计总单词数、行数、字符数。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <fstream>
#include <string>
using namespace std;
int main()
{
    ifstream fin("words.txt");
    string w;
    int cnt=0;
    while(fin >> w) cnt++;
    fin.close();
    cout << cnt << endl;
    return 0;
}
```

</details>

---

##### 2.4.20 批量文本替换工具

<div style="font-size:1.2em; line-height:1.7;">**题干**：读取 txt，替换指定关键词，保存成新文件。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <fstream>
#include <string>
using namespace std;
int main()
{
    string src, oldW, newW;
    cout << "输入源文件名: ";
    cin >> src;
    cout << "替换前关键词: ";
    cin >> oldW;
    cout << "替换后关键词: ";
    cin >> newW;
    ifstream fin(src.c_str());
    string content = "", line;
    while (getline(fin, line))
        content += line + "\n";
    fin.close();
    size_t pos = 0;
    while ((pos = content.find(oldW, pos)) != string::npos)   // 逐个替换
    {
        content.replace(pos, oldW.size(), newW);
        pos += newW.size();
    }
    ofstream fout("output.txt");
    fout << content;
    fout.close();
    cout << "已保存到 output.txt" << endl;
    return 0;
}
```

</details>

---

##### 2.4.21 迷宫 DFS 寻路

<div style="font-size:1.2em; line-height:1.7;">**题干**：二维字符迷宫，程序自动寻找从起点到终点路径并输出路线。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
char mp[105][105];
int n,m;
bool ok;
int dx[]={1,-1,0,0};
int dy[]={0,0,1,-1};
void dfs(int x,int y)
{
    if(mp[x][y] == 'T') {ok=true;return;}
    mp[x][y]='#';
    for(int d=0;d<4;d++)
    {
        int nx=x+dx[d], ny=y+dy[d];
        if(nx>=0&&nx<n&&ny>=0&&ny<m && mp[nx][ny]!='#')
        {
            dfs(nx,ny);
        }
    }
}
int main()
{
    cin >> n >> m;
    int sx,sy;
    for(int i=0;i<n;i++)
    {
        for(int j=0;j<m;j++)
        {
            cin >> mp[i][j];
            if(mp[i][j]=='S') sx=i,sy=j;
        }
    }
    ok=false;
    dfs(sx,sy);
    if(ok) cout << "YES";
    else cout << "NO";
    return 0;
}
```

</details>

---

##### 2.4.22 抽奖名单工具

<div style="font-size:1.2em; line-height:1.7;">**题干**：读取名单 txt，随机抽取 N 名获奖者，不重复抽取。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <fstream>
#include <string>
#include <cstdlib>
#include <ctime>
#include <algorithm>
using namespace std;
int main()
{
    srand(time(0));
    string names[100];
    int n = 0, k;
    ifstream fin("names.txt");
    while (fin >> names[n]) n++;
    fin.close();
    cout << "共" << n << "人，抽取人数: ";
    cin >> k;
    if (k > n) k = n;
    for (int t = 0; t < k; t++)
    {
        int idx = rand() % (n - t);          // 从未抽取范围取
        cout << names[idx] << endl;
        swap(names[idx], names[n - 1 - t]);  // 已抽的移到末尾
    }
    return 0;
}
```

</details>

---

##### 2.4.23 加密记事本

<div style="font-size:1.2em; line-height:1.7;">**题干**：写入文本，凯撒加密保存到文件，读取时解密。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <fstream>
#include <string>
using namespace std;
string encrypt(string s, int shift)
{
    for (int i = 0; i < s.size(); i++)
    {
        char c = s[i];
        if (c >= 'a' && c <= 'z') c = 'a' + (c - 'a' + shift) % 26;
        else if (c >= 'A' && c <= 'Z') c = 'A' + (c - 'A' + shift) % 26;
        s[i] = c;
    }
    return s;
}
int main()
{
    int choice;
    cout << "1加密写入 2读取解密: ";
    cin >> choice;
    cin.ignore();
    if (choice == 1)
    {
        cout << "输入内容: ";
        string s;
        getline(cin, s);
        ofstream fout("secret.txt");
        fout << encrypt(s, 3);     // 凯撒加密后保存
        fout.close();
        cout << "已加密保存" << endl;
    }
    else
    {
        ifstream fin("secret.txt");
        string s;
        getline(fin, s);
        fin.close();
        cout << "解密内容: " << encrypt(s, 23) << endl;   // 反向偏移3
    }
    return 0;
}
```

</details>

---

##### 2.4.24 石头剪刀布积分联赛

<div style="font-size:1.2em; line-height:1.7;">**题干**：多轮对战，记录总分，历史对局保存文件。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <fstream>
#include <string>
#include <cstdlib>
#include <ctime>
using namespace std;
int main()
{
    srand(time(0));
    int myScore = 0, compScore = 0, round = 0;
    string names[4] = {"", "石头", "剪刀", "布"};
    while (true)
    {
        round++;
        cout << "第" << round << "局: 1石头 2剪刀 3布 0退出: ";
        int me;
        cin >> me;
        if (me == 0) break;
        int comp = rand() % 3 + 1;
        cout << "电脑出: " << names[comp] << endl;
        if (me == comp) cout << "平局" << endl;
        else if ((me == 1 && comp == 2) || (me == 2 && comp == 3) || (me == 3 && comp == 1))
        {
            cout << "你赢了！" << endl;
            myScore++;
        }
        else
        {
            cout << "电脑赢了" << endl;
            compScore++;
        }
        cout << "比分: " << myScore << " : " << compScore << endl;
        ofstream fout("history.txt", ios::app);
        fout << "第" << round << "局 我出" << names[me] << " 电脑出" << names[comp] << endl;
        fout.close();
    }
    cout << "最终比分: " << myScore << " : " << compScore << endl;
    if (myScore > compScore) cout << "你获得胜利！" << endl;
    else if (myScore < compScore) cout << "电脑获胜" << endl;
    else cout << "平局收场" << endl;
    return 0;
}
```

</details>

---

##### 2.4.25 综合大项目

<div style="font-size:1.2em; line-height:1.7;">**题干**：文字 RPG 冒险：玩家角色（血量、攻击力），多房间地图，怪物战斗、拾取道具，存档读档。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <fstream>
#include <string>
#include <cstdlib>
#include <ctime>
using namespace std;
struct Player
{
    string name;
    int hp, attack, gold;
};
struct Monster
{
    string name;
    int hp, attack;
};
int main()
{
    srand(time(0));
    Player p;
    cout << "输入角色名: ";
    cin >> p.name;
    p.hp = 100; p.attack = 15; p.gold = 0;
    // 简易地图：3个房间，可能遇到怪物或宝箱
    for (int room = 1; room <= 3 && p.hp > 0; room++)
    {
        cout << "\n===== 房间 " << room << " =====" << endl;
        int event = rand() % 2;
        if (event == 0)
        {
            Monster m;
            m.name = (rand() % 2) ? "哥布林" : "骷髅";
            m.hp = 20 + rand() % 20;
            m.attack = 5 + rand() % 8;
            cout << "遇到怪物 " << m.name << "(" << m.hp << "/" << m.attack << ")!" << endl;
            while (p.hp > 0 && m.hp > 0)
            {
                m.hp -= p.attack;
                if (m.hp > 0) p.hp -= m.attack;
                cout << "你攻击，怪物剩 " << m.hp << " HP；你剩 " << p.hp << " HP" << endl;
            }
            if (p.hp <= 0) break;
            p.gold += 20;
            cout << "击败怪物！获得 20 金币" << endl;
        }
        else
        {
            int g = 10 + rand() % 20;
            p.gold += g;
            cout << "发现宝箱！获得 " << g << " 金币" << endl;
        }
        if (room < 3)
        {
            cout << "按回车进入下一房间...";
            cin.get(); cin.get();
        }
    }
    if (p.hp <= 0)
        cout << p.name << " 倒下了...游戏结束" << endl;
    else
    {
        cout << "\n===== 通关！ =====" << endl;
        cout << p.name << " 剩余HP: " << p.hp << " 金币: " << p.gold << endl;
        ofstream fout("save.txt");          // 存档
        fout << p.name << " " << p.hp << " " << p.gold << endl;
        fout.close();
        cout << "已存档到 save.txt" << endl;
    }
    return 0;
}
```

</details>

---

## 第3类 · 竞赛入门 ｜ 第三套 · CSP-J算法入门100题

> 难度：★★★☆☆

### 3.1 模拟（模拟题）

#### ▸ 小类 A：数字与日期处理

##### 3.1.01 数字翻转

<div style="font-size:1.2em; line-height:1.7;">**题干**：给定整数 n，输出将其各位数字翻转后的数，前导零不要输出。例：输入 120，输出 21。</div>

**样例**：

```text
输入整数，反转输出，如输入1234，输出4321
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int x,rev=0;
    cin >> x;
    while(x>0)
    {
        rev = rev*10 + x%10;
        x /=10;
    }
    cout << rev;
    return 0;
}
```

</details>

---

##### 3.1.02 日期天数

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入年、月、日，输出这一天是当年的第几天。需要处理闰年。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
bool isLeap(int y)
{
    return (y % 4 == 0 && y % 100 != 0) || y % 400 == 0;
}
int main()
{
    int y, m, d;
    cin >> y >> m >> d;
    int days[13] = {0,31,28,31,30,31,30,31,31,30,31,30,31};
    if (isLeap(y)) days[2] = 29;   // 闰年2月29天
    int sum = 0;
    for (int i = 1; i < m; i++) sum += days[i];
    sum += d;
    cout << sum;
    return 0;
}
```

</details>

---

##### 3.1.03 时间换算

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入总秒数，转换成 时:分:秒 格式输出。</div>

**样例**：

```text
输入总秒数s，换算h:m:s。 样例输入：3661 输出：1 1 1
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int s;
    cin >> s;
    int h = s / 3600;
    int m = (s % 3600)/60;
    int sec = s % 60;
    cout << h << " " << m << " " << sec;
    return 0;
}
```

</details>

---

##### 3.1.04 日期加减

<div style="font-size:1.2em; line-height:1.7;">**题干**：给定年月日，增加 k 天，输出新的年月日。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
bool isLeap(int y)
{
    return (y % 4 == 0 && y % 100 != 0) || y % 400 == 0;
}
int main()
{
    int y, m, d, k;
    cin >> y >> m >> d >> k;
    int days[13] = {0,31,28,31,30,31,30,31,31,30,31,30,31};
    while (k > 0)
    {
        int dim = days[m];          // 本月天数
        if (m == 2 && isLeap(y)) dim = 29;
        if (d < dim) { d++; k--; }
        else if (m < 12) { d = 1; m++; k--; }
        else { d = 1; m = 1; y++; k--; }
    }
    cout << y << " " << m << " " << d;
    return 0;
}
```

</details>

---

##### 3.1.05 进制转换 1

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入十进制整数，转为二进制字符串输出。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <string>
using namespace std;
int main()
{
    int n;
    cin >> n;
    if (n == 0) { cout << 0; return 0; }
    string s = "";
    while (n > 0)
    {
        s = char('0' + n % 2) + s;
        n /= 2;
    }
    cout << s;
    return 0;
}
```

</details>

---

##### 3.1.06 进制转换 2

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入二进制字符串，转为十进制整数。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <string>
using namespace std;
int main()
{
    string s;
    cin >> s;
    int ans = 0;
    for (int i = 0; i < s.size(); i++)
        ans = ans * 2 + (s[i] - '0');
    cout << ans;
    return 0;
}
```

</details>

---

##### 3.1.07 罗马数字转整数

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入合法罗马字符串，输出对应阿拉伯数字。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <string>
using namespace std;
int val(char c)
{
    if (c == 'I') return 1;
    if (c == 'V') return 5;
    if (c == 'X') return 10;
    if (c == 'L') return 50;
    if (c == 'C') return 100;
    if (c == 'D') return 500;
    return 1000;   // M
}
int main()
{
    string s;
    cin >> s;
    int ans = 0;
    for (int i = 0; i < s.size(); i++)
    {
        if (i + 1 < s.size() && val(s[i]) < val(s[i+1]))
            ans -= val(s[i]);   // 小在前：如 IV = 4
        else
            ans += val(s[i]);
    }
    cout << ans;
    return 0;
}
```

</details>

---

##### 3.1.08 整数转罗马数字

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入 1~3999 整数，输出罗马字符串。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <string>
using namespace std;
int main()
{
    int n;
    cin >> n;   // 1~3999
    string s = "";
    int num[13] = {1000,900,500,400,100,90,50,40,10,9,5,4,1};
    string rom[13] = {"M","CM","D","CD","C","XC","L","XL","X","IX","V","IV","I"};
    for (int i = 0; i < 13; i++)
        while (n >= num[i])
        {
            s += rom[i];
            n -= num[i];
        }
    cout << s;
    return 0;
}
```

</details>

---

#### ▸ 小类 B：统计与枚举

##### 3.1.09 成绩统计

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入 n 个分数，输出最高分、最低分、平均分。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int x,maxs=0,mins=1000,sum=0,cnt=0;
    while(cin >> x)
    {
        if(x == -1) break;
        cnt++;
        sum +=x;
        if(x>maxs) maxs=x;
        if(x<mins) mins=x;
    }
    cout << "最高分：" << maxs << "最低分：" << mins << "平均分：" << 1.0*sum/cnt;
    return 0;
}
```

</details>

---

##### 3.1.10 文字版计数器

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入一行字符，分别统计大写字母、小写字母、数字、空格、其他符号数量。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <string>
using namespace std;
int main()
{
    string a,b;
    cin >> a >> b;
    if(a > b) cout << a << "更大";
    else if(a < b) cout << b << "更大";
    else cout << "相等";
    return 0;
}
```

</details>

---

##### 3.1.11 购物找零

<div style="font-size:1.2em; line-height:1.7;">**题干**：商品价格，用户付款金额，按面额从大到小输出每种纸币找零数量。面额：100,50,20,10,5,1。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int price, pay;
    cin >> price >> pay;
    int change = pay - price;
    int m[6] = {100, 50, 20, 10, 5, 1};
    for (int i = 0; i < 6; i++)   // 从大面额开始
    {
        int cnt = change / m[i];
        if (cnt > 0)
            cout << m[i] << "元: " << cnt << "张 ";
        change %= m[i];
    }
    return 0;
}
```

</details>

---

#### ▸ 小类 C：过程与规则模拟

##### 3.1.12 奇数偶数分离

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入 n 个整数，先输出全部奇数，再输出全部偶数。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <vector>
using namespace std;
int main()
{
    int n; cin >> n;
    vector<int> v,odd,even;
    for(int i=0;i<n;i++)
    {
        int x; cin >> x;
        v.push_back(x);
        if(x%2==0) even.push_back(x);
        else odd.push_back(x);
    }
    cout << "奇数："; for(auto x:odd) cout << x << " ";
    cout << "\n偶数："; for(auto x:even) cout << x << " ";
    return 0;
}
```

</details>

---

##### 3.1.13 卡牌游戏

<div style="font-size:1.2em; line-height:1.7;">**题干**：n 张牌排成一圈，从第 1 张开始，每次数到第 k 张拿走，模拟直到拿完，输出拿走顺序（约瑟夫环模拟小数据）。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int n, k;
    cin >> n >> k;
    bool out[100] = {false};       // 是否已拿走
    int cnt = 0, idx = 0;          // 拿走张数、当前下标
    while (cnt < n)
    {
        int step = 0;
        while (step < k)           // 数到第k张
        {
            if (!out[idx]) step++;
            idx = (idx + 1) % n;
        }
        idx = (idx - 1 + n) % n;   // 回退到第k张
        out[idx] = true;
        cnt++;
        cout << idx + 1 << ' ';    // 拿走顺序
        idx = (idx + 1) % n;       // 从下一张继续数
    }
    return 0;
}
```

</details>

---

##### 3.1.14 字符串压缩

<div style="font-size:1.2em; line-height:1.7;">**题干**：连续相同字符缩写，aaabbbcc → a3b3c2。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <string>
using namespace std;
int main()
{
    string s;
    cin >> s;
    for (int i = 0; i < s.size(); )
    {
        int j = i;
        while (j < s.size() && s[j] == s[i]) j++;   // 连续相同
        cout << s[i] << j - i;
        i = j;
    }
    return 0;
}
```

</details>

---

##### 3.1.15 解压字符串

<div style="font-size:1.2em; line-height:1.7;">**题干**：a3b2 还原为 aaabb。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <string>
using namespace std;
int main()
{
    string s;
    cin >> s;
    for (int i = 0; i < s.size(); i++)
    {
        char c = s[i];
        int num = 0;
        while (i + 1 < s.size() && s[i+1] >= '0' && s[i+1] <= '9')
        {
            num = num * 10 + (s[i+1] - '0');
            i++;
        }
        if (num == 0) num = 1;      // 没有数字就输出1个
        for (int k = 0; k < num; k++) cout << c;
    }
    return 0;
}
```

</details>

---

##### 3.1.16 火车进站模拟

<div style="font-size:1.2em; line-height:1.7;">**题干**：给定入栈序列，判断出栈序列是否合法（小数据）。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <stack>
using namespace std;
int main()
{
    int n, in[100], out[100];
    cin >> n;
    for (int i = 0; i < n; i++) cin >> in[i];    // 入栈序列
    for (int i = 0; i < n; i++) cin >> out[i];   // 出栈序列
    stack<int> st;
    int j = 0;
    for (int i = 0; i < n; i++)
    {
        st.push(in[i]);                          // 火车进站
        while (!st.empty() && st.top() == out[j])
        {
            st.pop();                            // 匹配出站
            j++;
        }
    }
    cout << (st.empty() ? "合法" : "不合法");
    return 0;
}
```

</details>

---

##### 3.1.17 红绿灯模拟

<div style="font-size:1.2em; line-height:1.7;">**题干**：红灯 30 秒，绿灯 25 秒，黄灯 5 秒，输入总秒数，输出当前灯颜色。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int t;
    cin >> t;              // 总秒数
    int cycle = 30 + 25 + 5;   // 红30 绿25 黄5
    t %= cycle;
    if (t < 30) cout << "红灯";
    else if (t < 55) cout << "绿灯";
    else cout << "黄灯";
    return 0;
}
```

</details>

---

##### 3.1.18 螺旋矩阵

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入 n，输出 \(n\times n\) 顺时针螺旋填充矩阵。例 n=3： 1 2 3 8 9 4 7 6 5</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int n, a[20][20] = {0};
    cin >> n;
    int num = 1, top = 0, bottom = n - 1, left = 0, right = n - 1;
    while (num <= n * n)
    {
        for (int j = left; j <= right; j++) a[top][j] = num++;
        top++;
        for (int i = top; i <= bottom; i++) a[i][right] = num++;
        right--;
        for (int j = right; j >= left; j--) a[bottom][j] = num++;
        bottom--;
        for (int i = bottom; i >= top; i--) a[i][left] = num++;
        left++;
    }
    for (int i = 0; i < n; i++)
    {
        for (int j = 0; j < n; j++)
            cout << a[i][j] << ' ';
        cout << endl;
    }
    return 0;
}
```

</details>

---

##### 3.1.19 多项式加法

<div style="font-size:1.2em; line-height:1.7;">**题干**：两个一元多项式，用数组保存系数，输出相加后的多项式。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int n, m, x, c;
    int coef[101] = {0};      // 下标为次数
    cin >> n;
    for (int i = 0; i < n; i++)
    {
        cin >> x >> c;        // 次数 系数
        coef[x] += c;
    }
    cin >> m;
    for (int i = 0; i < m; i++)
    {
        cin >> x >> c;
        coef[x] += c;
    }
    bool first = true;
    for (int i = 100; i >= 0; i--)
        if (coef[i] != 0)
        {
            if (!first) cout << " + ";
            cout << coef[i];
            if (i > 0) cout << "x^" << i;
            first = false;
        }
    return 0;
}
```

</details>

---

##### 3.1.20 简单计算器

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入表达式只有 + - * 和整数，无括号，计算结果。</div>

**样例**：

```text
输入a op b，op是+ - * /，输出结果；除法为实数，保留2位。 样例输入：6 / 2 →3.00
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <iomanip>
using namespace std;
int main()
{
    double a,b;
    char op;
    cin >> a >> op >> b;
    double ans;
    if(op == '+') ans = a+b;
    else if(op == '-') ans = a-b;
    else if(op == '*') ans = a*b;
    else ans = a/b;
    cout << fixed << setprecision(2) << ans;
    return 0;
}
```

</details>

---

### 3.2 字符串专题（字符串专题）

#### ▸ 小类 A：模式与统计

##### 3.2.01 字符串最大连续相同字符

<div style="font-size:1.2em; line-height:1.7;">**题干**：找出最长连续相同字符，输出字符和长度。例如aaabbaaaaa得到a 5。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <string>
using namespace std;
int main()
{
    string s;
    cin >> s;
    int maxlen = 1,now=1;
    for(int i=1;i<s.size();i++)
    {
        if(s[i]==s[i-1]) now++;
        else now=1;
        if(now>maxlen) maxlen=now;
    }
    cout << maxlen;
    return 0;
}
```

</details>

---

##### 3.2.02 子串出现次数

<div style="font-size:1.2em; line-height:1.7;">**题干**：给定母串与子串，统计子串在母串中一共出现多少次（可重叠）。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <string>
using namespace std;
int main()
{
    string s, sub;
    cin >> s >> sub;
    int cnt=0;
    size_t pos = 0;
    while( (pos = s.find(sub,pos)) != string::npos )
    {
        cnt++;
        pos += sub.size();
    }
    cout << cnt << endl;
    return 0;
}
```

</details>

---

##### 3.2.03 最长回文子串

<div style="font-size:1.2em; line-height:1.7;">**题干**：给定字符串，找出长度最长的回文子串（暴力枚举版本）。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <string>
using namespace std;
bool isPalin(string s)
{
    for (int i = 0, j = s.size() - 1; i < j; i++, j--)
        if (s[i] != s[j]) return false;
    return true;
}
int main()
{
    string s, best = "";
    cin >> s;
    for (int i = 0; i < s.size(); i++)          // 起点
        for (int j = i; j < s.size(); j++)      // 终点
        {
            string sub = s.substr(i, j - i + 1);
            if (isPalin(sub) && sub.size() > best.size())
                best = sub;
        }
    cout << best;
    return 0;
}
```

</details>

---

##### 3.2.04 字符串相似度

<div style="font-size:1.2em; line-height:1.7;">**题干**：两个等长字符串，统计对应位置字符不同的个数（汉明距离）。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <string>
using namespace std;
int main()
{
    string a, b;
    cin >> a >> b;
    int diff = 0;
    for (int i = 0; i < a.size(); i++)   // 两个等长字符串
        if (a[i] != b[i]) diff++;
    cout << diff;
    return 0;
}
```

</details>

---

##### 3.2.05 密码校验

<div style="font-size:1.2em; line-height:1.7;">**题干**：密码满足：长度≥6，至少包含大写、小写、数字三类中的两类。输出合法 / 不合法。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <string>
using namespace std;
int main()
{
    string s;
    cin >> s;
    bool hasUpper=false, hasLower=false, hasDigit=false;
    for(auto ch : s)
    {
        if(ch>='A'&&ch<='Z') hasUpper=true;
        else if(ch>='a'&&ch<='z') hasLower=true;
        else if(ch>='0'&&ch<='9') hasDigit=true;
    }
    if(s.size()>=6 && hasUpper && hasLower && hasDigit)
        cout << "强密码";
    else cout << "弱密码";
    return 0;
}
```

</details>

---

#### ▸ 小类 B：括号与结构

##### 3.2.06 括号序列判定

<div style="font-size:1.2em; line-height:1.7;">**题干**：只含(和)，判断括号序列是否合法。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <string>
using namespace std;
int main()
{
    string s;
    cin >> s;
    int cnt = 0;                 // 未配对的左括号数
    bool ok = true;
    for (int i = 0; i < s.size(); i++)
    {
        if (s[i] == '(') cnt++;
        else
        {
            cnt--;
            if (cnt < 0) { ok = false; break; }
        }
    }
    if (cnt != 0) ok = false;
    cout << (ok ? "YES" : "NO");
    return 0;
}
```

</details>

---

##### 3.2.07 括号序列加强版

<div style="font-size:1.2em; line-height:1.7;">**题干**：含()[]，判断括号是否匹配。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <string>
#include <stack>
using namespace std;
int main()
{
    string s;
    cin >> s;
    stack<char> st;
    bool ok = true;
    for (int i = 0; i < s.size(); i++)
    {
        if (s[i] == '(' || s[i] == '[')
            st.push(s[i]);
        else
        {
            if (st.empty()) { ok = false; break; }
            char c = st.top();
            if ((s[i] == ')' && c == '(') || (s[i] == ']' && c == '['))
                st.pop();
            else { ok = false; break; }
        }
    }
    if (!st.empty()) ok = false;
    cout << (ok ? "YES" : "NO");
    return 0;
}
```

</details>

---

#### ▸ 小类 C：变换与比较

##### 3.2.08 单词翻转

<div style="font-size:1.2em; line-height:1.7;">**题干**：一句话，翻转每个单词内部字母，单词顺序不变。hello world → olleh dlrow。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <string>
using namespace std;
int main()
{
    string s;
    getline(cin, s);
    string w = "";
    for (int i = 0; i <= s.size(); i++)
    {
        if (i == s.size() || s[i] == ' ')
        {
            for (int j = w.size() - 1; j >= 0; j--)   // 单词内部反转
                cout << w[j];
            if (i < s.size()) cout << ' ';
            w = "";
        }
        else w += s[i];
    }
    return 0;
}
```

</details>

---

##### 3.2.09 字符串循环移位

<div style="font-size:1.2em; line-height:1.7;">**题干**：将字符串循环左移 k 位。abcd左移 1 位得到bcda。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <string>
using namespace std;
int main()
{
    string s;
    int k;
    cin >> s >> k;
    k %= s.size();               // 防止超过长度
    cout << s.substr(k) + s.substr(0, k);   // 左移k位
    return 0;
}
```

</details>

---

##### 3.2.10 字典序比较

<div style="font-size:1.2em; line-height:1.7;">**题干**：不使用字符串自带比较，手写函数比较两个字符串字典序大小。</div>

**样例**：

```text
输入s1,s2，字典序比较，s1小输出<；相等=；s1大>。
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <string>
using namespace std;
int main()
{
    string a,b;
    cin >> a >> b;
    if(a < b) cout << "<";
    else if(a == b) cout << "=";
    else cout << ">";
    return 0;
}
```

</details>

---

##### 3.2.11 提取数字

<div style="font-size:1.2em; line-height:1.7;">**题干**：从字符串中提取所有连续数字，输出每一个数字。a12bb345提取出 12，345。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <string>
using namespace std;
int main()
{
    string s;
    cin >> s;
    bool inNum = false;
    for (int i = 0; i < s.size(); i++)
    {
        if (s[i] >= '0' && s[i] <= '9')
        {
            cout << s[i];
            inNum = true;
        }
        else if (inNum)          // 一个数字结束
        {
            cout << endl;
            inNum = false;
        }
    }
    return 0;
}
```

</details>

---

##### 3.2.12 字符串去重

<div style="font-size:1.2em; line-height:1.7;">**题干**：删除重复字符，保留第一次出现顺序。abacaba → abc。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <string>
using namespace std;
int main()
{
    string s, ans = "";
    cin >> s;
    for (int i = 0; i < s.size(); i++)
    {
        bool has = false;
        for (int j = 0; j < ans.size(); j++)
            if (ans[j] == s[i]) has = true;
        if (!has) ans += s[i];   // 第一次出现才保留
    }
    cout << ans;
    return 0;
}
```

</details>

---

##### 3.2.13 前缀判断

<div style="font-size:1.2em; line-height:1.7;">**题干**：判断字符串 A 是不是字符串 B 的前缀。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <string>
using namespace std;
int main()
{
    string a, b;
    cin >> a >> b;
    if (b.size() < a.size()) { cout << "NO"; return 0; }
    for (int i = 0; i < a.size(); i++)
        if (a[i] != b[i]) { cout << "NO"; return 0; }
    cout << "YES";
    return 0;
}
```

</details>

---

##### 3.2.14 后缀判断

<div style="font-size:1.2em; line-height:1.7;">**题干**：判断字符串 A 是不是字符串 B 的后缀。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <string>
using namespace std;
int main()
{
    string a, b;
    cin >> a >> b;
    if (b.size() < a.size()) { cout << "NO"; return 0; }
    int start = b.size() - a.size();
    for (int i = 0; i < a.size(); i++)
        if (a[i] != b[start + i]) { cout << "NO"; return 0; }
    cout << "YES";
    return 0;
}
```

</details>

---

##### 3.2.15 最短循环节

<div style="font-size:1.2em; line-height:1.7;">**题干**：找字符串最小循环单元。例如abcabcabc最小循环节abc。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <string>
using namespace std;
int main()
{
    string s;
    cin >> s;
    for (int len = 1; len <= s.size(); len++)
    {
        if (s.size() % len != 0) continue;   // 长度必须能整除
        bool ok = true;
        for (int i = len; i < s.size(); i++)
            if (s[i] != s[i % len]) { ok = false; break; }
        if (ok)
        {
            cout << s.substr(0, len);        // 最小循环节
            return 0;
        }
    }
    return 0;
}
```

</details>

---

### 3.3 数组、前缀和与差分（数组前缀和差分）

#### ▸ 小类 A：前缀和与差分

##### 3.3.01 前缀和数组

<div style="font-size:1.2em; line-height:1.7;">**题干**：给定数组，构造前缀和数组，多次询问区间 \([l,r]\) 的和。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int n;
    cin >> n;
    int a[105],s[105]={0};
    for(int i=1;i<=n;i++)
    {
        cin >> a[i];
        s[i]=s[i-1]+a[i];
    }
    int l,r;
    cin >> l >> r;
    cout << s[r]-s[l-1];
    return 0;
}
```

</details>

---

##### 3.3.02 差分数组区间加

<div style="font-size:1.2em; line-height:1.7;">**题干**：初始数组全 0，多次区间 \([l,r]\) 全部加上 v，最后输出数组。</div>

**样例**：

```text
题目：数组，l~r每个元素+v，最后输出数组
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int n;
    cin >> n;
    int a[105],d[105]={0};
    for(int i=1;i<=n;i++) cin >> a[i];
    int l,r,v;
    cin >> l >> r >> v;
    d[l] +=v;
    d[r+1] -=v;
    int now=0;
    for(int i=1;i<=n;i++)
    {
        now += d[i];
        cout << a[i]+now << " ";
    }
    return 0;
}
```

</details>

---

##### 3.3.03 二维前缀和

<div style="font-size:1.2em; line-height:1.7;">**题干**：给定 \(n\times m\) 矩阵，多次询问子矩形内数字总和。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int a[105][105],s[105][105];
int main()
{
    int n,m;
    cin >> n >> m;
    for(int i=1;i<=n;i++)
        for(int j=1;j<=m;j++)
        {
            cin >> a[i][j];
            s[i][j] = s[i-1][j]+s[i][j-1]-s[i-1][j-1]+a[i][j];
        }
    int x1,y1,x2,y2;
    cin >> x1 >> y1 >> x2 >> y2;
    int ans = s[x2][y2]-s[x1-1][y2]-s[x2][y1-1]+s[x1-1][y1-1];
    cout << ans;
    return 0;
}
```

</details>

---

##### 3.3.04 二维差分

<div style="font-size:1.2em; line-height:1.7;">**题干**：矩阵多次子矩形批量加 v，最后输出整个矩阵。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int n, m, q, a[30][30] = {0}, diff[31][31] = {0};
    cin >> n >> m >> q;
    for (int i = 1; i <= n; i++)
        for (int j = 1; j <= m; j++)
            cin >> a[i][j];
    while (q--)
    {
        int x1, y1, x2, y2, v;
        cin >> x1 >> y1 >> x2 >> y2 >> v;   // 子矩形整体加v
        diff[x1][y1] += v;
        diff[x2+1][y1] -= v;
        diff[x1][y2+1] -= v;
        diff[x2+1][y2+1] += v;
    }
    for (int i = 1; i <= n; i++)
    {
        for (int j = 1; j <= m; j++)
        {
            diff[i][j] += diff[i-1][j] + diff[i][j-1] - diff[i-1][j-1];
            cout << a[i][j] + diff[i][j] << ' ';
        }
        cout << endl;
    }
    return 0;
}
```

</details>

---

#### ▸ 小类 B：子段与统计

##### 3.3.05 最大子段和（Kadane）

<div style="font-size:1.2em; line-height:1.7;">**题干**：求数组中连续一段数字的最大总和。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int n,a[105],s[105]={0};
    cin >> n;
    for(int i=1;i<=n;i++)
    {
        cin >> a[i];
        s[i]=s[i-1]+a[i];
    }
    int min_s = 0, res = -1e9;
    for(int i=1;i<=n;i++)
    {
        res = max(res, s[i]-min_s);
        min_s = min(min_s, s[i]);
    }
    cout << res;
    return 0;
}
```

</details>

---

##### 3.3.06 数组众数

<div style="font-size:1.2em; line-height:1.7;">**题干**：找出数组出现次数最多的数；如有多个，输出最小的。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int n, a[1000], cnt[10001] = {0};
    cin >> n;
    for (int i = 0; i < n; i++)
    {
        cin >> a[i];
        cnt[a[i]]++;
    }
    int best = a[0];
    for (int i = 1; i < n; i++)
        if (cnt[a[i]] > cnt[best] || (cnt[a[i]] == cnt[best] && a[i] < best))
            best = a[i];        // 次数最多；相同取最小
    cout << best;
    return 0;
}
```

</details>

---

##### 3.3.07 数组第 k 大

<div style="font-size:1.2em; line-height:1.7;">**题干**：给定数组，输出第 k 大数字（暴力排序解法）。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <vector>
#include <algorithm>
using namespace std;
int main()
{
    int n,k; cin >> n >> k;
    vector<int> v(n);
    for(int i=0;i<n;i++) cin >> v[i];
    sort(v.rbegin(),v.rend());
    cout << v[k-1] << endl;
    return 0;
}
```

</details>

---

##### 3.3.08 逆序对统计（暴力版）

<div style="font-size:1.2em; line-height:1.7;">**题干**：统计数组中 \(i<j\) 且 \(a[i]>a[j]\) 的对数。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <vector>
using namespace std;
int main()
{
    int n; cin >> n;
    vector<int> v(n);
    for(int i=0;i<n;i++) cin >> v[i];
    int cnt=0;
    for(int i=0;i<n;i++)
        for(int j=i+1;j<n;j++)
            if(v[i]>v[j]) cnt++;
    cout << cnt << endl;
    return 0;
}
```

</details>

---

##### 3.3.09 滑动窗口最大值

<div style="font-size:1.2em; line-height:1.7;">**题干**：定长窗口，在数组滑动，输出每个窗口内最大值（暴力）。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int n, k, a[1000];
    cin >> n >> k;
    for (int i = 0; i < n; i++) cin >> a[i];
    for (int i = 0; i <= n - k; i++)
    {
        int mx = a[i];
        for (int j = i + 1; j < i + k; j++)   // 暴力找窗口内最大
            if (a[j] > mx) mx = a[j];
        cout << mx << ' ';
    }
    return 0;
}
```

</details>

---

##### 3.3.10 寻找山顶

<div style="font-size:1.2em; line-height:1.7;">**题干**：数组山顶元素满足大于左右邻居，找出所有山顶下标。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int n, a[100];
    cin >> n;
    for (int i = 0; i < n; i++) cin >> a[i];
    for (int i = 0; i < n; i++)
    {
        bool isTop = true;
        if (i > 0 && a[i] <= a[i-1]) isTop = false;      // 大于左邻居
        if (i < n-1 && a[i] <= a[i+1]) isTop = false;    // 大于右邻居
        if (isTop) cout << i << ' ';
    }
    return 0;
}
```

</details>

---

##### 3.3.11 集合合并

<div style="font-size:1.2em; line-height:1.7;">**题干**：两个有序数组，求并集，升序输出。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int n, m, a[100], b[100];
    cin >> n;
    for (int i = 0; i < n; i++) cin >> a[i];
    cin >> m;
    for (int i = 0; i < m; i++) cin >> b[i];
    int i = 0, j = 0;
    while (i < n && j < m)         // 归并求并集（两个有序数组）
    {
        if (a[i] < b[j]) { cout << a[i] << ' '; i++; }
        else if (a[i] > b[j]) { cout << b[j] << ' '; j++; }
        else { cout << a[i] << ' '; i++; j++; }
    }
    while (i < n) { cout << a[i] << ' '; i++; }
    while (j < m) { cout << b[j] << ' '; j++; }
    return 0;
}
```

</details>

---

##### 3.3.12 数组环形最大子段和

<div style="font-size:1.2em; line-height:1.7;">**题干**：数组看成环形，求连续子数组最大和。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int n, a[1000];
    cin >> n;
    int total = 0;
    for (int i = 0; i < n; i++)
    {
        cin >> a[i];
        total += a[i];
    }
    int maxEnd = 0, maxSum = -1000000;   // 普通最大子段和
    int minEnd = 0, minSum = 1000000;    // 最小子段和
    for (int i = 0; i < n; i++)
    {
        maxEnd = (maxEnd + a[i] > a[i]) ? maxEnd + a[i] : a[i];
        if (maxEnd > maxSum) maxSum = maxEnd;
        minEnd = (minEnd + a[i] < a[i]) ? minEnd + a[i] : a[i];
        if (minEnd < minSum) minSum = minEnd;
    }
    int ring = total - minSum;           // 环形：总段 - 最小子段
    cout << (maxSum > ring ? maxSum : ring);
    return 0;
}
```

</details>

---

##### 3.3.13 区间最大公约数

<div style="font-size:1.2em; line-height:1.7;">**题干**：给定数组，多次询问区间 \([l,r]\) 的 gcd。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int gcd(int a, int b)
{
    return b == 0 ? a : gcd(b, a % b);
}
int main()
{
    int n, q, a[100];
    cin >> n;
    for (int i = 1; i <= n; i++) cin >> a[i];
    cin >> q;
    while (q--)
    {
        int l, r, ans = 0;
        cin >> l >> r;
        for (int i = l; i <= r; i++)
            ans = gcd(ans, a[i]);    // gcd(0, x) = x
        cout << ans << endl;
    }
    return 0;
}
```

</details>

---

#### ▸ 小类 C：离散化与集合

##### 3.3.14 数组压缩

<div style="font-size:1.2em; line-height:1.7;">**题干**：离散化。把原始很大的数值映射成 1~n 的排名。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <algorithm>
using namespace std;
int main()
{
    int n, a[1000], b[1000];
    cin >> n;
    for (int i = 0; i < n; i++)
    {
        cin >> a[i];
        b[i] = a[i];
    }
    sort(b, b + n);                                    // 排序
    int m = unique(b, b + n) - b;                      // 去重
    for (int i = 0; i < n; i++)                        // 离散化：映射为排名
        cout << lower_bound(b, b + m, a[i]) - b + 1 << ' ';
    return 0;
}
```

</details>

---

##### 3.3.15 集合交集

<div style="font-size:1.2em; line-height:1.7;">**题干**：两个有序数组，求交集，升序输出。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int n, m, a[100], b[100];
    cin >> n;
    for (int i = 0; i < n; i++) cin >> a[i];
    cin >> m;
    for (int i = 0; i < m; i++) cin >> b[i];
    int i = 0, j = 0;
    while (i < n && j < m)         // 两个有序数组归并找相同
    {
        if (a[i] == b[j]) { cout << a[i] << ' '; i++; j++; }
        else if (a[i] < b[j]) i++;
        else j++;
    }
    return 0;
}
```

</details>

---

### 3.4 排序与查找（排序与查找）

#### ▸ 小类 A：基础排序

##### 3.4.01 手写冒泡排序

<div style="font-size:1.2em; line-height:1.7;">**题干**：对整数数组从小到大排序。</div>

**样例**：

```text
题目：n个整数，冒泡从小到大排序输出。 样例输入：5 3 1 4 2 5，输出：1 2 3 4 5
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int n;
    cin >> n;
    int a[105];
    for(int i=0;i<n;i++) cin >> a[i];
    //冒泡
    for(int i=0;i<n-1;i++)
    {
        for(int j=0;j<n-1-i;j++)
        {
            if(a[j]>a[j+1])
            {
                int t=a[j];
                a[j]=a[j+1];
                a[j+1]=t;
            }
        }
    }
    for(int i=0;i<n;i++) cout << a[i] << " ";
    return 0;
}
```

</details>

---

##### 3.4.02 手写选择排序

<div style="font-size:1.2em; line-height:1.7;">**题干**：实现选择排序。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int n;
    cin >> n;
    int a[105];
    for(int i=0;i<n;i++) cin >> a[i];
    for(int i=0;i<n-1;i++)
    {
        int pos = i;
        for(int j=i+1;j<n;j++)
        {
            if(a[j]<a[pos]) pos=j;
        }
        int t=a[i]; a[i]=a[pos]; a[pos]=t;
    }
    for(int i=0;i<n;i++) cout << a[i] << " ";
    return 0;
}
```

</details>

---

##### 3.4.03 手写插入排序

<div style="font-size:1.2em; line-height:1.7;">**题干**：实现插入排序。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int n;
    cin >> n;
    int a[105];
    for(int i=0;i<n;i++) cin >> a[i];
    for(int i=1;i<n;i++)
    {
        int val = a[i];
        int j = i-1;
        while(j>=0 && a[j]>val)
        {
            a[j+1]=a[j];
            j--;
        }
        a[j+1]=val;
    }
    for(int i=0;i<n;i++) cout << a[i] << " ";
    return 0;
}
```

</details>

---

#### ▸ 小类 B：高级排序与结构体

##### 3.4.04 结构体排序

<div style="font-size:1.2em; line-height:1.7;">**题干**：学生结构体含姓名、分数，按分数降序；同分按名字字典序升序排序。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <string>
#include <algorithm>
using namespace std;
struct Student
{
    string name;
    int score;
};
bool cmp(const Student &a, const Student &b)
{
    if(a.score != b.score) return a.score > b.score;
    return a.name < b.name;
}
int main()
{
    int n; cin >> n;
    Student st[105];
    for(int i=0;i<n;i++) cin >> st[i].name >> st[i].score;
    sort(st, st+n, cmp);
    for(int i=0;i<n;i++) cout << st[i].name << " " << st[i].score << endl;
    return 0;
}
```

</details>

---

##### 3.4.05 去重排序

<div style="font-size:1.2em; line-height:1.7;">**题干**：读入 n 个数，去重之后从小到大输出。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <vector>
#include <algorithm>
using namespace std;
int main()
{
    int n; cin >> n;
    vector<int> v(n);
    for(int i=0;i<n;i++) cin >> v[i];
    sort(v.begin(),v.end());
    v.erase(unique(v.begin(),v.end()),v.end());
    for(auto x:v) cout << x << " ";
    return 0;
}
```

</details>

---

##### 3.4.06 合并两个有序数组

<div style="font-size:1.2em; line-height:1.7;">**题干**：两个升序数组合并为一个升序数组。</div>

**样例**：

```text
题目：两个已经升序的数组，合并成一个升序数组。 样例：a:1 3 5；b:2 4 6 →1 2 3 4 5 6
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int n,m;
    cin >> n;
    int a[105];
    for(int i=0;i<n;i++) cin >> a[i];
    cin >> m;
    int b[105];
    for(int i=0;i<m;i++) cin >> b[i];
    int c[210],p1=0,p2=0,idx=0;
    while(p1<n && p2<m)
    {
        if(a[p1] < b[p2]) c[idx++]=a[p1++];
        else c[idx++]=b[p2++];
    }
    while(p1<n) c[idx++]=a[p1++];
    while(p2<m) c[idx++]=b[p2++];
    for(int i=0;i<idx;i++) cout << c[i] << " ";
    return 0;
}
```

</details>

---

#### ▸ 小类 C：二分查找

##### 3.4.07 二分查找

<div style="font-size:1.2em; line-height:1.7;">**题干**：有序数组，查找目标值，存在返回下标，不存在返回 - 1。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int n, x, a[1000];
    cin >> n;
    for (int i = 0; i < n; i++) cin >> a[i];
    cin >> x;
    int L = 0, R = n - 1, ans = -1;
    while (L <= R)
    {
        int mid = (L + R) / 2;
        if (a[mid] == x) { ans = mid; break; }
        if (a[mid] < x) L = mid + 1;
        else R = mid - 1;
    }
    cout << ans;
    return 0;
}
```

</details>

---

##### 3.4.08 二分查找左边界

<div style="font-size:1.2em; line-height:1.7;">**题干**：有序数组，找目标数字第一次出现位置。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int n, x, a[1000];
    cin >> n;
    for (int i = 0; i < n; i++) cin >> a[i];
    cin >> x;
    int L = 0, R = n - 1, ans = -1;
    while (L <= R)
    {
        int mid = (L + R) / 2;
        if (a[mid] >= x)
        {
            if (a[mid] == x) ans = mid;
            R = mid - 1;          // 继续向左找更早的出现
        }
        else L = mid + 1;
    }
    cout << ans;
    return 0;
}
```

</details>

---

##### 3.4.09 二分查找右边界

<div style="font-size:1.2em; line-height:1.7;">**题干**：有序数组，找目标数字最后一次出现位置。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int n, x, a[1000];
    cin >> n;
    for (int i = 0; i < n; i++) cin >> a[i];
    cin >> x;
    int L = 0, R = n - 1, ans = -1;
    while (L <= R)
    {
        int mid = (L + R) / 2;
        if (a[mid] <= x)
        {
            if (a[mid] == x) ans = mid;
            L = mid + 1;          // 继续向右找更晚的出现
        }
        else R = mid - 1;
    }
    cout << ans;
    return 0;
}
```

</details>

---

##### 3.4.10 二分答案入门

<div style="font-size:1.2em; line-height:1.7;">**题干**：求最小 x 满足条件（例如：切绳子，n 根绳子，切成 k 段等长，求最大长度）。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int n, k;
    double len[100];
    cin >> n >> k;                    // n根绳子，切成k段
    for (int i = 0; i < n; i++) cin >> len[i];
    double L = 0, R = 100000;
    for (int t = 0; t < 100; t++)     // 二分100次足够精确
    {
        double mid = (L + R) / 2;
        int cnt = 0;
        for (int i = 0; i < n; i++)
            cnt += (int)(len[i] / mid);   // 每根能切几段
        if (cnt >= k) L = mid;        // 能切够，尝试更长
        else R = mid;
    }
    cout << L;
    return 0;
}
```

</details>

---

### 3.5 贪心算法（贪心算法）

#### ▸ 小类 A：区间类贪心

##### 3.5.01 活动选择

<div style="font-size:1.2em; line-height:1.7;">**题干**：多个活动有开始结束时间，同一时间只能参加一个，最多能选多少活动。</div>

**样例**：

```text
题目：活动有开始、结束时间，最多参加多少活动（和最大不相交区间一致）
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <algorithm>
using namespace std;
struct act{
    int st,ed;
}a[105];
bool cmp(act x,act y){return x.ed < y.ed;}
int main()
{
    int n; cin >> n;
    for(int i=0;i<n;i++) cin >> a[i].st >> a[i].ed;
    sort(a,a+n,cmp);
    int cnt=0,last=-1;
    for(int i=0;i<n;i++)
    {
        if(a[i].st >= last)
        {
            cnt++;
            last = a[i].ed;
        }
    }
    cout << cnt;
    return 0;
}
```

</details>

---

##### 3.5.02 区间覆盖

<div style="font-size:1.2em; line-height:1.7;">**题干**：给定线段 [1,T]，多个小区间，选最少数量覆盖整条线段。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <algorithm>
using namespace std;
struct Seg { int l, r; };
bool cmp(Seg a, Seg b) { return a.l < b.l; }
int main()
{
    int T, n;
    cin >> T >> n;                   // 要覆盖 [1, T]
    Seg s[100];
    for (int i = 0; i < n; i++) cin >> s[i].l >> s[i].r;
    sort(s, s + n, cmp);             // 按左端点排序
    int covered = 1, cnt = 0, i = 0;
    while (covered <= T)
    {
        int bestR = covered - 1;
        while (i < n && s[i].l <= covered)   // 能接上的区间里选右端最远
        {
            if (s[i].r > bestR) bestR = s[i].r;
            i++;
        }
        if (bestR < covered) { cout << -1; return 0; }   // 断开了
        covered = bestR + 1;
        cnt++;
    }
    cout << cnt;
    return 0;
}
```

</details>

---

##### 3.5.03 区间分组

<div style="font-size:1.2em; line-height:1.7;">**题干**：若干区间，同一组内区间不能重叠，最少分几组。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <algorithm>
using namespace std;
struct Seg { int l, r; };
bool cmp(Seg a, Seg b) { return a.l < b.l; }
int main()
{
    int n;
    cin >> n;
    Seg s[1000];
    for (int i = 0; i < n; i++) cin >> s[i].l >> s[i].r;
    sort(s, s + n, cmp);             // 按左端点排序
    int end[1000] = {0}, groups = 0;
    for (int i = 0; i < n; i++)
    {
        int j = 0;
        while (j < groups && end[j] >= s[i].l) j++;   // 找能插入的组
        if (j == groups) groups++;
        end[j] = s[i].r;             // 更新该组最晚结束时间
    }
    cout << groups;
    return 0;
}
```

</details>

---

#### ▸ 小类 B：资源与决策贪心

##### 3.5.04 硬币找零

<div style="font-size:1.2em; line-height:1.7;">**题干**：给定硬币面额，凑出金额，硬币数量最少（贪心适用版本）。</div>

**样例**：

```text
题目：硬币面值1,5,10,50，输入金额，贪心求最少硬币数量。 样例输入：37 → 5+10+10+10+1+1 =5枚
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int x;
    cin >> x;
    int coin[]={50,10,5,1};
    int cnt=0;
    for(int i=0;i<4;i++)
    {
        cnt += x / coin[i];
        x = x % coin[i];
    }
    cout << cnt;
    return 0;
}
```

</details>

---

##### 3.5.05 排队打水

<div style="font-size:1.2em; line-height:1.7;">**题干**：n 个人打水，每个人打水时间不同，安排顺序，所有人等待总时间最小。</div>

**样例**：

```text
题目：每个人打水时间，安排顺序使所有人等待时间总和最小。
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <algorithm>
using namespace std;
int main()
{
    int n,a[105];
    cin >> n;
    for(int i=0;i<n;i++) cin >> a[i];
    sort(a,a+n);
    long long sum=0,wait=0;
    for(int i=0;i<n;i++)
    {
        sum += wait;
        wait += a[i];
    }
    cout << sum;
    return 0;
}
```

</details>

---

##### 3.5.06 哈夫曼树简易版

<div style="font-size:1.2em; line-height:1.7;">**题干**：合并果子，每次合并两堆，代价为两堆之和，求最小总代价。</div>

**样例**：

```text
题目：n包糖果，每次选两包合并，代价为两包之和，最小总代价（哈夫曼简易版）
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <vector>
#include <algorithm>
using namespace std;
int main()
{
    int n;
    cin >> n;
    vector<int> v;
    for(int i=0;i<n;i++)
    {
        int x; cin >> x;
        v.push_back(x);
    }
    long long ans=0;
    while(v.size()>1)
    {
        sort(v.begin(),v.end());
        int a=v[0],b=v[1];
        v.erase(v.begin());
        v.erase(v.begin());
        int c=a+b;
        ans += c;
        v.push_back(c);
    }
    cout << ans;
    return 0;
}
```

</details>

---

##### 3.5.07 删数字

<div style="font-size:1.2em; line-height:1.7;">**题干**：给定数字字符串，删掉 k 个字符，剩下数字字典序最小。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <string>
using namespace std;
int main()
{
    string s;
    int k;
    cin >> s >> k;
    string res;
    for(char ch : s)
    {
        while(k>0 && !res.empty() && res.back()>ch)
        {
            res.pop_back();
            k--;
        }
        res.push_back(ch);
    }
    while(k--) res.pop_back();
    int pos=0;
    while(pos<res.size() && res[pos]=='0') pos++;
    if(pos == res.size()) cout << 0;
    else cout << res.substr(pos);
    return 0;
}
```

</details>

---

##### 3.5.08 商店库存

<div style="font-size:1.2em; line-height:1.7;">**题干**：商品有进货价、卖出价，每天可以买卖，求最大收益（简单贪心）。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int n, a[1000];
    cin >> n;                        // 每天价格
    for (int i = 0; i < n; i++) cin >> a[i];
    long long profit = 0;
    for (int i = 1; i < n; i++)
        if (a[i] > a[i-1])           // 涨价就赚差价
            profit += a[i] - a[i-1];
    cout << profit;
    return 0;
}
```

</details>

---

##### 3.5.09 小船过河

<div style="font-size:1.2em; line-height:1.7;">**题干**：多人过河，船最多坐两人，速度为较慢者速度，求最短总时间。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <algorithm>
using namespace std;
int main()
{
    int n, t[1000];
    cin >> n;
    for (int i = 0; i < n; i++) cin >> t[i];
    sort(t, t + n);                  // 按过河时间排序
    long long ans = 0;
    int i = 0, j = n - 1;
    while (i <= j)
    {
        if (i == j) { ans += t[i]; break; }        // 只剩1人
        if (i + 1 == j) { ans += t[j]; break; }    // 只剩2人
        // 方案1：最快送最慢两人 (去2回1去2)
        long long way1 = (long long)t[i] + t[j] + t[i] + t[j-1];
        // 方案2：最快两人过去，最快回，最慢两人过去，次快回
        long long way2 = (long long)t[i+1] + t[i] + t[j] + t[i+1];
        ans += (way1 < way2 ? way1 : way2);
        j -= 2;
    }
    cout << ans;
    return 0;
}
```

</details>

---

##### 3.5.10 加油站

<div style="font-size:1.2em; line-height:1.7;">**题干**：环形路线，每个站点存油，判断能否绕一圈（简化小数据）。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int n, gas[100], cost[100];
    cin >> n;
    for (int i = 0; i < n; i++) cin >> gas[i];    // 各站存油
    for (int i = 0; i < n; i++) cin >> cost[i];   // 各站耗油
    for (int start = 0; start < n; start++)       // 尝试每个起点（小数据）
    {
        int oil = 0;
        bool ok = true;
        for (int step = 0; step < n; step++)
        {
            int pos = (start + step) % n;
            oil += gas[pos] - cost[pos];
            if (oil < 0) { ok = false; break; }
        }
        if (ok) { cout << start; return 0; }
    }
    cout << -1;   // 无法绕一圈
    return 0;
}
```

</details>

---

### 3.6 数论（数论）

#### ▸ 小类 A：整除与质数

##### 3.6.01 欧几里得算法

<div style="font-size:1.2em; line-height:1.7;">**题干**：手写 gcd，求两个数最大公约数。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int gcd(int a,int b)
{
    if(b == 0) return a;
    return gcd(b,a%b);
}
int main()
{
    int x,y;
    cin >> x >> y;
    cout << gcd(x,y);
    return 0;
}
```

</details>

---

##### 3.6.02 最小公倍数

<div style="font-size:1.2em; line-height:1.7;">**题干**：利用 gcd 求 lcm。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int gcd(int a,int b)
{
    if(b==0) return a;
    return gcd(b,a%b);
}
int main()
{
    int a,b;
    cin >> a >> b;
    long long lcm = 1LL * a / gcd(a,b) * b;
    cout << lcm;
    return 0;
}
```

</details>

---

##### 3.6.03 埃氏筛

<div style="font-size:1.2em; line-height:1.7;">**题干**：筛出 1~n 所有质数。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
bool vis[1005];
int main()
{
    int n;
    cin >> n;
    for(int i=2;i<=n;i++)
    {
        if(!vis[i])
        {
            cout << i << " ";
            for(int j=2*i;j<=n;j+=i)
                vis[j]=true;
        }
    }
    return 0;
}
```

</details>

---

##### 3.6.04 质因数分解

<div style="font-size:1.2em; line-height:1.7;">**题干**：输入 n，输出质因数分解形式。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int n;
    cin >> n;
    for(int i=2;i*i<=n;i++)
    {
        while(n%i == 0)
        {
            cout << i << " ";
            n /= i;
        }
    }
    if(n>1) cout << n;
    return 0;
}
```

</details>

---

##### 3.6.05 判断完全数

<div style="font-size:1.2em; line-height:1.7;">**题干**：判断一个数是否等于所有真因数之和。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
bool isPerfect(int n)
{
    int sum =0;
    for(int i=1;i<n;i++)
        if(n%i ==0) sum +=i;
    return sum == n;
}
int main()
{
    int x;
    cin >> x;
    if(isPerfect(x)) cout << "完全数";
    else cout << "不是完全数";
    return 0;
}
```

</details>

---

##### 3.6.06 判断亲和数

<div style="font-size:1.2em; line-height:1.7;">**题干**：两个数互为真因数之和。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int sumDiv(int x)
{
    int s = 0;
    for (int i = 1; i < x; i++)
        if (x % i == 0) s += i;    // 真因数之和
    return s;
}
int main()
{
    int a, b;
    cin >> a >> b;
    if (sumDiv(a) == b && sumDiv(b) == a)
        cout << "YES";
    else
        cout << "NO";
    return 0;
}
```

</details>

---

#### ▸ 小类 B：模运算与数论函数

##### 3.6.07 快速幂

<div style="font-size:1.2em; line-height:1.7;">**题干**：手写快速幂，计算 \(a^b \bmod p\)。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
long long qpow(long long a,long long b,long long p)
{
    long long res=1;
    while(b>0)
    {
        if(b&1) res = res * a % p;
        a = a*a % p;
        b >>= 1;
    }
    return res;
}
int main()
{
    long long a,b,p;
    cin >> a >> b >> p;
    cout << qpow(a,b,p);
    return 0;
}
```

</details>

---

##### 3.6.08 欧拉函数 φ(n)

<div style="font-size:1.2em; line-height:1.7;">**题干**：计算 1~n 中和 n 互质的数字个数。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int gcd(int a, int b)
{
    return b == 0 ? a : gcd(b, a % b);
}
int main()
{
    int n;
    cin >> n;
    int cnt = 0;
    for (int i = 1; i <= n; i++)
        if (gcd(i, n) == 1) cnt++;   // 与n互质的个数
    cout << cnt;
    return 0;
}
```

</details>

---

##### 3.6.09 同余方程

<div style="font-size:1.2em; line-height:1.7;">**题干**：小数据暴力求解 \(ax \equiv 1 \pmod{m}\)。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int a, m;
    cin >> a >> m;                  // 求 ax ≡ 1 (mod m)
    for (int x = 0; x < m; x++)     // 暴力枚举 0~m-1（小数据）
        if ((long long)a * x % m == 1)
        {
            cout << x;
            return 0;
        }
    cout << -1;                     // 无解
    return 0;
}
```

</details>

---

##### 3.6.10 取模运算

<div style="font-size:1.2em; line-height:1.7;">**题干**：大整数模，输入很长的数字字符串，求 mod m。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <string>
using namespace std;
int main()
{
    string s;
    int m;
    cin >> s >> m;                  // 大整数以字符串输入
    int ans = 0;
    for (int i = 0; i < s.size(); i++)
        ans = (ans * 10 + (s[i] - '0')) % m;   // 逐位取模
    cout << ans;
    return 0;
}
```

</details>

---

### 3.7 递归、DFS与搜索（递归DFS搜索）

#### ▸ 小类 A：递归与组合枚举

##### 3.7.01 递归求组合数

<div style="font-size:1.2em; line-height:1.7;">**题干**：\(C(n,k)\)。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int C(int n, int k)
{
    if (k == 0 || k == n) return 1;                    // 边界
    return C(n - 1, k - 1) + C(n - 1, k);              // 组合递推
}
int main()
{
    int n, k;
    cin >> n >> k;
    cout << C(n, k);
    return 0;
}
```

</details>

---

##### 3.7.02 全排列

<div style="font-size:1.2em; line-height:1.7;">**题干**：递归输出 1~n 全部排列。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int n;
int a[105];
bool vis[105];
void dfs(int step)
{
    if(step == n+1)
    {
        for(int i=1;i<=n;i++) cout << a[i] << " ";
        cout << endl;
        return;
    }
    for(int i=1;i<=n;i++)
    {
        if(!vis[i])
        {
            vis[i]=true;
            a[step]=i;
            dfs(step+1);
            vis[i]=false;
        }
    }
}
int main()
{
    cin >> n;
    dfs(1);
    return 0;
}
```

</details>

---

##### 3.7.03 组合枚举

<div style="font-size:1.2em; line-height:1.7;">**题干**：从 n 个数选出 k 个，输出所有组合方案。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int n, k, path[20];
void dfs(int start, int len)
{
    if (len == k)
    {
        for (int i = 0; i < k; i++)
            cout << path[i] << (i == k-1 ? '\n' : ' ');
        return;
    }
    for (int x = start; x <= n; x++)
    {
        path[len] = x;
        dfs(x + 1, len + 1);        // 下一个数必须更大
    }
}
int main()
{
    cin >> n >> k;
    dfs(1, 0);
    return 0;
}
```

</details>

---

##### 3.7.04 子集枚举

<div style="font-size:1.2em; line-height:1.7;">**题干**：输出 n 个元素全部子集。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int n,a[105];
void dfs(int pos, int sum)
{
    if(pos == n)
    {
        cout << sum << endl;
        return;
    }
    dfs(pos+1, sum);
    dfs(pos+1, sum+a[pos]);
}
int main()
{
    cin >> n;
    for(int i=0;i<n;i++) cin >> a[i];
    dfs(0,0);
    return 0;
}
```

</details>

---

##### 3.7.05 24 点搜索版

<div style="font-size:1.2em; line-height:1.7;">**题干**：4 个数字，枚举所有运算符与括号组合，判断能否算出 24。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
bool near24(double x) { return x > 23.99 && x < 24.01; }
bool dfs(double nums[], int cnt)
{
    if (cnt == 1) return near24(nums[0]);
    double nxt[4];
    for (int i = 0; i < cnt; i++)          // 枚举任意两个数运算
        for (int j = 0; j < cnt; j++)
        {
            if (i == j) continue;
            int t = 0;
            for (int k = 0; k < cnt; k++)
                if (k != i && k != j) nxt[t++] = nums[k];
            double x = nums[i], y = nums[j];
            nxt[t] = x + y; if (dfs(nxt, t + 1)) return true;
            nxt[t] = x - y; if (dfs(nxt, t + 1)) return true;
            nxt[t] = x * y; if (dfs(nxt, t + 1)) return true;
            if (y != 0) { nxt[t] = x / y; if (dfs(nxt, t + 1)) return true; }
        }
    return false;
}
int main()
{
    double nums[4];
    for (int i = 0; i < 4; i++) cin >> nums[i];
    cout << (dfs(nums, 4) ? "YES" : "NO");
    return 0;
}
```

</details>

---

#### ▸ 小类 B：图与棋盘搜索

##### 3.7.06 迷宫 DFS

<div style="font-size:1.2em; line-height:1.7;">**题干**：二维迷宫，'.' 通路，'#' 墙，求从起点到终点是否存在路径。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
char mp[105][105];
int n,m;
bool ok;
int dx[]={1,-1,0,0};
int dy[]={0,0,1,-1};
void dfs(int x,int y)
{
    if(mp[x][y] == 'T') {ok=true;return;}
    mp[x][y]='#';
    for(int d=0;d<4;d++)
    {
        int nx=x+dx[d], ny=y+dy[d];
        if(nx>=0&&nx<n&&ny>=0&&ny<m && mp[nx][ny]!='#')
        {
            dfs(nx,ny);
        }
    }
}
int main()
{
    cin >> n >> m;
    int sx,sy;
    for(int i=0;i<n;i++)
    {
        for(int j=0;j<m;j++)
        {
            cin >> mp[i][j];
            if(mp[i][j]=='S') sx=i,sy=j;
        }
    }
    ok=false;
    dfs(sx,sy);
    if(ok) cout << "YES";
    else cout << "NO";
    return 0;
}
```

</details>

---

##### 3.7.07 连通块计数

<div style="font-size:1.2em; line-height:1.7;">**题干**：二维网格，统计连通块数量（DFS）。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int n, m, cnt = 0;
char g[30][30];
int dx[4] = {-1, 1, 0, 0};
int dy[4] = {0, 0, -1, 1};
void dfs(int x, int y)
{
    g[x][y] = '.';                  // 标记已访问
    for (int k = 0; k < 4; k++)
    {
        int nx = x + dx[k], ny = y + dy[k];
        if (nx >= 0 && nx < n && ny >= 0 && ny < m && g[nx][ny] == '#')
            dfs(nx, ny);
    }
}
int main()
{
    cin >> n >> m;
    for (int i = 0; i < n; i++)
        for (int j = 0; j < m; j++)
            cin >> g[i][j];
    for (int i = 0; i < n; i++)
        for (int j = 0; j < m; j++)
            if (g[i][j] == '#') { cnt++; dfs(i, j); }
    cout << cnt;
    return 0;
}
```

</details>

---

##### 3.7.08 八皇后

<div style="font-size:1.2em; line-height:1.7;">**题干**：递归枚举，输出八皇后全部合法方案。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int col[10], cnt = 0;
bool ok(int r)
{
    for (int i = 1; i < r; i++)
        if (col[i] == col[r] || col[i] - i == col[r] - r || col[i] + i == col[r] + r)
            return false;           // 同列或同一对角线
    return true;
}
void dfs(int r)
{
    if (r == 9)                     // 8行都放好
    {
        cnt++;
        for (int i = 1; i <= 8; i++) cout << col[i] << ' ';
        cout << endl;
        return;
    }
    for (int c = 1; c <= 8; c++)
    {
        col[r] = c;
        if (ok(r)) dfs(r + 1);
    }
}
int main()
{
    dfs(1);
    cout << "共" << cnt << "种方案";
    return 0;
}
```

</details>

---

#### ▸ 小类 C：搜索枚举

##### 3.7.09 数字拆分

<div style="font-size:1.2em; line-height:1.7;">**题干**：将 n 拆分为若干正整数之和，不考虑顺序，输出所有拆分方案。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int n, path[20];
void dfs(int left, int minPart, int len)
{
    if (left == 0)
    {
        if (len >= 2)               // 至少拆成两部分
        {
            for (int i = 0; i < len; i++)
                cout << path[i] << (i == len-1 ? '\n' : '+');
        }
        return;
    }
    for (int x = minPart; x <= left; x++)
    {
        path[len] = x;
        dfs(left - x, x, len + 1);  // 不降序，避免重复方案
    }
}
int main()
{
    cin >> n;
    dfs(n, 1, 0);
    return 0;
}
```

</details>

---

##### 3.7.10 填数字

<div style="font-size:1.2em; line-height:1.7;">**题干**：3×3 方格，填入 1~9 不重复，满足行和条件（小暴力搜索）。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int g[3][3];
bool used[10];
void show()
{
    for (int i = 0; i < 3; i++)
    {
        for (int j = 0; j < 3; j++)
            cout << g[i][j] << ' ';
        cout << endl;
    }
    cout << "---" << endl;
}
bool check()                         // 三阶幻方：行列对角线都相等
{
    int s = g[0][0] + g[0][1] + g[0][2];
    for (int i = 1; i < 3; i++)
        if (g[i][0] + g[i][1] + g[i][2] != s) return false;
    for (int j = 0; j < 3; j++)
        if (g[0][j] + g[1][j] + g[2][j] != s) return false;
    if (g[0][0] + g[1][1] + g[2][2] != s) return false;
    if (g[0][2] + g[1][1] + g[2][0] != s) return false;
    return true;
}
void dfs(int pos)
{
    if (pos == 9)
    {
        if (check()) show();
        return;
    }
    int x = pos / 3, y = pos % 3;
    for (int num = 1; num <= 9; num++)
        if (!used[num])
        {
            used[num] = true;
            g[x][y] = num;
            dfs(pos + 1);
            used[num] = false;
        }
}
int main()
{
    dfs(0);
    return 0;
}
```

</details>

---

### 3.8 简单动态规划（简单动态规划DP）

#### ▸ 小类 A：路径与序列DP

##### 3.8.01 爬楼梯

<div style="font-size:1.2em; line-height:1.7;">**题干**：一次可以走 1 或 2 级，走到 n 级有多少种方案。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int n;
    cin >> n;
    long long f[100];
    f[1] = 1;
    f[2] = 2;
    for (int i = 3; i <= n; i++)
        f[i] = f[i-1] + f[i-2];    // 最后一步走1级或2级
    cout << f[n];
    return 0;
}
```

</details>

---

##### 3.8.02 数字三角形

<div style="font-size:1.2em; line-height:1.7;">**题干**：从顶部往下走，每次只能左下或右下，求路径最大和。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <algorithm>
using namespace std;
int a[105][105],f[105][105];
int main()
{
    int n;
    cin >> n;
    for(int i=1;i<=n;i++)
        for(int j=1;j<=i;j++)
            cin >> a[i][j];
    for(int j=1;j<=n;j++) f[n][j]=a[n][j];
    for(int i=n-1;i>=1;i--)
    {
        for(int j=1;j<=i;j++)
        {
            f[i][j] = max(f[i+1][j],f[i+1][j+1]) + a[i][j];
        }
    }
    cout << f[1][1];
    return 0;
}
```

</details>

---

##### 3.8.03 最长上升子序列 LIS

<div style="font-size:1.2em; line-height:1.7;">**题干**：求数组最长严格上升子序列长度（O (n²) 版本）。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <algorithm>
using namespace std;
int main()
{
    int n,a[105],dp[105];
    cin >> n;
    for(int i=1;i<=n;i++)
    {
        cin >> a[i];
        dp[i]=1;
    }
    int ans=1;
    for(int i=1;i<=n;i++)
    {
        for(int j=1;j<i;j++)
        {
            if(a[j] < a[i])
            {
                dp[i]=max(dp[i],dp[j]+1);
            }
        }
        ans = max(ans,dp[i]);
    }
    cout << ans;
    return 0;
}
```

</details>

---

##### 3.8.04 最长公共子序列 LCS

<div style="font-size:1.2em; line-height:1.7;">**题干**：两个字符串，求最长公共子序列长度。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <string>
#include <algorithm>
using namespace std;
int dp[105][105];
int main()
{
    string s1,s2;
    cin >> s1 >> s2;
    int n = s1.size(), m = s2.size();
    for(int i=1;i<=n;i++)
    {
        for(int j=1;j<=m;j++)
        {
            if(s1[i-1]==s2[j-1])
            {
                dp[i][j] = dp[i-1][j-1]+1;
            }
            else
            {
                dp[i][j] = max(dp[i-1][j], dp[i][j-1]);
            }
        }
    }
    cout << dp[n][m];
    return 0;
}
```

</details>

---

##### 3.8.05 最长公共子串

<div style="font-size:1.2em; line-height:1.7;">**题干**：两个字符串，求最长连续公共子串。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <string>
using namespace std;
int main()
{
    string a, b;
    cin >> a >> b;
    int n = a.size(), m = b.size();
    int dp[101][101] = {0}, best = 0;
    for (int i = 1; i <= n; i++)
        for (int j = 1; j <= m; j++)
        {
            if (a[i-1] == b[j-1])
            {
                dp[i][j] = dp[i-1][j-1] + 1;   // 连续才累计
                if (dp[i][j] > best) best = dp[i][j];
            }
            else dp[i][j] = 0;
        }
    cout << best;
    return 0;
}
```

</details>

---

#### ▸ 小类 B：背包与组合DP

##### 3.8.06 01 背包

<div style="font-size:1.2em; line-height:1.7;">**题干**：n 件物品，体积 v，价值 w，背包容量 V，求最大价值。</div>

**样例**：

```text
题目：n件物品，背包容量V，每件物品重量w，价值v，求最大价值。
```

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <algorithm>
using namespace std;
int dp[1005];
int main()
{
    int n,V;
    cin >> n >> V;
    for(int i=1;i<=n;i++)
    {
        int w,v;
        cin >> w >> v;
        for(int j=V;j>=w;j--)
        {
            dp[j] = max(dp[j], dp[j-w]+v);
        }
    }
    cout << dp[V];
    return 0;
}
```

</details>

---

##### 3.8.07 完全背包

<div style="font-size:1.2em; line-height:1.7;">**题干**：物品可以无限拿，求背包最大价值。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int n, W, w[100], v[100], dp[1001] = {0};
    cin >> n >> W;
    for (int i = 0; i < n; i++) cin >> w[i] >> v[i];
    for (int i = 0; i < n; i++)            // 每件物品
        for (int j = w[i]; j <= W; j++)    // 完全背包正序遍历
            if (dp[j - w[i]] + v[i] > dp[j])
                dp[j] = dp[j - w[i]] + v[i];
    cout << dp[W];
    return 0;
}
```

</details>

---

##### 3.8.08 编辑距离

<div style="font-size:1.2em; line-height:1.7;">**题干**：把字符串 A 变成 B，允许插入、删除、替换，求最少操作次数。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
#include <string>
using namespace std;
int main()
{
    string a, b;
    cin >> a >> b;
    int n = a.size(), m = b.size();
    int dp[101][101] = {0};
    for (int i = 0; i <= n; i++) dp[i][0] = i;   // 全部删除
    for (int j = 0; j <= m; j++) dp[0][j] = j;   // 全部插入
    for (int i = 1; i <= n; i++)
        for (int j = 1; j <= m; j++)
        {
            if (a[i-1] == b[j-1])
                dp[i][j] = dp[i-1][j-1];
            else
            {
                int ins = dp[i][j-1] + 1;     // 插入
                int del = dp[i-1][j] + 1;     // 删除
                int rep = dp[i-1][j-1] + 1;   // 替换
                dp[i][j] = ins;
                if (del < dp[i][j]) dp[i][j] = del;
                if (rep < dp[i][j]) dp[i][j] = rep;
            }
        }
    cout << dp[n][m];
    return 0;
}
```

</details>

---

##### 3.8.09 整数划分 DP

<div style="font-size:1.2em; line-height:1.7;">**题干**：将 n 拆分为若干正整数之和，方案总数。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int n;
    cin >> n;
    long long dp[101] = {0};
    dp[0] = 1;                              // 空划分
    for (int x = 1; x <= n; x++)            // 每种数字
        for (int s = x; s <= n; s++)        // 完全背包计数
            dp[s] += dp[s - x];
    cout << dp[n];
    return 0;
}
```

</details>

---

##### 3.8.10 石子合并

<div style="font-size:1.2em; line-height:1.7;">**题干**：一排石子，每次合并相邻两堆，代价为两堆总和，求最小总代价（小数据）。</div>

<details>
<summary>点击展开参考答案（C++）</summary>

```cpp
#include <iostream>
using namespace std;
int main()
{
    int n, a[101], sum[101] = {0};
    int dp[101][101] = {0};
    cin >> n;
    for (int i = 1; i <= n; i++)
    {
        cin >> a[i];
        sum[i] = sum[i-1] + a[i];           // 前缀和
    }
    for (int len = 2; len <= n; len++)      // 区间长度
        for (int i = 1; i + len - 1 <= n; i++)
        {
            int j = i + len - 1;
            dp[i][j] = 1 << 30;
            for (int k = i; k < j; k++)     // 合并点
            {
                int cost = dp[i][k] + dp[k+1][j] + sum[j] - sum[i-1];
                if (cost < dp[i][j]) dp[i][j] = cost;
            }
        }
    cout << dp[1][n];
    return 0;
}
```

</details>

---
