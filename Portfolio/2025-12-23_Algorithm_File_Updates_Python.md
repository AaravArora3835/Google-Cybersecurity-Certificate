
# Algorithm for File Updates in Python

## Project Description

In this project, I developed a Python algorithm to manage an IP address allow list used to control access to a restricted subnetwork at a health care company. This subnetwork contains sensitive personal patient records, so maintaining accurate access controls is critical. The algorithm reads an existing allow list from a file, compares it against a predefined remove list, and removes any IP addresses that should no longer have access. After processing, the algorithm updates the original file to reflect the revised allow list, ensuring access permissions remain secure and up to date.

---

## Open the File That Contains the Allow List

```python
import_file = "allow_list.txt"

with open(import_file, "r") as file:
````

This code assigns the name of the allow list file to the variable `import_file` so it can be reused later in the program. The `open()` function opens the file in read mode (`"r"`), allowing its contents to be accessed without modifying them. The `with` statement ensures the file is automatically closed after it is read, which is a best practice for reliability and resource management. The file object is stored in the variable `file` while it is being accessed.

---

## Read the File Contents

```python
    ip_addresses = file.read()
```

The `.read()` method reads the entire contents of the file and returns them as a single string. This string contains all IP addresses currently on the allow list. Storing the contents in the variable `ip_addresses` makes it possible to process and modify the data in later steps of the algorithm.

---

## Convert the String into a List

```python
ip_addresses = ip_addresses.split()
```

The `.split()` method converts the string of IP addresses into a list by separating values based on whitespace. Converting the data into a list allows the algorithm to evaluate and remove individual IP addresses efficiently. Each IP address becomes a separate element in the list.

---

## Iterate Through the Remove List

```python
for element in remove_list:
```

This `for` loop iterates through each IP address stored in the `remove_list`. The loop variable `element` represents the current IP address being evaluated during each iteration. This structure allows the algorithm to systematically compare each remove-list IP against the allow list.

---

## Remove IP Addresses That Are on the Remove List

```python
    if element in ip_addresses:
        ip_addresses.remove(element)
```

The `if` statement checks whether the current IP address from the remove list exists in the allow list. If a match is found, the `.remove()` method deletes that IP address from the `ip_addresses` list. This conditional prevents errors by ensuring that only existing IP addresses are removed. Applying `.remove()` in this way is effective because the allow list does not contain duplicate IP addresses.

---

## Update the File with the Revised List of IP Addresses

```python
ip_addresses = "\n".join(ip_addresses)

with open(import_file, "w") as file:
    file.write(ip_addresses)
```

The `"\n".join(ip_addresses)` method converts the updated list back into a single string, placing each IP address on a new line. The file is then reopened in write mode (`"w"`), which overwrites the existing contents. The `.write()` method writes the revised allow list back to the file, ensuring that removed IP addresses no longer have access to the restricted subnetwork.

---

## Summary

This algorithm demonstrates how Python can be used to securely manage access control data stored in files. It begins by opening and reading an allow list file, then converts the file contents into a list for processing. A loop compares the allow list against a remove list and removes any unauthorized IP addresses. After modifications are complete, the updated list is converted back into a formatted string and written back to the original file. This approach helps maintain accurate access controls and supports secure handling of sensitive systems.
