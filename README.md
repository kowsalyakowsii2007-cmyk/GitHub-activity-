
ATM withdrawal simulation 
Name: kowsalya B 
Department: CCE- I year


    # ATM Withdrawal Simulation

balance = 5000  # Initial account balance

print("🏧 Welcome to ABC Bank ATM")
print("----------------------------")
print("Your current balance is:", balance)

# Ask user how much they want to withdraw
amount = int(input("Enter the withdrawal amount: "))

# Check conditions
if amount <= 0:
    print("❌ Invalid amount. Enter a positive number.")

elif amount > balance:
    print("❌ Insufficient balance! Please check your balance and try again.")

elif amount % 100 != 0:
    print("❌ ATM can dispense only multiples of 100.")

else:
    balance -= amount
    print("✅ Withdrawal Successful!")
    print("💵 Amount Withdrawn:", amount)
    print("💰 Remaining Balance:", balance)

print("----------------------------")
print("Thank you for using ABC Bank ATM 😊")