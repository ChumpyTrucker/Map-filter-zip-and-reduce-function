# Map-filter-zip-and-reduce-function
#Map function
from functools import reduce
my_list = [1,2,3]
your_list = [10,20,30]
their_list = [100,200,300]
def multiply_by2(item):
  return item*2

print(list(map(multiply_by2, my_list)))
print(my_list) 

#Filter function
my_list = [1,2,3]
def only_odd(item):
  return item % 2 != 0

print(list(filter(only_odd, my_list)))
print(my_list)

#Zip function
print(list(zip(my_list, your_list, their_list)))
print(my_list)

#Reduce function
def accumulator(acc, item):
  return acc + item
  print(acc, item)

print(reduce(accumulator, your_list, 5))
print(my_list)
