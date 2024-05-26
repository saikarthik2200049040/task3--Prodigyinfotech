import re

def check_password_complexity(password):
    # Define criteria
    length_criteria = len(password) >= 8
    uppercase_criteria = re.search(r'[A-Z]', password)
    lowercase_criteria = re.search(r'[a-z]', password)
    digit_criteria = re.search(r'\d', password)
    special_character_criteria = re.search(r'[!@#$%^&*()-_+=\[\]{}|\\:;"\',.<>?/~]', password)

    # Check each criteria
    if length_criteria and uppercase_criteria and lowercase_criteria and digit_criteria and special_character_criteria:
        return "Strong password"
    else:
        return "Weak password"

# Example usage
password = input("Enter your password: ")
result = check_password_complexity(password)
print(result)
