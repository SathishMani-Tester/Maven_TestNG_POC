# Maven_TestNG_POC
1.	File-> Project -> Maven -> Maven Project
2.	Right click proj -> buildpath -> configure build path -> sources -> add resource folder
3.	Maven -> Update Project
4.	Added the below lines in POM.xml
<build>
    <pluginManagement>
      <plugins>
        <plugin>
          <groupId>org.apache.maven.plugins</groupId>
          <artifactId>maven-surefire-plugin</artifactId>
          <version>2.19.1</version>
        </plugin>
        
        <plugin>
        <groupId>org.apache.maven.plugins</groupId>
        <artifactId>maven-compiler-plugin</artifactId>
        <version>3.6.0</version>
        <configuration>
          <source>1.8</source>
          <target>1.8</target>
        </configuration>
      </plugin>
      
      </plugins>
    </pluginManagement>
</build>
5.	Added dependencies in POM.xml
                               <dependency>
                                                 <groupId>org.seleniumhq.selenium</groupId>
                                                <artifactId>selenium-server</artifactId>
                                                 <version>3.0.1</version>
                                </dependency>  
                                <dependency>
        <groupId>org.seleniumhq.selenium</groupId>
        <artifactId>selenium-java</artifactId>
        <version>3.0.1</version>
    </dependency>    
    
    		<dependency>
	    		<groupId>org.seleniumhq.selenium</groupId>
	    		<artifactId>selenium-support</artifactId>
	    		<version>3.0.1</version>
</dependency>
6.	Install TestNG by Help -> Install New Software -> Add-> Name: TestNG and Location: http://beust.com/eclipse -> OK

7.	Check “TestNG” -> Next -> choose both TestNG and click “finish”.

8.	It will download and ask confirm popup and click OK.

9.	It will ask for restart and click OK.

10.	To verify the TestNG installation: Windows -> Preferences -> TestNG

11.	Add TestNG to Libraries by Right Click the Proj -> BuildPath-> Add Libraries

12.	Add TestNG class ::: Right Click the package -> New -> Other -> TestNG -> TestNG Class

13.	Then Download the “apache-maven-3.3.9-bin.zip” file from http://maven.apache.org/download.cgi and extract the zip file to the path “C:\Program Files\Apache\Maven”.

14.	Add the User variables as below:
a.	JAVA_HOME -  C:\Program Files\Java\jdk1.8.0_111
b.	M2_HOME - C:\Program Files\Apache\Maven
15.	Add the System Variables of “Path” with “C:\Program Files\Java\jdk1.8.0_111\bin;C:\Program Files\Apache\Maven\bin”.

16.	Add GeckoDriver to open firefox  WebDriver driver;  System.setProperty("webdriver.gecko.driver", "C:\\Users\\sathishkumarm\\Downloads\\geckodriver-v0.11.1-win64\\geckodriver.exe");
