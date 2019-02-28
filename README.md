# py

/*这是我最近的python作业1，绘制一个五角星，并涂色*/
import turtle
turtle.pensize(0.5)  #设置线条粗细
turtle.pencolor("black")  #画笔颜色
turtle.fillcolor("red")   #填涂颜色
 
turtle.begin_fill()  #准备开始填充图形
for i in range(6):  #循环六次，如果循环次数为五次，填涂的红色会覆盖五角星的线条
    turtle.forward(200)  #从头部绘制线条和箭头到尾部，200为向当前画笔方向前进的距离
    turtle.right(144)  #顺时针转动箭头方向144°
turtle.end_fill()  #填充完成

/*绘制六角形*/
import turtle 
 
turtle.pensize(0.5)
turtle.pencolor("black")
 
turtle.left(30)
turtle.forward(100)

for i in range(5):  #绘制一个正六边形
    turtle.right(60)
    turtle.forward(100)

turtle.forward(100)
turtle.right(120)
turtle.forward(100)

for i in range(5):  #以正六边形的每条边作为一个三角形的边绘制等边三角形
    turtle.left(60)
    turtle.forward(100)
    turtle.right(120)
    turtle.forward(100)
    
/*绘制叠加三角形*/
import turtle as t
 
t.pensize(0.5)
t.pencolor("black")

for i in range(3):
    t.fd(200)
    t.left(120)


for i in range(3):
    t.fd(100)
    t.left(120)

for i in range(2):
    t.fd(100)
    t.left(60)

t.left(60)
t.fd(100)

/*字符串的输入输出*/
name = input("")  #input()函数是输入字符串的
words = input("")
print("%s，我想对你说，%s" % (name,words))  # %s是输出字符串的格式限定符

/*求一个数的0到5次方*/
n = eval(input())  #eval()函数去掉参数最外侧引号并执行余下语句，即n如果是一个数，那么使用eval()函数，n可以是float类型也可以是int类型

a = pow(n,0)
b = pow(n,1)
c = pow(n,2)
d = pow(n,3)
e = pow(n,4)
f = pow(n,5)

print(a, b, c, d, e, f)

/*m和n的运算*/
m = eval(input())
n = int(input())  #n为int类型
a = m + n
b = m * n
c = pow(m,n)
d = m % n

if m > n:
    e = m
else:
    e = n
    
print(a, b, c, d, e)
