### What is Selenium
- Web based automation tool which automates browser.
- Selenium automates browsers.
- https://www.selenium.dev/ is official website.
- Free and open source.

### How to Use Selenium In Intellij
- Go to downloads https://www.selenium.dev/downloads/
- Download Selenium Server (Grid) by clicking on Latest stable version
- Open Intellij and go to file and project structure
- Go to modules and dependencies
- Click on + icon
- Click on JAR or Directories
- Select the downloaded file
- Apply
- Okay

### How to Download Chrome Driver
- Go to https://chromedriver.chromium.org/downloads
- Don't forget to check the version of browser.
- Download Chrome Driver
- Copy chromedriver.exe to C drive.

### How Website is Made
- By HTML, CSS & Javascript [+ Others]
- HTML: Hyper Text Markup Language [Structure Define]
- CSS: Cascading Style Sheets [Design and Style]
- JS: Javascript [Functions]



### Simple But Important
driver.getTitle(); - To Get Website Title
driver.getCurrentUrl(); - To Get Current URL
driver.get("https://selenium.dev"); - To Go to Website
driver.navigate().back(); - To Go Back
driver.navigate().forward(); - To Go Forward
driver.navigate().refresh(); - To Refresh Current Tab
driver.quit(); - To quit browser

### Alert Box
driver.switchTo().alert().dismiss(); - Cancel Alert Box
driver.switchTo().alert().accept(); - Okay Alert Box
driver.switchTo().alert().getText(); - Get alert message

### Go to Google / Search For Dart Tutorial, Open dart-tutorial.com


### How to Add Cookie
driver.manage().addCookie(new Cookie("key", "value"));

### How to View Cookie By Its Name
Cookie cookie1 = driver.manage().getCookieNamed("name");
System.out.println(cookie1);

### How to Display All Cookie
Set<Cookie> cookies = driver.manage().getCookies();
System.out.println(cookies);

### How to Delete Cookie
driver.manage().deleteCookieNamed("name");


### Work
- Go to Website https://thulotechnology.github.io/SampleTestWebsite/
- Click Backend In Dart [Iframe]

### How to Work With Iframe
driver.switchTo().frame("buttonframe"); - Switch by iframe id or name
driver.findElement(By.tagName("button")).click(); - Click button of ifrme
driver.switchTo().defaultContent(); - Go out or return to top 
driver.switchTo().frame(1); - Switch to frame index 1


### Maximize, Minimize and Full Screen
- driver.manage().window().maximize();
- driver.manage().window().minimize();
- driver.manage().window().fullscreen();


### Quit Vs Close
-  driver.close(); -Close is used to close the current tab.
-  driver.quit(); Quit is used to quit whole browser.

### Working With Window
To show all the active tabs
```java
ArrayList<String> tabs = new ArrayList<String> (driver.getWindowHandles());
```
To Switch to different tab
```java
driver.switchTo().window(tabs.get(1)); // 0 for first 1 for second and so on...
```
To Close the current tab
```java
driver.close();
```



### Work
- Go to http://www.webdriveruniversity.com/
- Click on CONTACT US.
- Add Firstname, Lastname, Email, Comments
- Click Submit
- Close the current window [Thank You for your message]
- Switch to first windows
- Click login portal
- Enter username and password
- Click login
- close the current window [Login]




