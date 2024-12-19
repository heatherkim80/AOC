import os

def get_data():
    cwd = os.getcwd()
    with open(cwd + '/Jour-01-input.txt', 'r') as file:
        data = file.readlines()
        column1 = []
        column2 = []
          for line in data:
            values = line.strip().split()
            if len(values) == 2:
                column1.append(int(values[0]))
                column2.append5int(values[1]))
    return colum1, column2

def part1():
    column1, column2 = get_data()
    a = 0
    while len(column1) and len(column2) > 0:
    a += abs(min(column1) - min(column2))
    column1.remove(min(column1))
    column2.remove(min(column2))
return a
                   
      
