刷爆朋友圈



Time Limit:1000MS  Memory Limit:65536K

Total Submit:1202 Accepted:446



Description



朋友圈是微信的大杀器之一，发朋友圈的消息可以快速在朋友之间分享。微信还提供一种转发功能，可以将在朋友圈看到的消息分享到自己的朋友圈。这可以实现消息的病毒式快速传播。

已知有N个人，他们的编号为0到N-1，他们形成了M个朋友圈，假设朋友圈内的每个人看到别人发朋友圈的消息都会在自己的朋友圈进行转发。

发朋友圈消息的人编号为0，请你算出总共有多少人(包括编号为0的人自己)能看到0所发的朋友圈消息。



Input



输入第一行为两个正整数N和M，（1 <= N <= 100000），M（ 1<= M <= 1000）,代表共N个人，M个朋友圈，以空格间隔。

接下来M行，每行首先输入一个整数K（ 2 <= K <= 100）代表该朋友圈的人数，然后输入K个数为该朋友圈内的人员编号(输入数据必有0，0的个数可能不唯一)，以空格间隔。



Output



输出一行一个整数，代表能看到0所发的朋友圈消息的人数。



Sample Input





100 4

2 1 2

5 10 13 11 12 14

2 0 1

2 99 2

Sample Output





4

字符串统计(时间限制：3秒)



Time Limit:3000MS  Memory Limit:65536K

Total Submit:2491 Accepted:422



Description



输入若干行字符串，输出出现次数最多的一条字符串。



Input



输入数据的第一行有一个整数N，表示有N行字符串（1 < N < 10^6）。

接下来有N行字符串，字符串只包含小写字母，长度不大于 100 ， 不重复的字符串数目不超过 1000 。



Output



输出出现次数最多的一条字符串，数据保证结果唯一。



Sample Input





3

asdfghjkl

asdfghjkl

fefeff

Sample Output





asdfghjkl



B. Zzz,Pddddddd and Hikari1149 were sworn brothers



Time Limit:1000MS  Memory Limit:65536K

Total Submit:1020 Accepted:195



Description



Hikari1149 got a job recently, so he has to go to work every day. But the traffic on the way to his company is very terrible. The road on his way always been ruined. It cause a huge trouble for Hikari1149 to find a way to company, So, as his sworn brothers, Zzz and Pddddddd, of course, will not let Hikari1149 feels that way. Given n places, m bidirectional roads that currently exist and q operations. There are two types of operation:

1\) P k (It means the kth road is ruined now.)

2\) Z x y (It means a query that does there currently exists a way between place x and place y.)







Input



The first line contains three integers n, m and q, which indicates the number of places, the number of roads and the number of operations.

Then each line of next m lines contains two integers u and v. The ith line of next m lines means the ith road is between place u and place v.

Then each line of next q lines contains one operation, its format is as mentioned in the previous description.

It’s guaranteed will not exists multiple edges, self-loop and one road will not been ruined repeatedly, but the graph maybe not connected.

1<=n, m, q<=10^5; 1<=k<=m; 1<=u, v, x, y<=n, x≠y.



Output



For each operation 2, if there currently exists a way between place x and place y, then output “Yes”, otherwise, output “No”.



Sample Input





5 4 5

1 2

2 3

3 4

4 5

Z 1 2

P 1

Z 1 3

P 3

Z 2 4

Sample Output





Yes

No

No



药不能停



Time Limit:1000MS  Memory Limit:65536K

Total Submit:1391 Accepted:398



Description



小明很喜欢算法和编程，他的大学学业生涯规划是：厦门理工学院程序设计大赛一等奖、福建省程序设计大赛金牌、蓝桥杯软件大赛全国一等奖、亚洲区域赛金牌、World final金牌、Google就业年薪百万。小明是懒癌晚期，他不想通过努力训练完成规划，他想通过吃药来提高智商，秒杀一众高手。





小明发现单吃一种药效果太差，他要将已有的N种药物混合成1种药再吃。已知每种药都有一定的毒性，将任意两种药混合的毒性为这两种药的毒性之和，混合产生的新药的毒性也同样为两种药的毒性之和。由于技术限制，小明每次只能挑选两种药进行混合。现在小明想知道将N种药合成1种药的最小毒性和。



Input



输入第一行为一个正整数N（1 <= N <= 100000）

接下来一行输入N个正整数，第i个整数a\[i]代表第i种药的毒性( 1 <= a\[i] <= 1000)



Output



输出一行一个整数，代表药的最小毒性和。



Sample Input





5

1 2 3 4 5

Sample Output





33

八目鳗烧烤店



Time Limit:1000MS  Memory Limit:65536K

Total Submit:2765 Accepted:1191



Description



八目鳗烧烤店一共有6个八目鳗，幽幽子一口能吃1到6个八目鳗，求吃完所有的八目鳗共有多少种吃法。

任意一口吃的八目鳗数量不同，就算不同的吃法。



Input



无



Output



输出一个整数，表示吃完所有的八目鳗共有多少种吃法。

不要书写任何多余的内容（例如：添加说明文字等）。



Sample Input





Sample Output





Hint



\#include



int main()

{

printf("这里写答案\\n");

return 0;

}



**#include <stdio.h>**

**#include <string.h>**

**#include <stdlib.h>**



**#define MAX\_STR\_LEN 101**

**#define HASH\_SIZE 2003**

**typedef struct Node**

**{**

&#x20;   **char str\[MAX\_STR\_LEN];**

&#x20;   **int count;**

&#x20;   **struct Node\* next;**

**} Node;**



**Node\* hashTable\[HASH\_SIZE];**



**unsigned int hash(const char\* s)**

**{**

&#x20;   **unsigned int h = 0;**

&#x20;   **while (\*s)**

&#x20;   **{**

&#x20;       **h = h \* 131 + (\*s++);**

&#x20;   **}**

&#x20;   **return h % HASH\_SIZE;**

**}**



**Node\* findOrInsert(const char\* s)**

**{**

&#x20;   **unsigned int idx = hash(s);**

&#x20;   **Node\* p = hashTable\[idx];**

&#x20;   **while (p)**

&#x20;   **{**

&#x20;       **if (strcmp(p->str, s) == 0)**

&#x20;           **return p;**

&#x20;       **p = p->next;**

&#x20;   **}**

&#x20;   **Node\* newNode = (Node\*)malloc(sizeof(Node));**

&#x20;   **strcpy(newNode->str, s);**

&#x20;   **newNode->count = 0;**

&#x20;   **newNode->next = hashTable\[idx];**

&#x20;   **hashTable\[idx] = newNode;**

&#x20;   **return newNode;**

**}**



**int main()**

**{**

&#x20;   **int N;**

&#x20;   **scanf("%d", \&N);**

&#x20;   **char buf\[MAX\_STR\_LEN];**

&#x20;   **Node\* maxNode = NULL;**

&#x20;   **for (int i = 0; i < N; ++i)**

&#x20;   **{**

&#x20;       **scanf("%s", buf);**

&#x20;       **Node\* node = findOrInsert(buf);**

&#x20;       **node->count++;**

&#x20;       **if (maxNode == NULL || node->count > maxNode->count)**

&#x20;       **{**

&#x20;           **maxNode = node;**

&#x20;       **}**

&#x20;   **}**

&#x20;   **printf("%s\\n", maxNode->str);**

&#x20;   **return 0;**

**}**

