package TestNG;


import org.openqa.selenium.WebDriver;
import org.openqa.selenium.firefox.FirefoxDriver;
import org.testng.annotations.AfterClass;
import org.testng.annotations.BeforeClass;
import org.testng.annotations.Parameters;
import org.testng.annotations.Test;


public class test {
	private WebDriver driver;
	@BeforeClass(alwaysRun = true)
	public void setUp() throws Exception {
		System.setProperty("webdriver.firefox.bin", "C:/Firefox/firefox.exe"); 
		driver = new FirefoxDriver();
		
	}
	@Test
	public void testNg() throws Exception{
		
		  driver.get("http://www.baidu.com");
		//driver.get("http://localhost:8018/jenkins/");  
		
		

	}
	@AfterClass(alwaysRun = true)
	public void tearDown() throws Exception {
		/* driver.quit();*/
	}
}
