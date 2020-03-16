# LTL-Quote-Automator
A program that will auto generate quotes from multiple websites, developed with Selenium, tkinter, and python.

General Setup:
1. Make sure to install the correct chromedriver for your browser. (https://chromedriver.chromium.org/getting-started)
2. Make sure the driver is in the same folder and the python file. 

3. Set the file path to the location of the chrome driver.     
(From within the code)
driver = webdriver.Chrome(r"C:\Users\USERNAME\Desktop\FOLDER\chromedriver")

4. Change the username and password credentials for each site. 
(from within the code)
#1st Tab Login Page
driver.find_element(By.XPATH, "//button[@id='dropdownMenuButton']").click()
driver.find_element(By.XPATH, "//input[@id='UserName']").send_keys('**********') #replace with your own username
driver.find_element(By.XPATH, "//input[@id='Password']").send_keys('**********') #replace with your own password
    
    


