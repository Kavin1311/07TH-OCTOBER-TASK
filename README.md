# 07TH-OCTOBER-TASK
# TC_01
```
import time
from selenium import webdriver
from selenium.webdriver.common.by import By
from selenium.webdriver.support.ui import WebDriverWait
from selenium.webdriver.support import expected_conditions as EC
options = webdriver.ChromeOptions() 
options.add_argument("--incognito")
driver = webdriver.Chrome(options=options) 
driver.get("https://www.saucedemo.com/")
driver.find_element(By.ID,"user-name").send_keys("standard_user")
driver.find_element(By.ID,"password").send_keys("secret_sauce")
driver.find_element(By.ID,"login-button").click()

time.sleep(20)
```

<img width="1019" height="800" alt="image" src="https://github.com/user-attachments/assets/66afaed9-046a-435e-bc40-42773158264b" />
# LOGGED IN SUCCESSFULLY


# TC_02
<img width="621" height="52" alt="image" src="https://github.com/user-attachments/assets/f21c33a8-d272-49b9-8fec-f461b73eb216" />
```
import time
from selenium import webdriver
from selenium.webdriver.common.by import By

driver = webdriver.Chrome()
driver.get("https://the-internet.herokuapp.com/javascript_alerts?utm_source=chatgpt.com")
driver.find_element(By.XPATH,"//button[text()='Click for JS Confirm']").click()
alert= driver.switch_to.alert
alert.accept()
time.sleep(60)
```
<img width="891" height="774" alt="image" src="https://github.com/user-attachments/assets/2d522517-67bf-4234-be3b-3906fa7bb8cb" />

# TC_03
<img width="684" height="65" alt="image" src="https://github.com/user-attachments/assets/e0c77054-31ef-41fe-aae1-67754500d1d5" />
```
import time
from selenium import webdriver
from selenium.webdriver.common.by import By

driver = webdriver.Chrome()
driver.get("https://the-internet.herokuapp.com/javascript_alerts?utm_source=chatgpt.com")
driver.find_element(By.XPATH,"//button[text()='Click for JS Confirm']").click()
alert= driver.switch_to.alert
alert.dismiss()
time.sleep(60)
```
<img width="1021" height="849" alt="image" src="https://github.com/user-attachments/assets/42006af5-468c-4d35-bd65-614d81a02644" />

# TC_04
<img width="742" height="70" alt="image" src="https://github.com/user-attachments/assets/03d6d1d7-0867-45ee-b0ed-0c07aba0a2bd" />
```
import time 
from selenium import webdriver
from selenium.webdriver.common.by import By

driver = webdriver.Chrome()

driver.get("https://the-internet.herokuapp.com/javascript_alerts")
driver.find_element(By.XPATH, "//button[text()='Click for JS Prompt']").click()
alert = driver.switch_to.alert
alert.send_keys("Kavin")

alert.accept()
time.sleep(20)
```
<img width="1027" height="833" alt="image" src="https://github.com/user-attachments/assets/965e0941-1f40-443a-9fd9-28b7c0a3bbde" />

# TC_05
<img width="700" height="54" alt="image" src="https://github.com/user-attachments/assets/2af1d6cd-9f59-47cf-9d1a-58d1ea889593" />
```
from selenium import webdriver
from selenium.webdriver.common.by import By
from selenium.webdriver.common.action_chains import ActionChains

driver = webdriver.Chrome()

driver.get("https://the-internet.herokuapp.com/hovers")

element = driver.find_element(By.XPATH, "(//div[@class='figure'])[1]")

ActionChains(driver).move_to_element(element).perform()
```
<img width="557" height="425" alt="WhatsApp Image 2026-10-07 at 2 44 40 PM" src="https://github.com/user-attachments/assets/dd70de4f-ca59-485e-949a-fcd45a38b335" />



# TC_06
<img width="767" height="61" alt="image" src="https://github.com/user-attachments/assets/f3dffbf2-8cb6-4f37-bdf1-4a7847b57289" />
```
import time
from selenium import webdriver
from selenium.webdriver.common.by import By
from selenium.webdriver.common.action_chains import ActionChains

driver = webdriver.Chrome()

driver.get("https://demoqa.com/buttons")

element = driver.find_element(By.ID, "doubleClickBtn")

ActionChains(driver).double_click(element).perform()

time.sleep(200)
```
<img width="648" height="556" alt="image" src="https://github.com/user-attachments/assets/75fb5d85-36de-457c-b8f2-4f2f87fc9db6" />


# TC-08
```
import time 
from selenium import webdriver
from selenium.webdriver.common.by import By
from selenium.webdriver.support.ui import WebDriverWait
from selenium.webdriver.support import expected_conditions as EC
driver=webdriver.Chrome()
driver.get("https://www.amazon.in")
driver.find_element(By.ID,"twotabsearchtextbox").send_keys("Projector")
driver.find_element(By.ID, "nav-search-submit-button").click()
wait=WebDriverWait(driver,10)
product = wait.until(
    EC.visibility_of_element_located(
        (By.CSS_SELECTOR, "[data-component-type='s-search-result']")
    )
)
time.sleep(5)
```
<img width="468" height="439" alt="WhatsApp Image 2026-10-07 at 2 47 11 PM" src="https://github.com/user-attachments/assets/f35c3626-9c5f-4465-b74d-eb33b1e472c9" />

# TC-09
```
from selenium import webdriver
from selenium.webdriver.common.by import By
from selenium.webdriver.common.action_chains import ActionChains
import time

driver = webdriver.Chrome()

driver.get("https://the-internet.herokuapp.com/hovers")

time.sleep(2)

element = driver.find_element(By.XPATH, "(//div[contains(@class,'figure')])[1]")

ActionChains(driver).move_to_element(element).perform()

time.sleep(200)
```

<img width="993" height="857" alt="image" src="https://github.com/user-attachments/assets/aa850f7a-0a6a-4ff0-ae8b-239241e715ec" />

# TC-10
```
import time
from selenium import webdriver
from selenium.webdriver.common.by import By
from selenium.webdriver.support.ui import WebDriverWait
from selenium.webdriver.support import expected_conditions as EC

driver = webdriver.Chrome()

driver.get("https://the-internet.herokuapp.com/javascript_alerts")

driver.find_element(By.XPATH, "//button[text()='Click for JS Alert']").click()

alert = WebDriverWait(driver, 10).until(EC.alert_is_present())

alert.accept()

time.sleep(10)
```

<img width="942" height="823" alt="image" src="https://github.com/user-attachments/assets/8b95e9c6-0b0a-4133-b31e-a2411c8bec1c" />
