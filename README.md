package seleniumproject;
import java.util.Set;
import java.util.concurrent.TimeUnit;
import org.openqa.selenium.By;
import org.openqa.selenium.Keys;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.WebElement;
import org.openqa.selenium.chrome.ChromeDriver;
import org.openqa.selenium.interactions.Action;
import org.openqa.selenium.interactions.Actions;
public class Freshteam {
 public static void main(String[] args) {
	// TODO Auto-generated method stub
	System.setProperty("webdriver.chrome.driver","C:\\softwares\\chromedriver_win32\\chromedriver.exe");
	WebDriver driver = new ChromeDriver();
	String url = "https://www.freshworks.com/";
	driver.get(url);
	// implicit wait
	driver.manage().timeouts().implicitlyWait(10, TimeUnit.SECONDS);
	
	// find products using xpath and store in txt variable
	WebElement txt = driver.findElement(By.xpath("/html/body/header/nav/div/div/ul/li[1]"));
	
	Actions builder = new Actions(driver);
	// move to element txt
	Action seriesOfActions = builder.moveToElement(txt).build();
	// perform action
	seriesOfActions.perform();
	
	// finding freshmarketer and navigating to it
	driver.findElement(By.xpath("//h6[text()=\"Freshmarketer\"]")).click();
	
	// clicking on sign up
	driver.findElement(By.xpath("/html/body/header/nav/div[2]/div/ul[1]/li[5]/a")).click();
	driver.manage().timeouts().implicitlyWait(10, TimeUnit.SECONDS);
	// clicking on sign up by email
	driver.findElement(By.xpath("/html/body/section/div/div/form/fieldset[2]/div[3]/div[1]")).click();
	// Entering inputs
	driver.findElement(By.xpath("/html/body/section/div/div/form/fieldset[1]/div[1]/div[1]/div[1]/div/input")).sendKeys("Likhitha");
	driver.findElement(By.xpath("/html/body/section/div/div/form/fieldset[1]/div[1]/div[1]/div[2]/div/input")).sendKeys("patel");
	driver.findElement(By.xpath("/html/body/section/div/div/form/fieldset[1]/div[1]/div[2]/input")).sendKeys("likhipatel48@gmail.com");
	driver.findElement(By.xpath("/html/body/section/div/div/form/fieldset[1]/div[2]/div[1]/input")).sendKeys("Aris");
	driver.findElement(By.xpath("/html/body/section/div/div/form/fieldset[1]/div[2]/div[2]/input")).sendKeys("9876543210");
	// clicking on sign up button
	driver.findElement(By.xpath("/html/body/section/div/div/form/fieldset[2]/div[1]/input")).click();
  
  
  // clicking on login
		driver.findElement(By.xpath("/html/body/header/nav/div[2]/div/ul[1]/li[4]/a")).click();
		driver.manage().timeouts().implicitlyWait(10, TimeUnit.SECONDS);
		
		// Entering inputs
		driver.findElement(By.xpath("//*[@id=\"fmarketer_login_form\"]/fieldset[1]/div/div[1]/input")).sendKeys("aris-388548836815786242");
		driver.findElement(By.xpath("//*[@id=\"fmarketer_login_form\"]/fieldset[2]/input")).click();
		
		// clicking on resources
		driver.findElement(By.xpath("/html/body/header/nav/div[2]/div/ul[1]/li[3]/span")).click();
		
		// clicking on product updates
		//driver.findElement(By.xpath("/html/body/header/nav/div[2]/div/ul[1]/li[3]/span")).click();

		// clicking on product tour
		driver.findElement(By.xpath("/html/body/header/nav/div[2]/div/ul[1]/li[3]/ul/li[2]/a/span")).click();
		//driver.findElement(By.xpath("//*[@id=\"video\"]/div/div/div[1]/div[1]/div[2]/p[1]")).click();
		//driver.findElement(By.xpath("//*[@id=\"video-popup-trigger-vvhwowq4hh\"]/span/img")).click();
		//driver.findElement(By.xpath("//*[@id=\"video-popup-trigger-vvhwowq4hh\"]/span")).click();
		//driver.findElement(By.xpath("//*[@id=\"video-popup-trigger-0taot33jpa\"]/span/img")).click();
		driver.findElement(By.xpath("//*[@id=\"video-popup-trigger-vy98nvlms2\"]/span/img")).click();
		
		// clicking on pricing
		driver.findElement(By.xpath("/html/body/header/nav/div[2]/div/ul[1]/li[2]/a")).click();
		// clicking on sign up
		driver.findElement(By.xpath("/html/body/section[1]/div/div/a")).click();
		// clicking on sign up by email 
		driver.findElement(By.xpath("/html/body/section/div/div/form/fieldset[2]/div[3]/div[1]")).click();
		// Entering inputs
		driver.findElement(By.xpath("/html/body/section/div/div/form/fieldset[1]/div[1]/div[1]/div[1]/div/input")).sendKeys("Likhitha");
		driver.findElement(By.xpath("/html/body/section/div/div/form/fieldset[1]/div[1]/div[1]/div[2]/div/input")).sendKeys("Patel");
		driver.findElement(By.xpath("/html/body/section/div/div/form/fieldset[1]/div[1]/div[2]/input")).sendKeys("likhithapatel@gmail.com");
		driver.findElement(By.xpath("/html/body/section/div/div/form/fieldset[1]/div[2]/div[1]/input")).sendKeys("Aris");
		driver.findElement(By.xpath("/html/body/section/div/div/form/fieldset[1]/div[2]/div[2]/input")).sendKeys("987654321");
		driver.findElement(By.xpath("/html/body/section/div/div/form/fieldset[2]/div[1]/input")).click();
		
		
		// clicking on features
		driver.findElement(By.xpath("/html/body/header/nav/div[2]/div/ul[1]/li[1]/span")).click();
		
		// clicking on CRM
		//driver.findElement(By.xpath("/html/body/header/nav/div[2]/div/ul[1]/li[1]/ul/li[1]/a/span")).click();
		
		// clicking on chat campaigns
		//driver.findElement(By.xpath("/html/body/header/nav/div[2]/div/ul[1]/li[1]/ul/li[2]/a/span")).click();
		
		// clicking on customer segmentation
		//driver.findElement(By.xpath("/html/body/header/nav/div[2]/div/ul[1]/li[1]/ul/li[3]/a/span")).click();
		
		// clicking on email campaigns
		//driver.findElement(By.xpath("/html/body/header/nav/div[2]/div/ul[1]/li[1]/ul/li[4]/a/span")).click();
		
        // clicking on event tracking
		//driver.findElement(By.xpath("/html/body/header/nav/div[2]/div/ul[1]/li[1]/ul/li[5]/a/span")).click();
		
		// clicking on journeys
		//driver.findElement(By.xpath("/html/body/header/nav/div[2]/div/ul[1]/li[1]/ul/li[6]/a/span")).click();
		
		// clicking on landing pages
		//driver.findElement(By.xpath("/html/body/header/nav/div[2]/div/ul[1]/li[1]/ul/li[7]/a/span")).click();
		
		// clicking onmarketing reports
		//driver.findElement(By.xpath("/html/body/header/nav/div[2]/div/ul[1]/li[1]/ul/li[8]/a/span")).click();
		
		// clicking on all features
		driver.findElement(By.xpath("/html/body/header/nav/div[2]/div/ul[1]/li[1]/ul/li[9]/a/span")).click();
		
		
		}
 
}
	
