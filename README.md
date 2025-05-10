# Servlets_JSP

## Servlet lifecycle methods

- init()
- service()
- Destroy()

## HTTP protocal

![Screenshot 2025-05-08 203708](https://github.com/user-attachments/assets/17dcc050-54c6-4467-a2d9-038eb2c9750a)
![DemoServlet](https://github.com/user-attachments/assets/d7ca50ac-51f1-4ee8-b22f-4706c602f53a)
![indexHtml](https://github.com/user-attachments/assets/d4ae0076-8078-4402-931e-d5266ce5ef85)
![webXml](https://github.com/user-attachments/assets/39e2a967-bc97-4a46-a0af-f4c5c9af707f)
- Here in web.xml we have to specify the Servelet name in both `<servlet>` and `<servlet-mapping>`
- The `<servlet-class>` name should include package_name.ServletPage_name.
- Specify the end point for the browser `<url-pattern>`.

  ### It has two methods GET and POST

- **Get** request is used to fetch data. 
- **Post88 request is used to send data.

  ### Note: In form tag if we did'nt specify any method by default it is considered as *GET* method

- When ever we are sending data using GET request the data goes into address bar(URL query).
- But if we are using POST request to send data it won't be using address URL to send the data.

### When ever we have to validate user credentials always use POST request

- **doPost()** it is only used to work with post method which is used in place of **service()** method in servlet pages

  ![doPost](https://github.com/user-attachments/assets/c4d649ef-15c7-45d6-8fb9-7cc5a5907a28)

  ## HttpServletRequest and HttpServletResponse

  - Request object will have all the data the servlet needs.
  - Response object will have all the data the client needs.



  ## RequestDispatcher and Redirect (Used to call one servlet in other servlet)

  ![reqDiseg](https://github.com/user-attachments/assets/367ed8b0-da36-4748-b89c-15146106215c)

  ![ReqDis1](https://github.com/user-attachments/assets/b1caac7f-35de-4281-a172-e20284d8bf93)

  ![ReqDis2](https://github.com/user-attachments/assets/b4a09836-4f13-41e3-baad-3ce627723640)

  ![ReqDis3](https://github.com/user-attachments/assets/b01be63d-16d1-4aec-aaaa-ca0b53a57651)

  - In RequestDispatcher the client won't be knowing that they are redirecting to other servlet or page.
 
  **Note: If the client also should know that the redirecting of servlet or pages occuring then use `sendRedirect()` method.**
  - eg. onlineshoping payment which rediects to other pages.
 
  **Note:  SessionManagement or URL Rewriting or Cookies is used pass data from one servlet to another.**
 
  ## sendRedirect() with URL Rewriting
 
  ![sendRed](https://github.com/user-attachments/assets/718f62b4-f9c3-48c9-b74b-0c4146c1f6c6)

  ![sendred1](https://github.com/user-attachments/assets/0376d39f-31df-41a7-bc1a-2a2d3bab4e46)

  ![sendRed2](https://github.com/user-attachments/assets/ca37b939-f5a2-4d99-84e3-cac6f10ce11c)

  ![SendRedOt](https://github.com/user-attachments/assets/7de65ac7-3fe5-4754-89ba-13b9300fab66)


 ## HttpSession 

 - By using this method we can use same data in multiple servlets.(Maintein data throughout the session)

 ![session1](https://github.com/user-attachments/assets/60f4a72c-1eec-4146-9f08-2d661d068b63)

 ![session2](https://github.com/user-attachments/assets/8370c16e-8e4a-48ee-b28b-54b3eff6f850)

 ![sessionOp](https://github.com/user-attachments/assets/efdeeb98-450b-4f41-8e4b-ad3b98bf25ad)

 - To remove the data from the session we can use `session.removeAttribute("str");`

## Cookies

![cookie1](https://github.com/user-attachments/assets/62288624-9847-484b-aef6-9c86df59817c)

![cookie2](https://github.com/user-attachments/assets/d135fd35-f9a2-4d1a-a5ed-f9734ac1dcf4)

![CookieOp](https://github.com/user-attachments/assets/d9d9bdd8-b0f7-4119-9075-feffbd9f520e)





