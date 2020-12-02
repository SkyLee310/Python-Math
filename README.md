# Python-Math
#PythonMath Author:Skylee310
import time
print('你好(*´▽｀)ノノ我是Sky，你的机械助理')
time.sleep(1)
print('当前版本为1.04.30 BETA ,您可通过联机获取最新版本')
time.sleep(1)
while True:
    xuanze=input('''请选择功能:
   a.计算器
   b.计算三角形面积 
   c.计算平方根(SquareRoot)
   d.寻找因数(Factor)
   e.计算最大公约数(HCF)
   f.计算最小公倍数(LCM)
   g.计算抛物线长度(Length of parabora)
   h.计算圆外边长度(Length of Arc)
   您的选择是： ''')
    if xuanze=='a':
            def add(x, y):
                return x + y
        
            def subtract(x, y):
                return x - y
        
            def multiply(x, y):
                return x * y
        
            def divide(x, y):
                return x / y
        
            
            print("选择运算：")
            print("1、相加")
            print("2、相减")
            print("3、相乘")
            print("4、相除")
        
            choice = input("输入你的选择(1/2/3/4/输入其他退出):")
        
            num1 = int(input("输入第一个数字: "))
            num2 = int(input("输入第二个数字: "))
        
            if choice == '1':
                print(num1,"+",num2,"=", add(num1,num2))
                time.sleep(2)
        
            elif choice == '2':
                print(num1,"-",num2,"=", subtract(num1,num2))
                time.sleep(2)
            elif choice == '3':
                print(num1,"*",num2,"=", multiply(num1,num2))
                time.sleep(2)
            elif choice == '4':
                print(num1,"/",num2,"=", divide(num1,num2))
                time.sleep(2)
            else:
                print("非法输入")
                time.sleep(2)
            break
    elif xuanze=='b':
                a = float(input('输入三角形第一边长: '))
                b = float(input('输入三角形第二边长: '))
                c = float(input('输入三角形第三边长: '))
                s = (a + b + c) / 2
                #海尔公式
                area = (s*(s-a)*(s-b)*(s-c)) ** 0.5
                print('三角形面积为 %0.2f' %area)
                time.sleep(2)
    elif xuanze=='c':
                num = float(input('请输入一个数字： '))
                num_sqrt = num ** 0.5
                print(' %0.3f 的平方根为 %0.3f'%(num ,num_sqrt))
                time.sleep(2)
    elif xuanze=='d':
        x = int(input("Input a Number: "))
        for i in range(1,x+1):
            if x%i==0:
                print(i)
        time.sleep(3)
    elif xuanze=='e':
                # 定义一个函数
        def hcf(x, y):
                #"""该函数返回两个数的最大公约数"""
        
        # 获取最小值
            if x > y:
                smaller = y
            else:
                smaller = x
            
            for i in range(1,smaller + 1):
                if((x % i == 0) and (y % i == 0)):
                    hcf = i
            
            return hcf
        
        
        # 用户输入两个数字
        num1 = int(input("输入第一个数字: "))
        num2 = int(input("输入第二个数字: "))
        
        print( num1,"和", num2,"的最大公约数为", hcf(num1, num2))
        time.sleep(2)
    elif xuanze=='f':
                # 定义函数
        def lcm(x, y):
        
        #  获取最大的数
            if x > y:
                greater = x
            else:
                greater = y
            while(True):
                if((greater % x == 0) and (greater % y == 0)):
                    lc = greater
                    break
                    greater += 1
            
            return lcm
            
        
        # 获取用户输入
        num1 = int(input("输入第一个数字: "))
        num2 = int(input("输入第二个数字: "))
        
        print( num1,"和", num2,"的最小公倍数为", lcm)
        time.sleep(2)
    
    elif xuanze == 'g':
        i = int(input("抛物线水平长度： "))
        h = int(input("为抛物线的矢高(抛物线对比地面的最高点）： "))
        L= i+(8*h**2)/(3*i**2)*i
        print("抛物线的长度为：", L)
        time.sleep(5)
    elif xuanze == 'h':
        pi = 3.1415926
        r = int(input("Radius: "))
        tht = int(input("θ："))
        arc = (tht/360)*(2*pi*r)
        print(arc)
        time.sleep(3)

#作者：Skylee


    

        

