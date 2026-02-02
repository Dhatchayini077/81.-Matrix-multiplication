# 81.-Matrix-multiplication
X = [
    [8, 5, 1],
    [9, 3, 2],
    [4, 6, 3]
]

Y = [
    [8, 5, 3],
    [9, 5, 7],
    [9, 4, 1]
]

# Initialize result matrix with zeros
result = [
    [0, 0, 0],
    [0, 0, 0],
    [0, 0, 0]
]

# Matrix multiplication
for i in range(len(X)):
    for j in range(len(Y[0])):
        for k in range(len(Y)):
            result[i][j] += X[i][k] * Y[k][j]

# Print result
print("Result of matrix multiplication:")
for row in result:
    print(row)
Output:
Result of matrix multiplication:
[107, 65, 46]
[111, 62, 52]
[106, 58, 43]
