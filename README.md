# task-2 : Calculator

print("\n -------------------Basic Calculator--------------------")

quit=""

while (len(quit)==0 or quit[0]=='y' or quit[0]=='Y'):
    a=float(input("\nEnter the first number : "))
    b=float(input("\nEnter the second number : "))
    print()

    print("Press :-\n",
          "\t1 --> for Addition\n",
          "\t2 --> for Subtraction\n",
          "\t3 --> for Multiplication\n",
          "\t4 --> for Division")
    
    ch=input("Enter your choice = ")
    print()

    if(ch.isdigit()):
        #for Addition
        if(int(ch) == 1):
            print(f"\tResult for : ( {a} + {b} ) == {a+b}")
            print()

        #for subtraction
        elif(int(ch) == 2):
            print(f"\tResult for : ( {a} - {b} ) == {a-b}")
            print()
            print(f"\tResult for : ( {b} - {a} ) == {b-a}")
            print()
        
        #for multiplication
        elif(int(ch) ==3):
            print(f"\tResult for : ( {a} * {b} ) == {a*b}")
            print()
        
        #for Division
        elif(int(ch) == 4):
            if(a==0 and b==0):
                print("\t Sorry both numbers are ZERO and can't be divided")
                print()
            else:
                if(b != 0):
                    print("\tResult for  ({a} / {b}) = {a/b}")
                else:
                    print("\t Sorry, {a} can't be divided by {b}")
                    print()
        
                if(a != 0):
                    print("\tResult for  ({b} / {a}) = {b/a}")
                else:
                    print("\t Sorry, {a} can't be divided by {b}")
                    print()

        #Not from the operator list
        else:
            print("\t ERROR :- No such operator can be used. Try Again")
            print()
    #Any Random Input found        
    else:
        print("\t ERROR :- No such operator can be used. Try Again")
        print()
        continue

    quit=input ("Want to continue?  (y/n) =")

    print("\n\n-----------------------------------------------------------------------")


    
