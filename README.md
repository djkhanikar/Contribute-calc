# Contribute-calc
Contribute calc
#Simplified calculator for contribution on any trip

print("Welcome to the contribution calculator!")
bill = float(input("What is the total expense? $"))
contribute = int(input("How much contribution would you like to give? 10, 14, or 20?"))
member = int(input("How many contributors to split the bill?"))
contribute_as_percent = contribute / 100
total_contribute_amount = bill * contribute_as_percent
total_bill = bill + total_contribute_amount
contribute_per_person = total_bill / member
final_amount = round(contribute_per_person, 2)
final_amount = "{:.2f}".format(contribute_per_person)
print(f"Each person should contribute {final_amount}")
