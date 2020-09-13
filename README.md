# Light Truck Load Quote Automator
A program that will auto generate quotes from multiple websites, developed with Selenium, tkinter, and python.

General Setup:
1. Make sure to install the correct chromedriver for your browser. (https://chromedriver.chromium.org/getting-started)
2. Make sure the driver is in the same folder as the python file. 

3. Set the file path to the location of the chrome driver.     
(From within the code)
driver = webdriver.Chrome(r"C:\Users\USERNAME\Desktop\FOLDER\chromedriver")

4. Change the username and password credentials for each site. 
(from within the code)
#1st Tab Login Page
driver.find_element(By.XPATH, "//button[@id='dropdownMenuButton']").click()
driver.find_element(By.XPATH, "//input[@id='UserName']").send_keys('**********') #replace with your own username
driver.find_element(By.XPATH, "//input[@id='Password']").send_keys('**********') #replace with your own password
    
Usage:
1. Input Origin and Destination zipcode.
2. Input values for Handling Unit, Pieces, Description, Length, Width, Height, Weight. You can press the "Caculate Class" to auto calculate the value for Class if Length, Width, Height, and Weight have been entered.
3. A test entry set is 1, 1, engine, 60, 42, 60, 2256, 65. 
4. Click "Add Set" to confirm the data set. If there are multiple sets of data, click "Add Set" after inputting eaching set.
5. Click "Get Quote" to generate quotes from the Chrome Browser. A brower session will open indicating that "Chrome is being controlled by automated test software. The program should correctly iterate through the data-sets, input the data into the entry fields and generate a quote for the first website. A total of three tabs should open.



