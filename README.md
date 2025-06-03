# task-6
Password Strength Evaluation Report
Objective:
To understand what constitutes a strong password and evaluate its strength using online tools.

 Passwords Created for Evaluation:
Simple Password: password123

Moderate Complexity: Summer2025!

High Complexity: G7r$2nV!lQ9zX8

Passphrase: BlueSky$Dances!UnderMoon

Randomly Generated: 9u$W2f!Kq8Zx@L

 Evaluation Using Online Password Strength Checker:
Using the online tool PasswordMeter, the following evaluations were made:

Password	Strength Score	Feedback
password123	Weak	Common password; easily guessable.
Summer2025!	Moderate	Contains uppercase, numbers, and symbols; still predictable.
G7r$2nV!lQ9zX8	Strong	High entropy; includes uppercase, lowercase, numbers, and symbols.
BlueSky$Dances!UnderMoon	Very Strong	Long passphrase; highly unpredictable.
9u$W2f!Kq8Zx@L	Very Strong	Randomly generated; high complexity.

 Analysis and Best Practices:
Length Over Complexity: Longer passwords are generally more secure. Aim for at least 16 characters. 
cisa.gov
+3
the-sun.com
+3
it.ucsb.edu
+3

Avoid Common Patterns: Passwords like password123 are easily guessable. 
cu.edu

Use Passphrases: Combining unrelated words can create memorable yet strong passwords. 
cyber.gc.ca

Randomness is Key: Randomly generated passwords with a mix of characters are harder to crack. 
acaglobal.com

Unique Passwords for Each Account: Reusing passwords increases vulnerability. 
cisa.gov
+1
acaglobal.com
+1

 Python Code to Check Password Strength:
python

import re

def check_password_strength(password):
    if len(password) < 12:
        return "Weak: Password must be at least 12 characters long."
    if not re.search(r"[a-z]", password):
        return "Weak: Password must contain at least one lowercase letter."
    if not re.search(r"[A-Z]", password):
        return "Weak: Password must contain at least one uppercase letter."
    if not re.search(r"[0-9]", password):
        return "Weak: Password must contain at least one digit."
    if not re.search(r"[!@#$%^&*(),.?\":{}|<>]", password):
        return "Weak: Password must contain at least one special character."
    return "Strong: Password meets all criteria."

# Test the function
passwords = ["password123", "Summer2025!", "G7r$2nV!lQ9zX8", "BlueSky$Dances!UnderMoon", "9u$W2f!Kq8Zx@L"]
for pwd in passwords:
    print(f"Password: {pwd} -> {check_password_strength(pwd)}")
 Summary of Findings:
Password Length: Longer passwords are more secure.

Character Variety: Mixing uppercase, lowercase, numbers, and symbols enhances strength.

Avoid Predictable Patterns: Steer clear of common words and sequences.
thesun.co.uk
+4
cu.edu
+4
acaglobal.com
+4

Use Passphrases: They are easier to remember and can be very strong.
cyber.gc.ca

Regular Updates: Change passwords periodically to maintain security.
