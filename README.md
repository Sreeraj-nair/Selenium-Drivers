# Selenium-Drivers

## Exception in thread "main" java.lang.IllegalStateException: The path to the driver executable must be set by the webdriver.gecko.driver system property

## Setting up selenium Gecko drivers. 
    
     System.setProperty("webdriver.gecko.driver", "D:\\Firefox Driver\\geckodriver.exe");
     WebDriver driver = new FirefoxDriver(); 
     driver.get(https://www.facebook.com");
     
     System.out.println("App title: " +driver.getTitle());
     driver.quit();
     
