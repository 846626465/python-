# python数据分析
## 列表拆分构建字典
- 例子：
```python
age_name = ["18_sibalu","17_alimiya"]
```
- 方法一：
```python
dict_person = {} # 构建空字典
for n in age_name：
  # 字符串.split()以某个字符为介，分割成两个字符串
  # 字典增加元素操作，字典['键'] = 值
  dict_person[n.split('_')[0]] = n.split('_')[1]
```
- 方法二：
```python
#字典推导式
dict_person = {n.split('_')[0]:n.split('_')[1] for n in name_age}
```
## 日期构建与格式变化
- 日期构建
```python
import datatime
date_nCoV = datetime.date(2020,1,3) # data_nCoV的值为2020-01-03
date_SARS = datetime.date(2002,12,5)
```
- 求日期差
```python
date_nCoV.__sub__(date_SARS) # __sub__两个对象相减
```
- 格式化输出日期
```python
# strftime() 函数接收以时间元组，并返回以可读字符串表示的当地时间
# %y 两位数的年份表示（00-99）,%Y 四位数的年份表示（000-9999）
date_nCoV.strftime("%y/%m/%d") #data_nCoV的值为20/01/03
```
## Jupyter魔术命令

