# Internship
#Password Generator Python
import random
import string

def generate_password(length=12):
    characters = string.ascii_letters + string.digits + string.punctuation
    password = ''.join(random.choice(characters) for _ in range(length))
    return password

def main():
    print("Welcome to the Password Generator!")
    while True:
        try:
            num_passwords = int(input("How many passwords would you like to generate? "))
            password_length = int(input("Enter the length of each password: "))
            break
        except ValueError:
            print("Please enter a valid number.")

    print("\nGenerating Passwords:")
    for i in range(num_passwords):
        password = generate_password(password_length)
        print(f"Password {i+1}: {password}")

if __name__ == "__main__":
    main()


https://github.com/Sailokesh3069/Internship/assets/162870856/b640ee78-80ce-4894-8172-807d39c6e9de

![Screenshot (2)](https://github.com/Sailokesh3069/Internship/assets/162870856/8a1c0a1a-8926-42de-bcff-613f6184c4a2)
