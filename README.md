
# 🛒 E-Commerce Website with Email OTP Verification

This is a simple e-commerce website project that demonstrates a user registration and login system with **email OTP verification** using PHP and PHPMailer.

## 🔐 Features

- ✅ User Login Authentication
- ✅ New User Registration with OTP Verification
- ✅ Email Integration using PHPMailer
- ✅ Forgot Password Functionality
- ✅ Clean UI with HTML/CSS
- ✅ Basic Client-Side Validation with JavaScript

## 📁 Project Structure

```
assignment/
├── index.html              # Login page
├── login.php               # Handles login authentication
├── register.html           # Registration form
├── register.php            # Sends OTP and processes registration
├── verify_otp.html         # OTP input form
├── verify_otp.php          # Verifies OTP and completes registration
├── forgot.html             # Forgot password page
├── forgot.php              # Handles forgot password logic
├── script.js               # JavaScript for validation
├── style.css / styles.css  # Styling files
├── image/                  # Folder for assets/images
├── phpmailer/              # PHPMailer library for sending email
```

## 🚀 How It Works

1. **Login Page (`index.html`)**  
   Users enter their username and password to log in.

2. **Registration Page (`register.html`)**  
   New users provide their details and receive an OTP via email.

3. **OTP Verification (`verify_otp.php`)**  
   Users input the OTP they received to complete registration.

4. **Forgot Password**  
   Users can request a password reset via email.

## 🛠 Setup Instructions

1. Clone or download this repository and place it in your `htdocs` folder (if using XAMPP).
2. Start **Apache** from XAMPP.
3. Make sure PHP has `openssl` enabled (in `php.ini`):
   ```ini
   extension=openssl
   ```
4. Configure your email credentials in `register.php` and `verify_otp.php`:
   ```php
   $mail->Host = 'smtp.gmail.com';
   $mail->Username = 'your-email@gmail.com';
   $mail->Password = 'your-app-password';
   ```
   > ⚠️ Use an App Password if you're using Gmail.

5. Open your browser and go to:  
   `http://localhost/assignment/index.html`

## 🔒 Notes

- Make sure to replace email credentials with your own.
- This project does not currently use a database. OTPs and user data are handled in memory or temporary variables.
- No password encryption is implemented – **do not use this in production without securing user data**.

## 💡 Future Enhancements

- Add MySQL database integration.
- Implement password hashing (e.g., bcrypt).
- Create product listing, cart, and checkout modules.
- Improve UI with responsive design.

---

### 📧 Contact

For any queries or contributions, feel free to reach out.
📺 [Watch Demo on YouTube](https://www.youtube.com/watch?v=ISwT6Ai4Q08)

