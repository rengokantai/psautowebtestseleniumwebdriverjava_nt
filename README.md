# psautowebtestseleniumwebdriverjava_nt
```
By.cssSelector("a.headername")).click();
By.linkText("sign in").click();
By.id("username")).clear();
By.id("username")).sendKeys("rengokantai");
By.id("login").click();
```

need to download firefox driver.
geckodriver
```
System.setProperty("webdriver.gecko.driver","C:/dev/tool/geckodriver.exe");
```

or set
```
GECKO_PATH
```

### A More Complex Script
```
WebElement sf = sriver.findElement(By.id(""));
sf.sandKeys("rengo");
sf.submit();
```


### Getting Table Data
```
getText()
```

### Using the Explicit Wait
```
driver manage().timeouts().implicitlyWait(10, TimeUnit.SECONDS);
```
explicit
```
WebSriverWait wait = new WebDriverWait(driver,10);
wait.until(ExpectedConditions.presenceOfElementLocated(By.linkText("Info")));
```

## 6. Using Selenium Server
### Starting Selenium Server
```
java -jar selenium-server-standalone-3.4.0.jar
```

### Running a test
```
WebDriver driver = new RemoteWebDrivwe(new URL(""),DesiredCapabilities.chrome());
driver.get();
```
### Setting up Grid
```
java -jar selenium-server-standalone-3.4.0.jar -role node -hub http://1.2.3.4:4444/grid/register
```
### 2nd node Setop
```
java -jar selenium-server-standalone-3.4.0.jar -role node -hub http://1.2.3.4:4444/grid/register -port 5556
```

