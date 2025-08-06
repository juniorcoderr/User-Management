### 🔐 Linux User Account Creation Script

This Bash script automates the process of creating a new user on a Linux system. It is designed to be executed with root privileges and allows you to:

* Create a user with a specified username
* Add optional comments (like full name or purpose)
* Automatically generate a secure password
* Set the password and force the user to change it on first login
* Display the username, password, and hostname after successful creation

---

### 📂 Usage

```bash
sudo ./create_user.sh USERNAME [COMMENT]
```

**Example:**

```bash
sudo ./create_user.sh john_doe "John Doe - Developer Account"
```

---

### ⚙️ Features

* Root permission check
* Validates arguments
* Random password generation using `sha256sum`
* Portable password setting using `chpasswd`
* First-login password reset enforcement
* Clean summary of created account

---

### 🛡️ Note

This script is intended for **administrative use in trusted environments**. The generated password is displayed in plain text; ensure it is handled securely.
