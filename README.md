# EXPERIMENT-6
## AIM:To write a Python program for checking Palindrome and to write test cases for ir. 

## ALGORITHM
Step 1: Start   
Step 2: Get an input from the user by prompting    
Step 3: Run a loop form 0 to len/2.   
Step 4: Check if the characters are the same both from the start and the end till len/2.   
Step 5: If it is, return the result that it is a palindrome.   
Step 6: Else, return that it is not a palindrome.    
Step 7: Stop. 

## PROGRAM
```
def Palindrome(string):
    for i in range(0, int(len(string) / 2)):
        if string[i] != string[len(string) - i - 1]:  # Fixed indexing
            return False
    return True


s = input("Enter a string: ")  # Added a prompt for clarity

c = 1
for i in s:
    if not i.isalpha():
        c = 0
        break  # Added break to stop checking after finding a non-alphabetic character

if c == 0:
    print("Enter a valid string")
    print("Test Case:Fail")
else:
    answer = Palindrome(s)
    if answer:
        print("The given string is a palindrome")
        print("Test Case:Pass")
    else:
        print("The given string is not a palindrome")
        print("Test Case:Pass") 
```

## OUTPUT
Alphanumeric values:

<img width="500" height="66" alt="427355149-d834feef-578f-4be2-9905-c59a88025030" src="https://github.com/user-attachments/assets/c64f08d4-836c-47ba-9e6e-05bffa97fae0" />

Numeric values:

<img width="301" height="74" alt="427355244-73468d2a-8b39-46b0-a0d5-431209ae173c" src="https://github.com/user-attachments/assets/4a953b6a-a3c2-4c60-981e-421153b2c1f5" />

Alphabet values:

<img width="356" height="72" alt="427355329-027e4bf0-7697-4cae-9f11-7d98192443f8" src="https://github.com/user-attachments/assets/f0203f2d-9898-42b3-b50a-0234e6ccb4b5" />

Non-palindrome string:

<img width="379" height="71" alt="427355393-b11b70ca-8240-4702-8452-023dd3d2acde" src="https://github.com/user-attachments/assets/fbc822ca-d030-43f2-a56c-db18e1ac413a" />

Symbols:

<img width="277" height="70" alt="427355466-885e5c23-70ee-46a3-bb4f-2c6cbedc1335" src="https://github.com/user-attachments/assets/f605fd61-bcee-4967-a006-d0789b650ce7" />


## RESULT
Thus, a program to check palindrome has been written and test cases have been written and verified successfully.
