## 1.find the root of quadratic equation

print("general equation ax^2+bx+c:")
def roots(a,b,c):
    
    #find discriminant
    d=(b**2-(4*a*c))
    if (d>=0):
        #find roots
        sol1=(-b+(d**0.5)/(2*a))
        sol2=(-b-(d**0.5)/(2*a))
        return sol1,sol2
    else:
        #real part+imaginary part
        realpart=(-b/(2*a))
        imaginarypart=((d**0.5)/(2*a))
        sol1=complex(realpart,imaginarypart)
        sol2=complex(realpart,-imaginarypart)
        return sol1,sol2
        
a=float(input("enter the value of a:"))
b=float(input("enter the value of b:"))
c=float(input("enter the value of c:"))
A=roots(a,b,c)
print("roots",A)




## 2.a)check if n is prime
##  b)generate allprime numbers till n
## c) generate first n prime numbers
## use function for everyone

def prime(num):
    p=0
    for i in range(2,num):
        if (num%i==0):
            p=1
            print("not prime")
            break
    if (p==0):
            print("prime")
num=int(input("enter the value:"))
prime(num)






def prime_upto_number(num):
   
    for i in range(2,num+1):
        if (num%i!=0):
          primes.append(i)
primes=[]
num=int(input("enter the value:"))
prime_upto_number(num)
print(primes)






def is_prime(num):
    """Check if a number is prime."""
    if num < 2:
        return False
    for i in range(2,num):
        if num % i == 0:
            return False
    return True

def generate_primes(n):
    """Generate the first n prime numbers."""
    primes = []
    current_num = 2  # Start with the first prime number
    while len(primes) < n:
        if is_prime(current_num):
            primes.append(current_num)
        current_num += 1
    return primes


num_primes = int(input("Enter the number of prime numbers to generate: "))


result = generate_primes(num_primes)
print(f"The first {num_primes} prime numbers are: {result}")


## 3.pattern
       *
     * * * 
   * * * * *
 * * * * * * *
* * * * * * * * *
n=5
for i in range(n):
    for j in range(i,n):
        print(" ",end=" ")
    for j in range(i):
        print("*",end=" ")
    for j in range(i+1):
        print("*",end=" ")
    print()




   * * * * * * * * *
     * * * * * * *
      * * * * *
        * * *
          *
 n= 5
for i in range(n):
    for j in range(i + 1):
        print(" ", end=" ")
    for j in range(i, n):
        print("*", end=" ")
    for j in range(i, n - 1):
        print("*", end=" ")
    print()



    

## 4.a)print whether the character is a letter or numeric digit or a special character 

char = input("Enter a character: ")

# Check if the character is a letter
if 'a' <= char <= 'z' or 'A' <= char <= 'Z':
    print(f"{char} is a letter.")
# Check if the character is a numeric digit
elif '0' <= char <= '9':
    print(f"{char} is a numeric digit.")
# If it's not a letter or numeric digit, consider it a special character
else:
    print(f"{char} is a special character.")


    
## b) if the character is a letter,print whether the letter is uppercase or lowercase
char = input("Enter a character: ")

# Check if the character is a letter
if 'a' <= char <= 'z' or 'A' <= char <= 'Z':
    print(f"{char} is a letter.")



## c)if character is numeric digit ,print its name in text(eg if input is 9, output is NINE.

# Accept a character from the user
char = input("Enter a character: ")

# Check if the character is a numeric digit
if '0' <= char <= '9':
    # Dictionary mapping numeric digits to their names
    digit_names = {'0': 'ZERO', '1': 'ONE', '2': 'TWO', '3': 'THREE', '4': 'FOUR', '5': 'FIVE', '6': 'SIX', '7': 'SEVEN', '8': 'EIGHT', '9': 'NINE'}

    # Print the name of the numeric digit
    print(f"{char} is {digit_names[char]}.")
else:
    print(f"{char} is not a numeric digit.")

## 5.operation on a string 

## a) find the frequency of a character on a string 
    
# Accept a string from the user
input_string = input("Enter a string: ")

# Accept a character whose frequency needs to be checked
char_to_find = input("Enter the character to find its frequency: ")

# Initialize a counter variable
char_frequency = 0

# Iterate through the string
for char in input_string:
    # Check if the current character matches the one we're looking for
    if char == char_to_find:
        char_frequency += 1

# Print the result
print(f"The frequency of '{char_to_find}' in the string is: {char_frequency}")

## b)replace the character by another character in a string

# Accept a string from the user
input_string = input("Enter a string: ")

# Accept the character to be replaced
char_to_replace = input("Enter the character to be replaced: ")

# Accept the character to replace with
replacement_char = input("Enter the character to replace with: ")

# Initialize an empty string to store the result
result_string = ""

# Iterate through the input string
for char in input_string:
    # Check if the current character is the one to be replaced
    if char == char_to_replace:
        # If yes, append the replacement character to the result string
        result_string += replacement_char
    else:
        # If no, simply append the current character to the result string
        result_string += char

# Print the resulting string
print(f"The modified string is: {result_string}")


or  

a=input("enter the string")
b=input("you want replace")
c=input("char on replace ")
result=""
for char in a:
    if char==b:
        result+=c
        
    else:
        result+=char
print(f"The modified string is: {result}")



## c)remove the first occurence of the string








## d) remove all occurence of a character from a string


          
