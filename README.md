# Intern_Project

# Login with the Website

package automation;
import org.openqa.selenium.By;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.chrome.ChromeDriver;
public class Practise_Project {

public static void main(String[] args)throws InterruptedException  {
		// TODO Auto-generated method stub

   WebDriver driver = new ChromeDriver();

  driver.get("https://www.automationexercise.com/login");
        driver.manage().window().maximize();

   driver.findElement(By.name("email"))
              .sendKeys("zaman123@gmail.com");

  Thread.sleep(1000);

  driver.findElement(By.name("password"))
              .sendKeys("zaman456");

   Thread.sleep(1000);

  driver.findElement(By.cssSelector("[data-qa='login-button']"))
        .click();
        Thread.sleep(5000);

   driver.quit();
	}

}









  

   
