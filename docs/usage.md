# Usage Guide for Dtech Password Generator

The Password Generator package allows you to create secure and customizable passwords with ease. This guide provides detailed examples and usage scenarios to help you make the most of the package.

## Installation

To install the package, use pip:

```bash
pip install dtech-password-generator
```

---

#### 3. **Basic Usage**

```markdown
## Basic Usage

Import the package and use the `password` function to generate random passwords:

```python
from dtech_password_generator import password

# Generate a default password of 10 characters
print(password())  # Example: 'qCcM#071H3'

# Generate a password with a specific length
print(password(16))  # Example: 'BN3bz7+JkP1N2!'
```


---

#### 4. **Handling Edge Cases**

```markdown
## Handling Edge Cases

The `password` function enforces secure password lengths between 7 and 35 characters. 

If an invalid length is provided, an error message will be returned:

```python
print(password(5))  # Output: 'Length must be within 7 and 35'
print(password(60))  # Output: 'Length must be within 7 and 35'
```

---

#### 5. **Advanced Usage**
The module can be integrated with python applications in different use cases. 

```markdown
## Advanced Usage

You can assign generated passwords to variables and use them in your applications:

```python
# Assigning a password to a variable
user_password = password(20)

# Use it for account creation or storage
print(f"Generated password for the new user: {user_password}")
```

---

#### 6. **FAQs**

```markdown
## FAQs

### Q: What happens if I don’t pass a length to the `password` function?
A: The default length of 10 characters is used.

### Q: Can I generate a password with only numbers or letters?
A: The current version generates passwords with a mix of letters, numbers, and special characters. You can extend the function to allow specific character sets. Newer versions will be released to allow numbers/spacial-characters/letters only.

### Q: Does the package support Python 2?
A: No, this package supports Python 3.6 and above.

```

7. #### **Examples**

### Example 1: Generate a 10-character password
```python
from password_generator import password
print(password())  # Example output: '2?QF7W[k'
```
### Invalid Length
```python
print(password(5))  # Output: 'Length must be within 7 and 40'
print(password(37))  # Output: 'Length must be within 7 and 40'
```


---

#### 8. **Contribution**
Feel free to contribute to this project.

```markdown
## Contribution

We welcome contributions to improve the package! If you’d like to add features or fix bugs, please:
- Fork the repository
- Create a feature branch
- Submit a pull request
```
