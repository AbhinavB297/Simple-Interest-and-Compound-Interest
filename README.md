# Simple-Interest-and-Compound-Interest
def simple_intrest_equation(principle, intrest, time):
	equation_1=(principle*intrest*time)/100
	print("Here is your answer:", equation_1)
def compound_intrest_equation(principle, intrest, time):
	totalamount=principle*(1+intrest/100)**time
	equation_2=totalamount-principle
	print("Here is your answer:", equation_2)
principle=float(input("How much do you want to put in?: "))
intrest=float(input("at what rate do you want it to grow(pls do in percent)?: "))
time=float(input("How long do you want it to grow? give in years, if you want to add months, add as decimal.: "))
user_question=int(input("Do you want me to calculate simple intrest(insert number 1), or compound intrest(insert number 2): "))
if user_question==1:
	simple_intrest_equation(principle, intrest, time)
elif user_question==2:
	compound_intrest_equation(principle, intrest, time)
else:
	print("error: invalid number, only 1 or 2")
