# CALCULATOR PRGRAM
def add(num1, num2):
    return num1+num2
def subtract(num1, num2):
    return num1-num2
def multiply(num1, num2):
    return num1*num2
def division(num1, num2):
    return num1/num  
print("please select an operation\n","1.add\n","2.subtract\n","3.multiply\n","4.divide\n")     
select=int(input("selectthe operation from 1,2,3,4:")) 
number_1=int(input("enter 1st no. ")) 
number_2=int(input("enter 2nd no. "))
if select==1:
    print(number_1,"+",number_2,"=",add(number_1,number_2))     
elif select==2:
   print(number_1,"-",number_2,"=",subtract(number_1,number_2))     
elif select==3:
   print(number_1,"*",number_2,"=",multiply(number_1,number_2))     
elif select==4:
      print(number_1,"/",number_2,"=",divide(number_1,number_2))    
else:
    print("invalid input")
