

print("🏧 Welcome to ATM Withdrawal System")

# Initial balance in account
balance = 5000  

while True:
    print("\nYour Current Balance: ₹", balance)

    amount = int(input("Enter amount to withdraw: "))

    if amount <= 0:
        print("❌ Invalid amount. Please enter a valid number.")

    elif amount > balance:
        print("❌ Insufficient balance!")

    else:
        balance -= amount
        print("\n✅ Withdrawal Successful!")
        print("Amount Withdrawn: ₹", amount)
        print("Remaining Balance: ₹", balance)

    choice = input("\nDo you want to withdraw again? (yes/no): ").lower()

    if choice != "yes":
        print("\n Thank you for using the ATM!")
        break