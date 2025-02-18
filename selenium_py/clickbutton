from selenium import webdriver  #yeh browser control karta hai 
from selenium.webdriver.chrome.options import Options #yeh profile control karenga
from selenium.webdriver.common.action_chains import ActionChains #yeh click yeh saare action control karenga 
import time #yeh hum automation me delay dalne k liye use kiya jata hai 

# Set up Chrome options
#yeh code humne iss liye likha hai taaki hum yeh specific profile open kar sake 
chrome_options = Options()
chrome_options.add_argument(r"--user-data-dir=C:\Users\Uzma\AppData\Local\Google\Chrome\User Data")  # Path to Chrome user data
chrome_options.add_argument(r"--profile-directory=Profile 10")  # Specify the profile directory


#option me profile 10 ki details hai , webdriver ko yeh intialize karengev
driver = webdriver.Chrome(options=chrome_options)

# Open Google
driver.get("https://www.google.com")

#google k searbox ka attribrute ka naam q hota hai kyuke 
search_box = driver.find_element("name", "q")
search_box.send_keys("Selenium Python tutorial")

 #time to sleep to be added 
time.sleep(1)

search_box.submit()  # Alternative to using RETURN key


