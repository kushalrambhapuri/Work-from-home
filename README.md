# Work from home automation bot
Now you can rest easy while your laptop stays active all day! This simple Python script automates basic mouse and keyboard activity to ensure your system doesn’t go idle.
I created this bot using PyCharm, a popular Python code editor. Follow the steps below to replicate this automation on your own system:
Prerequisites
Python Installed: Ensure Python is installed on your system.
Install PyAutoGUI: Open the terminal and run the following command:
pip install pyautogui
Code Explanation
Importing Libraries: At the beginning of the script, the required libraries are imported:
import pyautogui  
import time  
Disable Fail-Safe: The following line ensures the program doesn't stop if the mouse is moved to the corner of the screen:
pyautogui.FAILSAFE = False  
Infinite Loop: The main functionality is contained within an infinite loop:
while True:  
    # Pause for 300 seconds (5 minutes)  
    time.sleep(300)  
    
    # Simulate mouse movement  
    for i in range(0, 100):  
        pyautogui.moveTo(0, i * 5)  
    
    # Simulate keyboard activity  
    for i in range(0, 3):  
        pyautogui.press('shift')  
Mouse Movement: The moveTo function simulates mouse activity by moving the cursor in small increments.
Keyboard Input: The press function simulates pressing the Shift key three times, which doesn't perform any actual action but keeps the system awake.
How It Works
Once you run this script, it will:

Move the mouse cursor slightly every 5 minutes.
Simulate pressing the Shift key to keep the system awake.
Notes
This script is designed for personal use and works well for preventing system inactivity.
Always use such automation responsibly, and ensure it adheres to your workplace or personal policies.
Enjoy your well-deserved rest while your laptop stays active!
