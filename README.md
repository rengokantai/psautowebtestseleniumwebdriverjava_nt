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
