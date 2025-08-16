# File Permissions Task

## 🎯 Task
Understand Linux file permissions and create a flowchart for them. Then, apply the `chmod` command in Python to make the permissions `rwxrwxr-x`.

---

## 🔑 Explanation of Permissions
- **r = read (4)**
- **w = write (2)**
- **x = execute (1)**

`rwxrwxr-x` → Owner = rwx (7), Group = rwx (7), Others = r-x (5)  
**Octal = 775**

---

## 🛠 Python Implementation

```python
import os

file_path = "example.txt"
os.chmod(file_path, 0o775)
print("Permissions changed to rwxrwxr-x (775)")
