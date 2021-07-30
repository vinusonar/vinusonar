package LinkedInHomePage;

import org.openqa.selenium.By;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.chrome.ChromeDriver;
import org.testng.annotations.Test;

public class JoinLinkedIn1 

{
  WebDriver driver;
  
  @Test
  
  public void setUp() 
  
  {
	  System.setProperty("webdriver.chrome.driver","G:/Selenium/Executable Jar/chromedriver_win32 (2)/chromedriver.exe/");
	  
	  driver= new ChromeDriver();
	  
	  driver.get("https://www.flipkart.com/");
	  
	  driver.findElement(By.xpath("(//input[@type='text'])[2]")).sendKeys("8275918137");
	  
	  driver.findElement(By.xpath("//input[@type='password']")).sendKeys("Vinu@1990");
	  
	  driver.findElement(By.xpath("(//button[@type='submit'])[2]")).click();
  }
  
  }
