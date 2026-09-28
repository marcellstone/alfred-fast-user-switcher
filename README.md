
<img width="764" height="284" alt="0_usage" src="https://github.com/user-attachments/assets/17480581-5c74-45c0-a739-b92d6f5a3884" />

# 🔄 Fast User Switcher

An Alfred workflow that controls the macOS Control Center to let you quickly switch between user accounts using just your keyboard.

## ⚠️ Prerequisites (Very Important)
For this workflow to recognize and click the correct menu, two macOS settings must be configured:

1. **Enable the Menu Bar Icon**
   - Go to  (Apple logo) > **System Settings** > **Control Center**.
   - Scroll down to **Fast User Switching** and set the dropdown to **'Show in Menu Bar (Icon)'**.
     <img width="400" height="auto" alt="1_menu_bar_settings" src="https://github.com/user-attachments/assets/aeccf7c2-cf8d-4d5e-a8de-64ce8ee8063a" />
     
   - You should see something like below in your menu bar.
     <img width="400" height="auto" alt="2_menu_bar" src="https://github.com/user-attachments/assets/965e8c59-7d48-432d-b291-769db47ca681" />

2. **Grant Accessibility Permissions**
   - Go to  > **System Settings** > **Privacy & Security** > **Accessibility**.
   - Ensure the toggle for **Alfred** is turned ON. (macOS may prompt you for this permission upon first run).
     <img width="400" height="auto" alt="3_privacy_settings" src="https://github.com/user-attachments/assets/8cb97010-4988-4641-801c-e331f25fd680" />

## ⚙️ Configuration
After installing, you must register your account list to match your Mac's environment.

* **USER_LIST**

  Look at the actual User Switching menu in your macOS menu bar. Type the account names **exactly in the order they appear from top to bottom**, placing one name per line.

  **[Example]**

  <img width="400" height="auto" alt="4_alfred_settings" src="https://github.com/user-attachments/assets/5f06c68b-1f42-4ef7-bc5c-f6c5d178b660" />

## 🚀 How to Use
1. Open Alfred and type the keyword `sw`.
2. Your configured user list will appear.
3. Select the target account using the arrow keys and press `Enter`. The account will switch instantly!

## 💡 Tips & Troubleshooting
* **The button blinks a few times:** This is the normal macOS visual feedback for menu clicks. The script is working perfectly.
* **I only hear a "ding" error sound:** Alfred's accessibility permissions might be glitched. Go to System Settings > Accessibility, remove Alfred entirely using the minus (`-`) button, and then add it back using the plus (`+`) button.
* **Touch ID Tip:** If you have a Mac with Touch ID, register different fingers for each account and enable 'Use Touch ID for fast user switching'. You won't even need to type your password!
