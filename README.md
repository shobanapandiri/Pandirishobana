# Pandirishobana
A Python-based ATM simulation with login, deposit, withdrawal, and balance features.
# Setting predefined username and password for login
username = 'shobana'
password = 'python123'

# Taking user input for login
c_name = input("Enter your name: ")      # Prompt user to enter their username
c_pass = input("Enter your password: ")  # Prompt user to enter their password

# Checking if entered credentials match the stored ones
if c_name == username and c_pass == password:
    # If login is successful, display options
    print('''
1. Deposit
2. Withdraw
3. Mini Statement
4. Exit
''')

    amount = 50000  # Initialize ATM balance with 50,000
    option = int(input("Select your option (1-4): "))  # Take user choice

    # If user selects Deposit
    if option == 1:
        dep = int(input("Enter the amount: "))  # Ask for deposit amount
        amount += dep  # Add deposit to balance
        print("Total amount:", amount)  # Show updated balance

    # If user selects Withdraw
    elif option == 2:
        withd = int(input("Enter the amount: "))  # Ask for withdrawal amount
        amount -= withd  # Subtract wit

    # If user selects Exit
    elif option == 4:
        exit()  # Exit the program

# If login credentials are incorrect
else:
    print("Enter correct logins")  # Prompt user to try again
    