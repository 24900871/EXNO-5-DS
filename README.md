![image](https://github.com/user-attachments/assets/4fa59352-ec71-4a3a-8b25-da95a7cc5651)# EXNO-5-DS-DATA VISUALIZATION USING MATPLOT LIBRARY

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

~~~
x1 = [1,2,3]
y1 = [2,4,1]
x2 = [1,2,3]
y2 = [4,1,3]
plt.plot(x1,y1,label='line1')
plt.plot(x2,y2,label='line2')
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Two lines on same graph!')
plt.legend()
plt.show()
~~~

![image](https://github.com/user-attachments/assets/fa13f90d-bdd8-4356-9df8-345cb4a47e19)

~~~

import matplotlib.pyplot as plt
x=[1,2,3,4,5,6]
y=[2,4,1,5,2,6]
plt.plot(x,y,color='green',linestyle='dashed',linewidth=3,marker='o',markerfacecolor='blue',markersize=12)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Some cool customizations!')
plt.show()

~~~

![image](https://github.com/user-attachments/assets/84e44240-be2d-4984-b652-0f13862b0882)

~~~

yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(yield_apples)

~~~

![image](https://github.com/user-attachments/assets/42cf8f8f-7d28-4106-a24c-9cf8ac8a7955)

~~~

years=[2010,2011,2012,2013,2014,2015]
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(years,yield_apples)

~~~

![image](https://github.com/user-attachments/assets/36c52a05-e97d-4431-97ac-51492fefb100)

~~~

years=range(2000,2012)
apples=[0.895,0.91,0.919,0.926,0.929,0.931,0.934,0.936,0.937,0.9375,0.9372,0.939]
oranges=[0.926,0.941,0.930,0.923,0.918,0.908,0.907,0.904,0.901,0.898,0.9,0.896, ]
plt.plot(years, apples)
plt.plot(years, oranges)
plt.xlabel('Year')
plt.ylabel('Yield (tons per hectare)')
plt.title('Crop Yields in Kanto')
plt.legend(['Apples','Oranges']);

~~~

![image](https://github.com/user-attachments/assets/eb68de82-0fb5-4e81-bb33-060fffb68d95)

~~~

plt.figure(figsize=(12,6))
plt.plot(years,oranges,marker='o')
plt.title("Yield of Oranges (tons per hectare)");

~~~

![image](https://github.com/user-attachments/assets/59aacd2b-5f44-4ebe-8eb6-d53075556586)


~~~

plt.scatter(x,y,c='r')
plt.xlabel('X-axis')
plt.ylabel('Y-axis')
plt.title('Graph in 2D')
plt.savefig('Test.png')

~~~

![image](https://github.com/user-attachments/assets/ba31768a-2e5d-4c16-a096-6bd08e974a76)

~~~

plt.plot(x,y,'g*',linestyle='dashed',linewidth=2,markersize=12)
plt.xlabel('X axis')
plt.ylabel('Y axis')
plt.title('2d Diagram')
plt.legend(['y-values']);

~~~

![image](https://github.com/user-attachments/assets/0e43de4f-870d-4ad7-acd1-1fb6c3811298)

~~~
import matplotlib.pyplot as plt
import numpy as np
x=[1,2,3,4,5]
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10]
plt.fill_between(x,y1,color='blue')
plt.fill_between(x,y2,color='green')
plt.plot(x,y1,color='red')
plt.plot(x,y2,color='black')
plt.legend(['y1','y2'])
plt.show()

~~~

![image](https://github.com/user-attachments/assets/2ef057e7-b3e3-4fd1-bdb8-dfe9e506a113)

~~~

import matplotlib.pyplot as plt
height=[10,24,36,40,5]
names=['one','two','three','four','five']
c1=['red','green']
c2=['b','g']
plt.bar(names,height,width=0.8,color=c1)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('My bar chart!')
plt.show()

~~~

![image](https://github.com/user-attachments/assets/419e8ea5-1adc-40f3-9cd0-b351c4469c9e)

~~~

x=[2,8,10]
y=[11,16,9]
x2=[3,9,11]
y2=[6,15,7]
plt.bar(x,y,color='r')
plt.bar(x2,y2,color='g')
plt.title('Bar graph')
plt.ylabel('Y axis')
plt.xlabel('X axis')
plt.show()

~~~

![image](https://github.com/user-attachments/assets/d7732fa5-ddcf-40e4-877b-aa35622aab66)

~~~

import matplotlib.pyplot as plt
ages=[2,5,70,40,30,45,50,45,43,40,44,60,7,13,57,18,90,77,32,21,20,40]
range=(0,100)
bins=10
plt.hist(ages,bins,range,color='green',histtype='bar',rwidth=0.8)
plt.xlabel('age')
plt.ylabel('No. of people')
plt.title('My histogram')
plt.show()

~~~

![image](https://github.com/user-attachments/assets/225cc3ff-e637-4d6c-a373-6638eb13cf9e)

~~~

fig,ax=plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Values')
ax.set_title('Box Plot')

~~~

![image](https://github.com/user-attachments/assets/86d4d4ec-52df-44a6-a7d2-f100fafcad68)

~~~

labels='Python','C++','Ruby','Java'

sizes=[215,130,245,210]
colors=['gold','yellowgreen','lightcoral','lightskyblue']
explode=(0,0.4,0,0.5)
plt.pie(sizes,explode=explode,labels=labels,colors=colors,autopct='%1.1f%%',shadow=True)
plt.axis('equal')
plt.show()

~~~

![image](https://github.com/user-attachments/assets/34f695fc-2806-4208-8a35-66384fe113e4)

~~~

activities=['eat','sleep','work','play']
slices=[3,7,8,6]
colors=['r','y','g','b']
plt.pie(slices,labels=activities,colors=colors,startangle=90,shadow=True,explode=(0,0,0.1,0),radius=1.2,autopct='%1.1f%%')
plt.legend()

~~~

![image](https://github.com/user-attachments/assets/b2b89f3f-0c7b-4e7b-b042-706f2d3fc33d)


# Result:
Thus the program has been executed successfully.
