import math

x = int(input("Enter total count of numbers in first: "))
y = int(input("Enter count of correct numbers: "))

z = int(input("Enter total count of numbers in second: "))
c = int(input("Enter count of correct numbers: "))

def varbutiba():


    qwer = y / x
    rewq = c / z
    qwerty = y / x * 100
    ytrewq = c / z * 100

    if qwer > rewq:
        print("Pirmaja varbutiba ir veiksmigaks.")
        print("Tās iespēja ir: ", qwerty, "%")
    elif qwer < rewq:
        print("Otraja varbutiba ir veiksmigaks.")
        print("Tās iespēja ir: ", ytrewq, "%")
    elif qwer == rewq:
        print("Abi ir veiksmigi")
    else:
        print("Error, mēgiņiet velreiz.")

varbutiba()

def kombinatorika():

    ty = y / x
    th = c / z

    if ty > th:
        print("Combination count is: ", (math.factorial(x)))
    elif ty < th:
        print("Combination count is: ", (math.factorial(c)))

kombinatorika()

if __name__ == '__main__':
    while True:
       varbutiba()
       restart = input('One more time? :?').lower()
       if restart == "Yes":
           varbutiba()
