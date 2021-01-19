# Circle-Calculator-
A calculator that calculates the volume or area of a circle with inputs of the radius and height  

#Author William Bui
import math

def area(radius,height):#function or method which is called in the if statements
  areaCylinder=2*math.pi*radius*height+2*math.pi*math.pow(radius,2)
  print('The area is ' ,round(areaCylinder,2))
  
def volume(radius,height): #function or method which is called in the if statements
  vC=math.pi*radius**2*height
  print('The volume is', round(vC,2))


def main():
    radius=float(input("Please enter radius \n"))
    height=float(input("Please enter a height \n"))
      
    answer=input("What do you want to caluclate:area or volume \n")
    if answer=='area':#if input= areait will display the aformentioned below
      area(radius,height)
      
    if answer=='volume':#if input=vC it will display the aformentioned below
      volume(radius,height)
      
    again=input("do you wish to do it again? (yes/ no)\n")
    if again =='yes': #repeats code
        main()
    else: #exits code
        print("Bye")
        exit()
main()

