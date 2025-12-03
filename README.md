```markdown
# 🔐 Password Manager – C Console Application

A lightweight command-line password manager written in C that securely stores credentials in an encrypted binary file. All usernames and passwords are XOR-encrypted before saving to disk. Works fully offline.

## 🚀 Features
- Master password authentication (`1234` by default)
- Add website login credentials
- Search stored credentials or view all
- Persistent encrypted storage (`passwords.dat`)
- Simple and fast local application

## 📂 Project Structure
```

PasswordManager/
├─ src/
│  └─ PasswordManager.c
├─ data/
│  └─ passwords.dat  (auto-generated, not stored in Git)
└─ README.md

````

## 🛠️ Build & Run

### Linux / macOS
```bash
gcc src/PasswordManager.c -o passwordmgr
./passwordmgr
````

### Windows (MinGW)

```bash
gcc src/PasswordManager.c -o passwordmgr.exe
passwordmgr.exe
```

## 🧩 Usage

1️⃣ Launch the program
2️⃣ Enter master password:

```
1234
```

3️⃣ Choose an action:

```
1 → Add new credential
2 → View or search saved credentials
3 → Exit
```

Credentials are automatically encrypted and saved into `passwords.dat`.

## 🔏 Encryption Information

XOR-based reversible encryption:

```c
#define ENCRYPTION_KEY 'X'
```

✔ Good for learning
⚠ Not suitable for real-world password storage

## 📌 Planned Improvements

* Stronger encryption (hashed master password, AES)
* Better input protection (mask password entry)
* Edit / delete stored credentials
* Backup & export support
* Input validations and UI improvements

## 👤 Author

**Aditya Dewangan**

```
```
