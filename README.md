# Programming_Assingment-8


1. Write a Python Program to Add Two Matrices?
sol:
mat1 = [[1,2,3],
        [6, -4, -9],
        [3,6,9]]

mat2 = [[6,9,3],
        [1,-1,1],
        [0, 9, 11]]
result = []

for i in range(len(mat1)):
    row = []
    for j in range(len(mat1)):
        row.append(mat1[i][j]+mat2[i][j])
        
    result.append(row)
    
result
[[7, 11, 6], [7, -5, -8], [3, 15, 20]]



2. Write a Python Program to Multiply Two Matrices?
sol:
# Take 3x3 matrix
A = [[12, 7, 3],
    [4, 5, 6],
    [7, 8, 9]]

B = [[5, 8, 1, 2],
    [6, 7, 3, 0],
    [4, 5, 9, 1]]

result = [[0, 0, 0, 0],
        [0, 0, 0, 0],
        [0, 0, 0, 0]]

for i in range(len(A)):
    for j in range(len(B[0])):
        for k in range(len(B)):
            result[i][j] += A[i][k] * B[k][j]

for r in result:
    print(r)
[114, 160, 60, 27]
[74, 97, 73, 14]
[119, 157, 112, 23]



3. Write a Python Program to Transpose a Matrix?
sol:
# Program to transpose a matrix using a nested loop

X = [[12,7],
    [4 ,5],
    [3 ,8]]

result = [[0,0,0],
         [0,0,0]]

# iterating through rows
for i in range(len(X)):
   # iterating through columns
   for j in range(len(X[0])):
        result[j][i] = X[i][j]

for r in result:
    print(r)
[12, 4, 3]
[7, 5, 8]



4. Write a Python Program to Sort Words in Alphabetic Order?
sol:
try:
    sentance = input("Enter the words: ")
    words = [word.lower() for word in sentance.split()]
    words.sort()
    
    print("Sorted order of words:")
    for word in words:
        print(word, end = ' ')
    
except Exception as e:
    print(e)
Enter the words: This is task from the Assignment
Sorted order of words:
assignment from is task the this




5. Write a Python Program to Remove Punctuation From a String?
sol:
punctuations = '''!()-[]{};:'"\,<>./?@#$%^&*_~'''

string = input("Enter the string: ")

outputString = ""

for char in string:
    if char not in punctuations:
        outputString += char
        
print(outputString)
Enter the string: Hello, World!!! <HTML> c++; {braces} \/!@##^&*()( Ending the string now
  
  
  
Hello World HTML c++ braces  Ending the string now
