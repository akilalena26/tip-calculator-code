# tip-calculator-code
# Just a program to understand how the numerical datatype works.
#If the bill was $150.00, split between 5 people, with 12% tip. 

#Each person should pay (150.00 / 5) * 1.12 = 33.6
#Format the result to 2 decimal places = 33.60

print("Welcome to the tip calculator!")
bill=input("What is the bill amount?")
tip=input("what is the tip percentage?")
people=input("How many people are splitting the bill?")
bill_as_float=float(bill)
tip_as_float=float(tip)
people_as_int=int(people)
tip_as_float=(tip_as_float/100)+1
total_bill=bill_as_float*tip_as_float
total_bill_per_person=total_bill/people_as_int
total_bill_per_person=round(total_bill_per_person,2)
print(f"Each person should pay {total_bill_per_person}")
