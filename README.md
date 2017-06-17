# Selenium-Drivers

### Exception in thread "main" java.lang.IllegalStateException: The path to the driver executable must be set by the webdriver.gecko.driver system property

### Setting up selenium Gecko drivers. 
    
     System.setProperty("webdriver.gecko.driver", "D:\\Firefox Driver\\geckodriver.exe");
     WebDriver driver = new FirefoxDriver(); 
     driver.get(https://www.facebook.com");
     
     System.out.println("App title: " +driver.getTitle());
     driver.quit();

### Important Interfaces and Classes of Selenium API. 

1. public Interface WebDriver  - The main interface to use for testing. It represents an idealized web browser. The methods in this class fall into 3 categories 

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

2. public Class Actions - The user facing API for emulating complex gestures. Use this class rather than using the Keyboard or 
Mouse directly. 
    
    Methods - 
    1. Actions sendKeys(String charSequence) - 
    1. Actions sendKeys(WebElment target, String charSequence) - 
    1. Action build() - Generates a composite action containing all actions so far, ready to be performed (and resets the internal          builder state, so subsequent calls to build() will contain fresh sequences).
    2. Actions click() - 
    3. Actions click(WebElement target) - 
    4. Actions clickAndHold() - 
    5. Actions contextClick() - 
    6. Actions doubleClick() - 
    7. Actions dragAndDrop(WebElement source, WebElement target) - 
    8. Actions dragAndDropBy(WebElement source, int xOffset, int yOffset)
    9. Actions keyDown() - 
    10. Actions keyUp() - 
    11. Actions moveToElement() - 
    
3. public class By - Mechanism used to locate elements within a document. In order to create your own locators subclass this class
and override the proptected methods as required. 

    Methods 
    1. static By id(String id) - 
    2. static By name(String name) - 
    3. static By className(String className) - 
    4. satic By cssSelector(String cssSelector) - 
    5. static By linkText(String text) -
    6. static By partialLinkText(String text) - 
    7. static By xpath(String xpath) - 
    8. String toString() - 
    
4. Select - Models a SELECT tag, providing helper methods to select and deselect options.

    Methods 
    1. void deselectAll() - clears all selected entries. 
    2. void deselectByIndex(int index) - deselect the option at a given index. 
    3. void deselectByValue(String value) - Deselect all options that have a value matching the argument.
    4. void deselectByVisibleText(java.lang.String text) - Deselect all options that display text matching the argument. 
    5. java.util.List<WebElement> getAllSelectedOptions() - 
    6. WebElement getFirstSelectedOption() - 
    

    

5. Capabilities 

6. DesiredCapabilities 

7. FirefoxDriver 

8. ChromeDriver 

9. InternetExplorerDriver 

10. HTML
