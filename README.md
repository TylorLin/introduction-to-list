# introduction-to-list
codecademy lesson


#introduction to list 
zoo_animals = ["pangolin", "cassowary", "sloth","pig" ];
# One animal is missing!

if len(zoo_animals) > 3:
	print "The first animal at the zoo is the " + zoo_animals[0]
	print "The second animal at the zoo is the " + zoo_animals[1]
	print "The third animal at the zoo is the " + zoo_animals[2]
	print "The fourth animal at the zoo is the " + zoo_animals[3]
  
  
#access by index
numbers = [5, 6, 7, 8]

print "Adding the numbers at indices 0 and 2..."
print numbers[0] + numbers[2]
print "Adding the numbers at indices 1 and 3..."
print numbers[1] + numbers[3]

#new nieghbors
zoo_animals = ["pangolin", "cassowary", "sloth", "tiger"]
# Last night our zoo's sloth brutally attacked 
#the poor tiger and ate it whole.

# The ferocious sloth has been replaced by a friendly hyena.
zoo_animals[2] = "hyena"
zoo_animals[3] = "pig"

#late arrival & list length
suitcase = [] 
suitcase.append("sunglasses")
suitcase.append("people")
suitcase.append("beach")
suitcase.append("hat")

list_length = len(suitcase)# Set this to the length of suitcase

print "There are %d items in the suitcase." % (list_length)
print suitcase

#List Slicing
suitcase = ["sunglasses", "hat", "passport", "laptop", "suit", "shoes"]

first  = suitcase[0:2]  # The first and second items (index zero and one)
middle = suitcase[2:4]                # Third and fourth items (index two and three)
last   = suitcase[4:6]                # The last two items (index four and five)

#Slicing Lists and Strings
animals = "catdogfrog"
cat  = animals[:3]   # The first three characters of animals
dog  = animals[3:6]              # The fourth through sixth characters
frog = animals[6:]              # From the seventh character to the end
print cat
print dog
print frog

#Maintaining Order
animals = ["aardvark", "badger", "duck", "emu", "fennec fox"]
duck_index =animals.index("duck")    # Use index() to find "duck"
animals.insert(duck_index,"cobra")
print animals # Observe what prints after the insert operation

#For One and All
my_list = [1,9,3,8,5,7]
for i in my_list:
    print 2*i

#More with 'for'
start_list = [5, 3, 1, 2, 4]
square_list = []
for number in start_list:
    number = number**2
    square_list.append(number)
    square_list.sort()
print square_list

#This Next Part is Key
residents = {'Puffin' : 104, 'Sloth' : 105, 'Burmese Python' : 106}
print residents['Puffin'] 
print residents['Sloth']
print residents['Burmese Python']

#New Entries
menu = {} # Empty dictionary
menu['Chicken Alfredo'] = 14.50 # Adding new key-value pair
print menu['Chicken Alfredo']
menu['Spam']=2.5
menu['rice']=8.7
menu['noodle']=10
print "There are " + str(len(menu)) + " items on the menu."
print menu

#Changing Your Mind
zoo_animals = { 'Unicorn' : 'Cotton Candy House',
'Sloth' : 'Rainforest Exhibit',
'Bengal Tiger' : 'Jungle House',
'Atlantic Puffin' : 'Arctic Exhibit',
'Rockhopper Penguin' : 'Arctic Exhibit'} 
del zoo_animals['Unicorn']
a = zoo_animals
del a['Sloth']
del a['Bengal Tiger']
a['Rockhopper Penguin'] = 'Housing Exhibit'
print zoo_animals


#Remove a Few Things
backpack = ['xylophone', 'dagger', 'tent', 'bread loaf']
backpack.remove('dagger')
print backpack


#It's Dangerous to Go Alone! Take This
inventory = {
    'gold' : 500,
    'pouch' : ['flint', 'twine', 'gemstone'], # Assigned a newlist to 'pouch' key
    'backpack' : ['xylophone','dagger', 'bedroll','bread loaf']

}

# Adding a key 'burlap bag' and assigning a list to it
inventory['burlap bag'] = ['apple', 'small ruby', 'three-toed sloth']
inventory['pocket'] = ['seashell','strange berry','lint']
# Sorting the list found under the key 'pouch'
inventory['pouch'].sort() 
inventory['backpack'].sort()
inventory['backpack'].remove('dagger')
inventory['gold'] += 50
