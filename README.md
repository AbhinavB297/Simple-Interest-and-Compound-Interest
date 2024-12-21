# Simple-Interest-and-Compound-Interest
def simple_intrest_equation(principle, intrest, time):
	"""This will function will calculate simple intrest"""
	equation_1=(principle*intrest*time)/100
	print("Here is your answer:", equation_1)
def compound_intrest_equation(principle, intrest, time):
	"""This will function will calculate compound intrest"""
	totalamount=principle*(1+intrest/100)**time
	equation_2=totalamount-principle
	print("Here is your answer:", equation_2)
"""These 3 will have user provide the quanities they want to input"""
principle=float(input("How much do you want to put in?: "))
intrest=float(input("at what rate do you want it to grow(pls do in percent)?: "))
time=float(input("How long do you want it to grow? give in years, if you want to add months, add as decimal.: "))
"""This next question will ask the user if they want to use simple or compound intrest. They will have to insert 1 or 2 depending on their prefered choice"""
user_question=int(input("Do you want me to calculate simple intrest(insert number 1), or compound intrest(insert number 2): "))
"""The if-elif-else statment below is used to calculate the response from user_question line. It will call the corrisponding function depending on their choice. If they choose an invalid choice, the error code will come up."""
if user_question==1:
	simple_intrest_equation(principle, intrest, time)
elif user_question==2:
	compound_intrest_equation(principle, intrest, time)
else:
	print("error: invalid number, only 1 or 2")
