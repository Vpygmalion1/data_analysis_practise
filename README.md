## 数据分析笔试题

### 题目1：数据集Retail_Data_Transactions.csv记录了客户ID，交易时间和交易金额三个字段，需求是对客户ID进行汇总统计，计算每一个客户的如下特征变量，并把结果输出为csv文件。

- Last_date: 最后一次交易时间

- Recency: 最后一次交易时间距离今天的间隔天数

- Frequnece: 累计交易次数

- Amount: 累计交易金额
- Intereval: 平均两次交易之间的间隔天数(如果客户只有一次交易字段为空值)

 

### 题目2：在题目1的输出结果基础上，构造三个新的字段，规则如下，结果输出为csv文件。

- 对Recency字段进行分段，分为5段，用1-5编号，每一段内的人数相同，分段后的新字段名Recency_bin
- 对Frequency字段进行分段，分为5段，用1-5编号，每一段内的人数相同，分段后的新字段名Frequency_bin
- 对Amount字段进行分段，按照100为间距分段，即0-100,100-200… 分段编号用1,2,3,…自然数编号，分段后的新字段名Amount_bin

### 题目3：在题目2的输出结果基础上，对Recency_bin和Frequency_bin进行交叉统计分析，生成如下报表：统计Rececny_bin和Frequency_bin组合对应的客户数。