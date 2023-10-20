# Ex-04_RESTful_Web_Services
## Aim:

To create, deploy and execute RESTful Web service programs using Server, Client and Client-Side remote invocation
## Procedure:

### Server side:
Step 1: Create a new Java Web Project. Follow Steps 1-5 as in SOAP Based Web Service.

Step 2: Right-click on the project name and select New->RESTful Web Services from Patterns.

![image](https://github.com/Krishnakumar05/Ex-04_RESTful_Web_Services/assets/119393130/4950dd33-71e5-4927-8e28-27bffb32c724)



Step 3: A new window will appear. Select “Simple Root Resource” and click Next.

 ![image](https://github.com/Krishnakumar05/Ex-04_RESTful_Web_Services/assets/119393130/0da31501-0016-4990-8cdb-a9d30974fa5c)

 


Step 4: In the next window, give a Resource Package name and choose MIME Type as “text/html”. Click Finish.

![image](https://github.com/Krishnakumar05/Ex-04_RESTful_Web_Services/assets/119393130/81979013-16de-4b39-8626-4317b48d08d1)


Step 5: Two editing tabs will appear. Close “ApplicationConfig.java”. You need to write all your required functionalities in GenericResource.java.
Step 6: Alter getHtml() method as shown below.
Step 7: Save your project, clean and build it. Deploy your project.

 ![image](https://github.com/Krishnakumar05/Ex-04_RESTful_Web_Services/assets/119393130/07459d8a-7f68-49c5-a086-4219f4d0be65)


 


Step 8: To test your web service, open a new browser window/tab and type the URL as http://localhost:8080/project_name/webresources/generic?params=45&params=35 and hit enter. (This is the easiest way of testing the web service when it makes use of List).



Client-Side:


Step 1: Create a new Java Web Project. Follow steps 1-5 as in section 1.1.
Step 2: Right-click on the project and select New->RESTful Java Client.

![image](https://github.com/Krishnakumar05/Ex-04_RESTful_Web_Services/assets/119393130/84f6199c-9d0a-48b1-bcd8-15f618e822eb)




Step 3: A new window will appear. In that, give a name to your client, a package name and select “From Project” under the “Select the REST resource:” tab and click Browse.

Step 4: Carefully select your RESTful resource (web service) and click OK.
 
![image](https://github.com/Krishnakumar05/Ex-04_RESTful_Web_Services/assets/119393130/a2d8400c-b92a-4036-82c2-fe94b2db0416)
 


Step 5: Once everything is filled, the New RESTful Java Client window should look like this. Click Finish.

![image](https://github.com/Krishnakumar05/Ex-04_RESTful_Web_Services/assets/119393130/b6882013-f0ae-4e23-9c4b-420bd4d63140)

Step 6: An editing tab will open. Alter getHtml() method with the following.

![image](https://github.com/Krishnakumar05/Ex-04_RESTful_Web_Services/assets/119393130/dad59d93-88c0-497f-a3b8-71f98afe0a8f)
 


Step 7: Right-click on the Libraries folder under your project and select “Add JAR/Folder”.

![image](https://github.com/Krishnakumar05/Ex-04_RESTful_Web_Services/assets/119393130/737bebd9-df84-4fe8-aed8-a3013d26ff07)

Step 8: A new window will appear. Navigate to the folder where you have placed the “javax.ws.rs-api2.0.1.jar” file and select Open.

![image](https://github.com/Krishnakumar05/Ex-04_RESTful_Web_Services/assets/119393130/a95d1fe4-41bd-41e8-8e0c-7b0b72383db5)

 


Step 9: Right-click on the Web Pages folder and select JSP. In the new window, give a name to the JSP page and click Finish.
Step 10: A new tab will appear with the default contents of the JSP page. In that, include at the top and type the following code to invoke the client java code.

![image](https://github.com/Krishnakumar05/Ex-04_RESTful_Web_Services/assets/119393130/996d5b6b-bcab-4085-8d86-dd7c2c72510c)


Step 11: Save the project and build it.
Step 12: Run the JSP file and you should see the output in a new browser window.

![image](https://github.com/Krishnakumar05/Ex-04_RESTful_Web_Services/assets/119393130/8094b62f-fea4-4d9b-a6de-aef9d64c6c46)

 
 


Client-Side Remote Invocation:


Step 1: Follow steps 1-5 as in Section 2.2
Step 2: In the generated NewJerseyClient.java file, Replace BASE_URI from private static final String BASE_URI = "http://localhost:8080/RESTful_Server/webresources"; TO private static final String BASE_URI = "http://192.168.116.62:8080/RESTful_Server/webresources";
Step 3: Follow steps 6-12 as in Section 2.2


## Result:
 Thus, the RESTful web service program has been successfully created and executed.
