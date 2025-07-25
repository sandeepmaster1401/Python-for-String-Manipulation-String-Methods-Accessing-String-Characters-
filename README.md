1. What is a String in Python?
A string is a sequence of characters enclosed in single quotes ' ', double quotes " ", or triple quotes ''' ''' or """ """.

python
Copy
Edit
s1 = 'hello'
s2 = "world"
s3 = '''multiline
string'''


🔹 2. Accessing Characters in a String
Strings are indexed, starting from 0.

python
Copy
Edit
s = "Python"
print(s[0])  # P
print(s[1])  # y
print(s[-1]) # n (last character)
🔸 Slicing a String
python
Copy
Edit
print(s[0:3])  # Pyt
print(s[2:])   # thon
print(s[:4])   # Pyth
print(s[-3:])  # hon



🔹 3. Common String Methods
🟢 Changing Case
python
Copy
Edit
s = "hello world"
print(s.upper())      # HELLO WORLD
print(s.lower())      # hello world
print(s.capitalize()) # Hello world
print(s.title())      # Hello World


🟢 Removing Whitespaces
python
Copy
Edit
s = "  hello  "
print(s.strip())  # 'hello'
print(s.lstrip()) # 'hello  '
print(s.rstrip()) # '  hello'


🟢 Finding and Replacing
python
Copy
Edit
s = "banana"
print(s.find("na"))       # 2
print(s.replace("na", "xy"))  # baxyxy


🟢 Splitting and Joining
python
Copy
Edit
s = "a,b,c"
print(s.split(","))       # ['a', 'b', 'c']

words = ['I', 'love', 'Python']
print(" ".join(words))    # I love Python


🔹 4. String Concatenation
Joining strings together:

python
Copy
Edit
a = "Hello"
b = "World"
c = a + " " + b
print(c)  # Hello World


🔹 5. String Formatting
f-strings (Recommended)
python
Copy
Edit
name = "Sandeep"
age = 21
print(f"My name is {name} and I am {age} years old.")
.format()
python
Copy
Edit
print("My name is {} and I am {} years old.".format(name, age))


🔹 6. Checking String Properties
python
Copy
Edit
s = "Python3"

print(s.isalpha())  # False (contains a digit)
print(s.isdigit())  # False
print("123".isdigit())  # True
print("abc".isalpha())  # True


🔹 7. Looping Through a String
python
Copy
Edit
s = "AI"
for char in s:
    print(char)

    
🔹 8. Immutability of Strings
Strings are immutable – you can’t change characters directly:

python
Copy
Edit
s = "hello"
# s[0] = 'H' ❌ This will raise an error
# Instead:
s = 'H' + s[1:]  # Hello ✅


🔹 9. Useful String Methods (Quick Reference)
Method	Description
upper()	Converts to uppercase
lower()	Converts to lowercase
strip()	Removes spaces
replace(a,b)	Replaces a with b
split(',')	Splits by delimiter
join(list)	Joins list into a string
find('x')	Finds first index of 'x'
startswith()	Checks if string starts with value
endswith()	Checks if string ends with value
isalpha()	True if only letters
isdigit()	True if only digits


