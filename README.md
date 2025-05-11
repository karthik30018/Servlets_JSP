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

## ServletConfig and ServletContext
- Both are used to set the initial value.
- If we are using ServletContext.

![Screenshot 2025-05-10 230107](https://github.com/user-attachments/assets/44af315c-0c9d-4dc2-930b-bdbe60697084)


![sercxt1](https://github.com/user-attachments/assets/b37fe6d3-e23c-408d-9b4b-0918713a31ee)

![Screenshot 2025-05-10 230012](https://github.com/user-attachments/assets/8117a386-4b23-424b-a537-315cf87147d2)

- If we are using ServletConfig it belongs to a perticular servlet.

![ServConf1](https://github.com/user-attachments/assets/618ce830-1b0a-4820-a63e-f680cc0bc19d)

![servCon2](https://github.com/user-attachments/assets/48133199-e05e-4158-9b85-d8b258285a12)

![svtconop](https://github.com/user-attachments/assets/16360a6b-2c01-433a-8224-80ff22963a3d)

## Servlet Annotation Configuration

- Used to config the URL path in which path the page should open
![Screenshot 2025-05-10 231144](https://github.com/user-attachments/assets/dfc9e2be-4720-4e5a-ade2-0d8ea160bcb6)

instead of using xml code we can use annotation and specify the path.

![annot](https://github.com/user-attachments/assets/76e45060-8263-4f94-ac33-38247dda0600)

## JSP

Scriptlet
Declaration
Directive
Expression

![JSPtag](https://github.com/user-attachments/assets/563f2721-ac1a-4d71-8343-f3eeb56d8d8b)

### JSP Directive
![jspdir](https://github.com/user-attachments/assets/8dd2d2a6-60ed-47be-b038-fc5ee5690eb6)
![Screenshot 2025-05-11 140111](https://github.com/user-attachments/assets/2b3f36c7-ade6-4c6a-95ef-a9ea1a57ebeb)
![Screenshot 2025-05-11 140135](https://github.com/user-attachments/assets/9409c396-fad2-414c-af71-4eb11efe19b8)
![Screenshot 2025-05-11 140611](https://github.com/user-attachments/assets/12bb253e-66a1-417e-8483-80ea033b0533)

- To include other jsp page in the current page.
![Screenshot 2025-05-11 140757](https://github.com/user-attachments/assets/38480862-3eed-48de-a039-8f52346e6ca1)
![Screenshot 2025-05-11 140919](https://github.com/user-attachments/assets/296d1266-d69c-41de-ac74-ed74fa709bf5)


![Screenshot 2025-05-11 141032](https://github.com/user-attachments/assets/3cda8aa7-e5d3-4f16-b51f-52453c52e9f9)
- we can directly use the above objects in JSP.`<% request.getParameter(); %>`

![Screenshot 2025-05-11 141346](https://github.com/user-attachments/assets/51dc6b28-d225-49e1-a026-3f37a7e3ef75)
- The scope of the pageContext is the page where it is written.

![Screenshot 2025-05-11 141553](https://github.com/user-attachments/assets/27afc845-1ac2-4214-947f-f033c56625e6)
- It makes it available for every pages and will be stored in session.

## Exception handling in JSP

Create an error page and specify that it is an error page by including `isErrorPage="true"` in the first `<%@ %>` of JSP page
![Screenshot 2025-05-11 144258](https://github.com/user-attachments/assets/464995f9-1cdf-42a5-acdb-c3a49bc903cd)
Include the error page in other page
![Screenshot 2025-05-11 144336](https://github.com/user-attachments/assets/ccaf80ec-cdb6-46a1-a261-223dd167dc9d)




