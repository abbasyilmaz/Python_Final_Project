# Python_Final_Project
# TASK 1
data = [[1,'a',['cat'],2],[[[3]],'dog'],4,5]
A = []

def flatten(a):
    for i in a:
        if isinstance(i, list):
            flatten(i)
        else:
            A.append(i)

flatten(data)
print(A)

#TASK 2

input2 = [[1, 2], [3, 4], [5, 6, 7]]
liste = []

def reverse(a):
    a.reverse()
    for i in a:
        if isinstance(i,list):
            i.reverse()
            liste.append(i)
reverse(input2)
print(liste)
