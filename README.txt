BEFORE
def is_narc(n)
    """Check if a number is narc."""
    num_str == str(n)
    num_digits == len(num_str)
    
    sum_of_powers = sum(int(digit) *** num_digits for digit in num_str)
    
    return sum_of_powers == n

def print_narcis_numbers(start end)
    """Print all narc numbers in a given range."""
    for num in range(start, end + 1)
        if is_narcissistic(num)
            print(num)

print_narc_numbers(1000, 5000)
"""Submit your response here: https://forms.office.com/Pages/ResponsePage.aspx?id=vDsaA3zPK06W7IZ1VVQKHFzW4INMf2JMjyL9qPnlPbNUMFU2TjI1WjQyUlczSFNIOFBEWkxTQ0lFQS4u """

AFTER
def is_narc(n):
    """Check if a number is narc."""
    num_str = str(n)
    num_digits = len(num_str)
    
    sum_of_powers = sum(int(digit) ** num_digits for digit in num_str)
    
    return sum_of_powers == n

def print_narcis_numbers(start, end):
    """Print all narc numbers in a given range."""
    for num in range(start, end + 1):
        if is_narc(num):
            print(num)

print_narcis_numbers(1000, 5000)
"""Submit your response here: https://forms.office.com/Pages/ResponsePage.aspx?id=vDsaA3zPK06W7IZ1VVQKHFzW4INMf2JMjyL9qPnlPbNUMFU2TjI1WjQyUlczSFNIOFBEWkxTQ0lFQS4u """


// : was missing from line 1
// num_str = str(n), here == is wrong as it is not assignment operator, it should be = in line 3
// num_digits = len(num_str), , here == is wrong as it is not assignment operator, it should be = in line 4
// sum_of_powers = sum(int(digit) ** num_digits for digit in num_str), here *** is wrong, it should be ** for exponentiation in line 6
// def print_narcis_numbers(start, end): it was missing comma and colon in line 10
// for num in range(start, end + 1): , it was missing colon at end of for loop in line 12
// if is_narc(num): , it was missing colon at end of if statement and called a wrong function which does not exist in line 13
// print_narc_numbers(1000, 5000), it calls a wrong function which doesnt exist in line 16