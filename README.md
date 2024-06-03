#Input matrices
#Matrix1 and Matrix2 should have same length 
matrix_1 = [[3,4],[5,6],[7,8]]
matrix_2 = [[0,1],[1,2],[3,4]]

#Empty matrices for operations 
matrix_sum = [[0,0],[0,0],[0,0]]
matrix_dif = [[0,0],[0,0],[0,0]]
matrix_mul = [[0,0],[0,0],[0,0]]
matrix_div = [[0,0],[0,0],[0,0]]

#Defining 

#Addition 
def add():
    for i in range(len(matrix_1)):
        for j in range(len(matrix_2[0])):
            matrix_sum[i][j] = matrix_1[i][j] + matrix_2[i][j]
    print ("Matrix Sum :",matrix_sum)

#Subtraction
def dif():
    for i in range(len(matrix_1)):
        for j in range (len(matrix_2[0])):
            matrix_dif[i][j] = matrix_1[i][j] - matrix_2[i][j]
    print("Matrix Difference :",matrix_dif)

#Multiplication
def mul():
    for i in range(len(matrix_1)):
        for j in range(len(matrix_2[0])):
            matrix_mul[i][j] = matrix_1[i][j] * matrix_2[i][j]
    print("Matrix Multiplication:",matrix_mul)

 #Division 
def div():
    for i in range(len(matrix_1)):
        for j in range(len(matrix_2[0])):
            if matrix_2[i][j] == 0:
                matrix_2[i][j] = 0
            else:
                matrix_div[i][j] = matrix_1[i][j] / matrix_2[i][j] 
    print("Matrix Division :",matrix_div)  

#Running Code and Output
add()
dif()
mul()
div()
