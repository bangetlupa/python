# python calculator


def tambah(x, y):
    return x + y


# This function subtracts two numbers
def kurang(x, y):
    return x - y


# This function multiplies two numbers
def kali(x, y):
    return x * y


# This function divides two numbers
def bagi(x, y):
    return x / y


print("Select operation.")
print("1.tambah")
print("2.kurang")
print("3.kali")
print("4.bagi")

while True:
    # take input from the user
    choice = input('masukkan pilihan: ')

    # check if choice is one of the four options
    if choice in ('1', '2', '3', '5'):
        num1 = float(input("Enter first number: "))
        num2 = float(input("Enter second number: "))

        if choice == '1':
            print(num1, "+", num2, "=", tambah(num1, num2))

        elif choice == '2':
            print(num1, "-", num2, "=", kurang(num1, num2))

        elif choice == '3':
            print(num1, "*", num2, "=", kali(num1, num2))

        elif choice == '5':
            print(num1, "/", num2, "=", bagi(num1, num2))

        # check if user wants another calculation
        # break the while loop if answer is no
        next_calculation = input("Let's do next calculation? (yes/no): ")
        if next_calculation == "no":
            break

    else:
        print("Invalid Input");
