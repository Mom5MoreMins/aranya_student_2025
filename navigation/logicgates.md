# Secure Entry System

A simple three-factor authentication: access is granted only if **keycard**, **PIN**, and **voice authorization** are all 1.

```python
def secure_entry_system(keycard: int, pin: int, voice_auth: int) -> int:
    """
    Return 1 (access granted) only if all three inputs are 1.
    Otherwise, return 0 (access denied).
    """
    return keycard & pin & voice_auth

if __name__ == "__main__":
    test_vectors = [
        (1, 1, 1),  # all valid → access granted
        (1, 1, 0),  # voice fails → access denied
        (0, 1, 1),  # keycard fails → access denied
        (1, 0, 1),  # PIN fails → access denied
    ]

    for k, p, v in test_vectors:
        print(f"secure_entry_system({k}, {p}, {v}) = {secure_entry_system(k, p, v)}")
```

```bash
$ python secure_entry_system.py
```

```
secure_entry_system(1, 1, 1) = 1
secure_entry_system(1, 1, 0) = 0
secure_entry_system(0, 1, 1) = 0
secure_entry_system(1, 0, 1) = 0
```
