# Hey
# Just some random ideas
# May as well put some code in here!

responses = {}

# set a flag to indicate that polling is true
polling_active = True

while polling_active:
	name = input("\nWhat is your name? ")
	response = input("Which party do you intend to vote for in the 2020 general election?")

	# Store the response in a the dictionary (above)
	responses[name] = response

	#find out if someone else is going to take the poll 

	repeat = input("Would you like to let another person respond? (yes/ no) ")
	if repeat == 'no':
		polling_active = False

#polling complete. Show the results

for name, response in responses.items():
	print(f"{name} intends to vote for {response}.")
