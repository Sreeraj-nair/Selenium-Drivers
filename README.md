# Selenium-Drivers

### Exception in thread "main" java.lang.IllegalStateException: The path to the driver executable must be set by the webdriver.gecko.driver system property

### Setting up selenium Gecko drivers. 
    
     System.setProperty("webdriver.gecko.driver", "D:\\Firefox Driver\\geckodriver.exe");
     WebDriver driver = new FirefoxDriver(); 
     driver.get(https://www.facebook.com");
     
     System.out.println("App title: " +driver.getTitle());
     driver.quit();

### Important Interfaces and Classes of Selenium API. 

1. WebDriver (Interface) - The main interface to use for testing. It represents an idealized web browser. The methods in this class 
fall into 3 categories 

    * Control of the browser itself
    * Selection of WebElements 
    * Debugging aids
    
    Some of the important methods of 
    1. void close() - Close the current window, quitting the browser if it's the last window currently open.
    2. WebElement findElement(By by) - Find the first WebElement using the given method.
    3. java.util.List<WebElement> findElements(By by) - Find all elements within the current page using the given mechanism.
    4. void get(java.lang.String url) - Load a new web page in the current browser window. 
    5. String getCurrentUrl() - Get a string representing the current URL that the browser is looking at.
    6. String getPageSource() - Get the source of the last loaded page.
    7. String getTitle() - The title of the current page.
    8. String getWindowHandle() - Return an opaque handle to this window that uniquely identifies it within this driver instance.
    9. java.util.Set<java.lang.String> getWindowHandles() - Return a set of window handles which can be used to iterate over all open       windows of this WebDriver instance by passing them to switchTo().WebDriver.Options.window()
    10. Driver.navigate().to(String url) - Abstraction to navigate forward, back. 
    11. WebDriver.TargetLocator switchTo() - Send future commands to a different frame or window. 

2. Actions 

3. By 

4. Select 

5. Capabilities 

6. DesiredCapabilities 

7. FirefoxDriver 

8. ChromeDriver 

9. InternetExplorerDriver 

10. HTML
