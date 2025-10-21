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
```
import matplotlib.pyplot as plt
x=[0,1,2,3,4,5]
y=[10,20,4,16,30,40]
plt.plot(x,y)
plt.xlabel("X-AXIS")
plt.ylabel("Y-AXIS")
plt.title("GRAPH")
plt.show()
```
![image](https://github.com/user-attachments/assets/e6f963c3-01c4-43b8-ad59-5b3356d20a2f)
```
x1=[1,2,3]
y1=[2,4,1]
x2=[1,2,3]
y2=[4,1,3]
plt.plot(x2,y2,label="line 2")
plt.plot(x1,y1,label="line 1")
plt.xlabel("X-AXIS")
plt.ylabel("Y-AXIS")
plt.title("GRAPH")
plt.legend()
plt.show()
```

![image](https://github.com/user-attachments/assets/533fcc25-0ab3-4d30-af97-3e7c360a041a)
```
x=[1,2,3,4,5,6]
y=[2,4,1,5,2,6]
plt.plot(x,y,color="red",linewidth=9,linestyle="dashed",marker='o',markerfacecolor='green',markersize=12)
plt.ylim(1,8)
plt.xlim(1,8)
plt.xlabel("X-AXIS")
plt.ylabel("Y-AXIS")
plt.title("GRAPH")
plt.show()
```

![image](https://github.com/user-attachments/assets/66b748af-f252-446d-9f31-87143806d950)
```
years = range(2000, 2012)
apples = [0.895, 0.91, 0.919, 0.926, 0.929, 0.931, 0.934, 0.936, 0.937, 0.9375, 0.9372, 0.939]
oranges = [0.962, 0.941, 0.93, 0.923, 0.918, 0.908, 0.897, 0.894, 0.891, 0.886, 0.9, 0.896]

plt.plot(years, apples)
plt.plot(years, oranges)

plt.xlabel('Year')
plt.ylabel('Yield (tons per hectare)')
plt.title('Crop Yields in Kanto')
plt.legend(['Apples', 'Oranges'])
```

![image](https://github.com/user-attachments/assets/ddefa414-6d01-43f6-abb2-4d26c6626460)
```
yield_apples = [0.895, 0.91, 0.919, 0.926, 0.929, 0.931]
plt.plot(yield_apples)
```

![image](https://github.com/user-attachments/assets/c030b27d-bbbb-4024-96f2-d9cb273851d8)
```
years = [2010, 2011, 2012, 2013, 2014, 2015]
yield_apples = [0.895, 0.91, 0.919, 0.926, 0.929, 0.931]
plt.plot(years, yield_apples)
plt.xlabel('YEAR')
plt.ylabel('YIELD(tons per hectare)')
```

![image](https://github.com/user-attachments/assets/6f3089ec-8e97-468d-9c39-d72e7b050031)
```
plt.figure(figsize=(10,6))
y=list(range(2000,2012))
plt.plot(y,oranges,marker='o')
plt.title("YIELD OF ORANGES(tons per hectare)")
```

![image](https://github.com/user-attachments/assets/09400eae-1c69-4fe8-bf04-369e0f775bec)
```
plt.plot(y,oranges,marker='x')
plt.plot(y,apples,marker='o')
plt.xlabel("YEAR")
plt.ylabel("YIELD(tons per hectare)")
plt.title("YIELD OF ORANGES AND APPLES(tons per hectare)")
plt.legend(["oranges","apples"])
```

![image](https://github.com/user-attachments/assets/98445f98-d9f3-4ae7-9b1a-5a0cf7da215f)
```
x=[0,1,2,3,4,5]
y=[10,20,4,16,30,40]
plt.scatter(x,y,s=30,color="red")
plt.show()
```

![image](https://github.com/user-attachments/assets/e7bb1233-036a-4250-b60c-3bb1ca389e27)
```
x=[0,1,2,3,4,5]
y=[10,20,4,16,30,40]
plt.scatter(x,y,marker="*",color="blue")
plt.xlabel("X-AXIS")
plt.ylabel("Y-AXIS")
plt.title("SCATTER PLOT")
plt.legend()
plt.show()
```

![image](https://github.com/user-attachments/assets/3e8db8c9-2ea9-4370-9c8f-2c6b9c22e62d)
```
import numpy as np
import pandas as pd
x=np.arange(0,10)
y=np.arange(11,21)
x
```

![image](https://github.com/user-attachments/assets/4535e010-9150-461e-b838-26d70c9fc66b)
```
y
```

![image](https://github.com/user-attachments/assets/5bfcc40e-f79f-4bde-9d1a-1223840b3247)
```
plt.scatter(x,y,c="r")
plt.xlabel("X-AXIS")
plt.ylabel("Y-AXIS")
plt.title("GRAPH IN 2D")
plt.savefig("Test.png")
```

![image](https://github.com/user-attachments/assets/edcb0655-c683-4689-b09d-068840ba440c)
```
y=x*x
y
```

![image](https://github.com/user-attachments/assets/01dcebdd-2422-40a8-a138-7fc57b63b416)
```
plt.plot(x,y,'g*',linestyle="dashed",linewidth=2,markersize=12)
plt.xlabel("X-AXIS")
plt.ylabel("Y-AXIS")
plt.title("2D GRAPH")
```

![image](https://github.com/user-attachments/assets/4dd7f126-daa3-41a2-bac8-d4a699b2e4bc)
```
plt.subplot(2, 2, 1)
plt.plot(x, y, 'r--')

plt.subplot(2, 2, 2)
plt.plot(x, y, 'g*--')

plt.subplot(2, 2, 3)
plt.plot(x, y, 'bo')

plt.subplot(2, 2, 4)
plt.plot(x, y, 'go')
```

![image](https://github.com/user-attachments/assets/322f105d-7558-4741-a7ad-0e780a4d99c8)
```
x=np.arange(0,4*np.pi,0.1)
y=np.sin(x)
plt.title("sine wave form")
plt.plot(x, y)
plt.show()

```

![image](https://github.com/user-attachments/assets/0532cadd-fedd-4abd-ab01-7f2129dec995)
```
x = [1, 2, 3, 4, 5]
y1 = [10, 12, 14, 16, 18]
y2=[5, 7, 9, 11, 13]
y3=[2, 4, 6, 8, 10]
plt.fill_between(x, y1, color='blue')
plt.fill_between(x, y2, color='green')
plt.plot(x, y1, color='red')
plt.plot(x, y2, color='black')
plt.legend(['y1','y2'])
plt.show()
```

![image](https://github.com/user-attachments/assets/d26085db-547e-4520-b3c7-8dd0e2452296)
```
plt.stackplot(x, y1, y2, y3, labels=['Line 1', 'Line 2', 'Line 3'])
plt.legend(loc='upper left')
plt.title('Stacked Line Chart')
plt.xlabel('X-axis')
plt.ylabel('Y-axis')
plt.show()
```

![image](https://github.com/user-attachments/assets/6e4ca601-2c7d-4584-84a0-6d885b6e4138)
```
from scipy.interpolate import make_interp_spline
x= np.array([1, 2, 3, 4, 5, 6, 7, 8, 9, 10])
y = np.array([2, 4, 5, 7, 8, 8, 9, 10, 11, 12])
spl = make_interp_spline(x, y)
x_smooth = np.linspace(x.min(), x.max(), 100)
y_smooth = spl(x_smooth)
plt.plot(x, y, 'o', label='data')
plt.plot(x_smooth, y_smooth, '-', label='spline')
plt.legend()
plt.title("SPLINE CHART")
plt.show()
```

![image](https://github.com/user-attachments/assets/ecc696e9-1240-477b-95df-ed258fa945cf)
```
val=[5,4,8,6,3]
names=["A","B","C","D","E"]
plt.bar(names,val,color="red")
plt.title("BAR GRAPH")
plt.show()
```

![image](https://github.com/user-attachments/assets/0d1449e7-757d-47b6-8777-951046dcc6ec)
```
plt.barh(names,val,color="pink")
plt.title("BAR GRAPH(horizontal)")
plt.show()
```

![image](https://github.com/user-attachments/assets/dfe2ac34-9cb2-42bf-b69e-e7ede87f1215)
```
height=[10,24,36,37,45]
names=['one','two','three','four','five']
c1=['red','blue']
c2=['b','g']
plt.bar(names,height,color=c1,width=0.8)
plt.xlabel("names")
plt.ylabel("height")
plt.title("BAR CHART")
plt.show()
```

![image](https://github.com/user-attachments/assets/a5b7d71c-62d8-4e56-baa9-fe3d7affe05d)
```
x=[2,8,10]
y=[11,16,9] 
x2=[3,9,11] 
y2=[6,15,7]
plt.bar(x, y,color='yellowgreen') 
plt.bar(x2, y2, color = 'purple')
plt.title("Bar graph")
plt.ylabel('Y axis')
plt.xlabel('x axis')
plt.show()
```

![image](https://github.com/user-attachments/assets/38219006-1b9f-43aa-aae5-7c6bc6fc5258)
```
ages=[2,5,70,40,30,45,50,45,43,40,44,60,7,13,57,18,90,77,32,21,20,40]
range=(0, 100)
bins=10
plt.hist(ages, bins, range, color='cyan', histtype='bar', rwidth=0.8)
plt.xlabel('age')
plt.ylabel('No. of people')
plt.title('Histogram')
plt.show()
```

![image](https://github.com/user-attachments/assets/431ea6bf-d3e2-4848-b797-2b9d4f51516b)
```
x = [2,1,6,4,2,4,8,9,4,2,4,10,6,4,5,7,7,3,2,7,5,3,5,9,2,1]
plt.hist(x, bins=10, color='blue', alpha=0.5)
plt.show()

```

![image](https://github.com/user-attachments/assets/99fefd74-333a-463a-ab6f-726ec7cecf15)
```
np.random.seed(0)
data=np.random.normal(loc=0,scale=1,size=100)
data
```

![image](https://github.com/user-attachments/assets/03d8540f-60ae-468d-9ae0-f56e0e16f7b9)
```
fig,ax=plt.subplots()
ax.boxplot(data)
ax.set_title("BOX PLOT")
ax.set_ylabel("Y-AXIS")
ax.set_xlabel("X-AXIS")
```

![image](https://github.com/user-attachments/assets/765b76af-0126-460c-b2fa-64c3e8b44570)
```
activities = ['eat', 'sleep', 'work', 'play']
slices=[3, 7, 8, 6]
colors = ['r', 'y', 'g', 'b']
plt.pie(slices,labels=activities,colors=colors,startangle=90, 
        shadow=True,explode=(0,0,0.1,0), radius=1.2, autopct='%1.1f%%')
plt.legend ()
plt.show()
```

![image](https://github.com/user-attachments/assets/b56e792a-957c-44bb-b4df-b2648ea9f30a)
```
labels=['Python','C++','Ruby','Java']
sizes=[215, 130, 245, 210] 
colors=['gold', 'yellowgreen', 'lightcoral', 'lightskyblue'] 
explode=(0,0.4,0,0.5)
plt.pie(sizes, explode=explode, labels=labels, colors=colors, autopct='%1.1f%%',shadow=True)
plt.axis('equal')
plt.show()
```

![image](https://github.com/user-attachments/assets/64d715a0-e308-4fc7-8ef3-b08e1a1c9bf8)

# Result:
Data Visualization using matplot python library for the given datas is successfully performed.

