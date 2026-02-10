# Infix Expression Evaluation using Stack

def apply_operator(op, b, a):
    if op == '+':
        return a + b
    if op == '-':
        return a - b
    if op == '*':
        return a * b
    if op == '/':
        return a / b

def precedence(op):
    if op == '+' or op == '-':
        return 1
    if op == '*' or op == '/':
        return 2
    return 0

def evaluate_infix(expression):
    operands = []
    operators = []

expr = input("Enter infix expression (single digit operands): ")
result = evaluate_infix(expr)
print("Result of the expression is:", result)# Data-Structure-03
Enter infix expression (single digit operands): 2+3*4
Result of the expression is: 14
