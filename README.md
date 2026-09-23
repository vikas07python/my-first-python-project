# Weekly Expense Tracker - Day 2 Project

expenses = []
total = 0

print("Enter your expenses for 7 days:")
for i in range(7):
    amount = int(input(f"Day {i+1} expense: "))
    expenses.append(amount)
    total += amount

average = total / 7
highest = max(expenses)

print("\n--- Weekly Report ---")
print(f"Total expense: {total} Rs")
print(f"Average per day: {average} Rs")
print(f"Highest expense in a day: {highest} Rs")

if total > 3000:
    print("You spent too much this week. Let's save next week!")
else:
    print("Great control on spending!")
