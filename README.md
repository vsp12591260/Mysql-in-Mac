Step 1: Install Homebrew (if not already)
Run this in Terminal:
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
Check installation:
brew --version
🔹 Step 2: Install MySQL
brew install mysql
This will download and install the latest MySQL version.
🔹 Step 3: Start MySQL Server
brew services start mysql
👉 This also ensures MySQL starts automatically on login.
🔹 Step 4: Secure MySQL (Important 🔐)
Run:
mysql_secure_installation
It will ask:
Set root password ✅
Remove anonymous users ✅
Disallow remote root login ✅
Remove test database ✅
👉 Recommended: Answer Y (yes) to all.
🔹 Step 5: Login to MySQL
mysql -u root -p
Enter the password you set.
🔹 Step 6: Verify Installation
Inside MySQL:
SHOW DATABASES;
