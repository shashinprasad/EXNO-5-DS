# EXNO-5-DS-DATA VISUALIZATION USING MATPLOT LIBRARY

# Aim:
  To Perform Data Visualization using matplot python library for the given datas.

# EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

# Coding and Output:
```python
import matplotlib.pyplot as plt
x_values=[0,1,2,3,4,5]
y_values=[0,1,4,9,16,25]
plt.plot(x_values,y_values)
plt.show()
```
![image](https://github.com/Augustine0306/EXNO-5-DS/assets/119404460/8d37b088-143e-4f9e-a809-f36abd824ff1)
```python
import matplotlib.pyplot as plt
x=[1,2,3]
y=[2,4,1]
plt.plot(x,y)
plt.xlabel('x-axis')
plt.ylabel("y-axis")
plt.title('My first grpah!')
plt.show()
```
![image](https://github.com/Augustine0306/EXNO-5-DS/assets/119404460/4b0e6974-4a99-4ba9-bb18-8fcb2de3496a)
```python
import matplotlib.pyplot as plt
x1=[1,2,3]
y1=[2,4,1]
plt.plot(x1,y1,label='line 1')
x2=[1,2,3]
y2=[4,1,3]
plt.plot(x2,y2,label='line 2')
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title("two lines on same grapg!")
plt.legend()
plt.show()
```
![image](https://github.com/Augustine0306/EXNO-5-DS/assets/119404460/75a32970-b7eb-4bff-91fb-790d76219aed)
```python
import matplotlib.pyplot as plt
import numpy as np
x=[1,2,3,4,5]
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10]
plt.fill_between(x,y1,color='blue')
plt.fill_between(x,y2,color='green')
```
![image](https://github.com/Augustine0306/EXNO-5-DS/assets/119404460/89c87c88-35b5-4ca6-b994-381b338ee648)
```python
plt.stackplot(x,y1,y2,y3,labels=['line1','line2','line3'])
plt.legend(loc='upper left')
plt.title('stacked line chart')
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.show()
```
![image](https://github.com/Augustine0306/EXNO-5-DS/assets/119404460/3148ad2e-2b1e-460d-89bb-5197a2a635f4)
```python
import numpy as np
import matplotlib.pyplot as plt
values=[5,6,3,7,2]
names=["A","B","C","D","E"]
plt.bar(names,values,color='green')
plt.show()
```
![image](https://github.com/Augustine0306/EXNO-5-DS/assets/119404460/41e804be-9970-4fbb-986e-6bdf6d5b5f91)
```python
import matplotlib.pyplot as plt
import numpy as np

ages=[2,5,70,40,30,45,50,45,43,40,44,60,7,13,57,18,90,77,32,21,20,40]
range = (0, 100)
bins=10
plt.hist(ages,bins,range,color='green',histtype='bar',rwidth=0.8)
plt.xlabel('age')
plt.ylabel('no of people')
plt.title('histogram')
plt.show()
```
![image](https://github.com/Augustine0306/EXNO-5-DS/assets/119404460/b5b1fe7a-aaad-4c30-82d1-42918996089d)
```python
import matplotlib.pyplot as plt
import numpy as np
np.random.seed(0)
data=np.random.normal(loc=0,scale=1,size=100)
data
```
![image](https://github.com/Augustine0306/EXNO-5-DS/assets/119404460/8f5ac038-2099-4999-9b1b-1138cc3d984f)
```python
fig,ax=plt.subplots()
ax.boxplot(data)
ax.set_xlabel("data")
ax.set_ylabel("values")
ax.set_title("box plot")
```
![image](https://github.com/Augustine0306/EXNO-5-DS/assets/119404460/a6fc9060-1637-48ab-b95c-dfc789e4d798)
```python
import matplotlib.pyplot as plt
activities=['eat','sleep','work','play']
slices=[3,7,8,6]
colors=['r','y','g','b']
plt.pie(slices,labels = slices,colors=colors,startangle=90,shadow = True,explode = (0,0,0.1,0),radius=1.2,autopct='%1.1f%%')
plt.legend()
plt.show()
```
![image](https://github.com/Augustine0306/EXNO-5-DS/assets/119404460/da790ff0-33a9-4864-aeed-776610a34b49)
# Result:
Thus, Data Visualization using matplot python library is implemented successfully.
