# Ex.07 Restuarant Website
## Date:

## AIM:
To develop a static Resturant website to display the menu and services provided by the resturant.

## DESIGN STEPS:

### Step 1:
Requirement collection.

### Step 2:
Creating the layout using HTML and CSS.

### Step 3:
Updating the sample content.

### Step 4:
Choose the appropriate style and color scheme.

### Step 5:
Validate the layout in various browsers.

### Step 6:
Validate the HTML code.

### Step 7:
Publish the website in the given URL.

## PROGRAM:
home.html
```
<html>
  <head>
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>ABC SOLUTIONS</title>
    <style type="text/css">
      * {
        margin: 0;
        padding: 0;
        font-family:system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
      }
      .banner {
        width: 100%;
        height: 95vh;
        background-image: linear-gradient(
            rgb(52, 2, 90),
            rgba(12, 1, 39, 0.892)
          ),
          url('/static/SUNDAR.png');
        background-size: cover;
        background-position: center;
      }
      .navbar {
        width: 90%;
        margin: auto;
        padding: 35px 0;
        display: flex;
        align-items: center;
        justify-content: space-between;
      }
      .logo {
        color: rgb(230, 6, 77);
        font-size: 40px;
        font-weight: 700;
        letter-spacing: 3px;
      }
      span {
        color: palevioletred;
      }
      form {
        width: 300px;
        height: 40px;
        display: flex;
        background:rgb(235, 152, 178) ;
        padding: 1px 1px;
        font-size: 15px;
        border-radius: 10px;
        backdrop-filter: blur(4px) saturate(180%);
      }
      form input {
        background: transparent;
        flex: 1;
        border: 0;
        outline: none;
        padding: 12px 20px;
        font-size: 15px;
        color: rgb(11, 109, 154);
      }
      ::placeholder {
        color: black;
      }
      form button {
        border: 100px;
        outline: none;
        padding: 5px 20px;
        color: rgb(255, 255, 255);
        border-radius: 10px;
        background: rgb(52, 2, 90);
        cursor: pointer;
      }
      #search.hover {
        border: 1px;
        padding: 10px;

        transition: 0.5s;
        cursor: pointer;
        border-radius: 30px;
        background: #0ef;
        color: #081b29;
        box-shadow: 0 0 20px #0ef;
      }
      .navbar li {
        list-style: none;
        display: inline-block;
        margin: 0 20px;
        position: relative;
      }
      .navbar li a {
        text-decoration:wavy;
        color: rgb(230, 6, 77);
        text-transform: uppercase;
        font-weight: 700;
        font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
      }
      .navbar li:hover {
        border: 1px;
        padding: 10px;

        transition: 0.5s;
        cursor: pointer;
        border-radius: 30px;
        background: rgba(12, 1, 39);
        color: #081b29;
        box-shadow: 0 0 20px rgb(230, 6, 77);
      }
      .content {
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        text-align: center;
      }
      .text h2 {
        color: rgb(235, 152, 178);
        font-weight: 800;
        font-size: 50px;
        letter-spacing: 3px;
      }
      .text p {
        color: rgb(235, 152, 178);
        text-transform: capitalize;
        font-size: 15px;
        margin-bottom: 30px;
        word-spacing: 2px;
        letter-spacing: 1px;
      }
      .login {
        margin: 0px 10px;
        border: 2px solid rgb(23, 1, 40);
        padding: 13px 35px;
        letter-spacing: 1px;
        color: rgb(230, 6, 77);
        border-radius: 30px;
        background-color: rgb(52, 2, 90);
        text-decoration: none;
      }
      .login:hover {
        border: 2px solid rgb(230, 6, 77);
        color: rgb(230, 6, 77);
        background-color: rgb(52, 2, 90);
        transition: 0.5s;
        cursor: pointer;
      }
      .signup {
        margin: 0px 10px;
        border: 2px solid rgb(23, 1, 40);
        padding: 13px 35px;
        letter-spacing: 1px;
        color: rgb(230, 6, 77);
        border-radius: 30px;
        background-color: rgb(52, 2, 90);
        text-decoration: none;
      }
      .signup:hover {
        border: 2px solid rgb(230, 6, 77);
        color: rgb(230, 6, 77);
        background-color: rgb(52, 2, 90);
        transition: 0.5s;
        cursor: pointer;
      }
      footer {
        border: 1px;
        padding: 10px;
        font-weight: 700;
        transition: 0.5s;
        cursor: pointer;
        border-radius: 30px;
        background: rgb(230, 6, 77);
        color: #4c035b;
        box-shadow: 0 0 20px rgb(230, 6, 77);
      }
    </style>
  </head>
  <body>
    <div class="banner">
      <br />
      <div class="navbar">
        <h1 class="logo">ABC SOLUTIONS</h1>
        <ul>
          <li><a href="/static/home.html"> Home </a></li>
          <li><a href="/static/service.html"> Services </a></li>
          <li><a href="/static/people.html"> People </a></li>
          <li><a href="/static/contact.html"> Contact Us </a></li>
        </ul>
        <form action="" method="get">
          <input type="text" placeholder="Enter to Search" />
          <button id="search" type="submit">Search</button>
        </form>
      </div>
      <div class="content">
        <div class="text">
          <h2>
            "Driving Growth Through Digital Innovation."
          </h2>
          <br />

          <br />
          <div>
            <a href="#" class="login"> Login </a>
            <a href="#" class="signup"> Sign Up </a>
          </div>
        </div>
      </div>
    </div>
    <footer>
      <center>Niranjan S (212224040221)</center>
    </footer>
  </body>
</html>

```
service.html
```
<html>
  <head>
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Product Page</title>
    <style type="text/css">
      * {
        margin: 0;
        padding: 0;
        font-family: Arial, Helvetica, sans-serif;
      }
      .banner {
        width: 100%;
        height: 95vh;
        background-image: linear-gradient(
            rgb(52, 2, 90),
            rgba(12, 1, 39, 0.892)
          ),
          url(niranjan\ softapp.webp);
        background-size: cover;
        background-position: center;
      }
      .navbar {
        width: 90%;
        margin: auto;
        padding: 35px 0;
        display: flex;
        align-items: center;
        justify-content: space-between;
      }
      .bg-product {
        border: 1px;
        padding: 10px;
        color: white;
        background-color: rgba(12, 1, 39, 0.892);
        border-radius: 30px;
      }
      .logo {
        color: rgb(230, 6, 77);
        font-size: 40px;
        font-weight: 700;
        letter-spacing: 3px;
      }
      span {
        color: palevioletred;
      }
      form {
        width: 300px;
        height: 40px;
        display: flex;
        background:rgb(235, 152, 178) ;
        padding: 1px 1px;
        font-size: 15px;
        border-radius: 10px;
        backdrop-filter: blur(4px) saturate(180%);
      }
      form input {
        background: transparent;
        flex: 1;
        border: 0;
        outline: none;
        padding: 12px 20px;
        font-size: 15px;
        color: black;
      }
      ::placeholder {
        color: black;
      }
      form button {
        border: 100px;
        outline: none;
        padding: 5px 20px;
        color: rgb(255, 255, 255);
        border-radius: 10px;
        background: rgb(52, 2, 90);
        cursor: pointer;
      }
      .navbar li {
        list-style: none;
        display: inline-block;
        margin: 0 20px;
        position: relative;
      }
      .navbar li a {
        text-decoration:wavy;
        color: rgb(230, 6, 77);
        text-transform: uppercase;
        font-weight: 700;
        font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
      }
      .navbar li:hover {
        border: 1px;
        padding: 10px;

        transition: 0.5s;
        cursor: pointer;
        border-radius: 30px;
        background: rgba(12, 1, 39);
        color: #081b29;
        box-shadow: 0 0 20px rgb(230, 6, 77);
      }
      .container {
        background: transparent;
        padding: 10px 5%;
        padding-bottom: 100px;
      }
      .container .box-container {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(170px, 1fr));
        gap: 100px;
      }
      .container .box-container .box {
        color: rgb(52, 2, 90);
        box-shadow: 0 5px 10px rgb(26, 1, 45);
        border-radius: 20px;
        background: transparent;
        border: 1px solid rgb(253, 0, 101) ;
        padding: 30px 20px;
      }
      .container .box-container .box img {
        height: 70px;
        border-radius: 20px;
      }
      .container .box-container .box h3 {
        color: rgb(255, 0, 93);
        font-size: large;
        padding: 20px 0;
      }
      .container .box-container .box p {
        color: plum;
        font-size: small;
        line-height: 1.5;
      }
      footer {
        border: 1px;
        padding: 10px;
        font-weight: 700;
        transition: 0.5s;
        cursor: pointer;
        border-radius: 30px;
        background: rgb(230, 6, 77);
        color: #4c035b;
        box-shadow: 0 0 20px rgb(230, 6, 77);
      }
    </style>
  </head>
  <body>
    <div class="banner">
      <br />
      <div class="navbar">
        <h1 class="logo">ABC SOLUTIONS</span></h1>
        <ul>
          <li><a href="home.html"> Home </a></li>
          <li><a href="product.html" class="bg-product"> Services </a></li>
          <li><a href="people.html"> People </a></li>
          <li><a href="contact.html"> Contact Us </a></li>
        </ul>
        <form action="" method="get">
          <input type="text" placeholder="Enter to Search" />
          <button type="submit">Search</button>
        </form>
      </div>
      <div class="container">
        <div class="box-container">
          <div class="box">
            <h3>Front End</h3>
            <p>
              We deliver responsive, user-focused front-end development using modern frameworks to create visually engaging, fast, and seamless web experiences.
            </p>
          </div>
          <div class="box">
            <h3>Back End</h3>
            <p>
              We provide robust back-end development services, building secure, scalable server architectures, APIs, and databases that power seamless, high-performing applications.
            </p>
          </div>
          <div class="box">
            <h3>Data Base Management</h3>
            <p>
                Delivering end-to-end database management services, including design, implementation, optimization, security, backup, and efficient data handling solutions.
            </p>
          </div>
          <div class="box">
            <h3>Cyber Security</h3>
            <p>
             We provide advanced cybersecurity solutions to protect businesses from threats, ensuring data integrity, secure networks, privacy compliance, and continuous monitoring.
            </p>
          </div>
        </div>
      </div>
    </div>
    <footer>
      <center>Niranjan S (212224040221)</center>
    </footer>
  </body>
</html>
```
people.html
```
<html>
  <head>
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>people page</title>
    <style type="text/css">
      * {
        margin: 0;
        padding: 0;
        font-family: Arial, Helvetica, sans-serif;
      }
      .banner {
        width: 100%;
        height: 95vh;
        background-image: linear-gradient(
            rgb(52, 2, 90),
            rgba(12, 1, 39, 0.892)
          ),
          url('/static/SUNDAR.png');
        background-size: cover;
        background-position: center;
      }
      .navbar {
        width: 85%;
        margin: auto;
        padding: 35px 0;
        display: flex;
        align-items: center;
        justify-content: space-between;
      }
      .bg-people {
        border: 1px;
        padding: 10px;
        color: white;
        background-color: rgba(12, 1, 39, 0.892);
        border-radius: 20px;
      }
      .logo {
        color: palevioletred;
        font-size: 40px;
        font-weight: 700;
        letter-spacing: 1px;
      }
      span {
        color: plum;
      }
      form {
        width: 300px;
        height: 40px;
        display: flex;
        background: rgb(39, 1, 60);
        padding: 1px 1px;
        font-size: 15px;
        border-radius: 10px;
        backdrop-filter: blur(4px) saturate(180%);
      }
      form input {
        background: transparent;
        flex: 1;
        border: 0;
        outline: none;
        padding: 12px 20px;
        font-size: 15px;
        color: white;
      }
      ::placeholder {
        color: white;
      }
      form button {
        border: 0;
        outline: none;
        padding: 5px 20px;
        color: white;
        border-radius: 10px;
        background:rgb(255, 0, 85);
        cursor: pointer;
      }
      .navbar li {
        list-style: none;
        display: inline-block;
        margin: 0 20px;
        position: relative;
      }
      .navbar li a {
        text-decoration:wavy;
        color: rgb(230, 6, 77);
        text-transform: uppercase;
        font-weight: 700;
        font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
      }
      .navbar li:hover {
        border: 1px;
        padding: 10px;

        transition: 0.5s;
        cursor: pointer;
        border-radius: 30px;
        background: rgba(12, 1, 39);
        color: #081b29;
        box-shadow: 0 0 20px rgb(230, 6, 77);
      }
      .image {
        position: relative;
        border: 0;
        top: 150px;

        background: transparent;
      }
      .image table {
        border: 0;
        color: white;
        position: relative;
        left: 200px;
        border: 10PX;
        padding-left: 10px;
      
      }
      .image table img {
        height: 140px;
        width: 140px;
        border: 2px solid white;
        padding: 5px;
        border-radius: 50%;
      }
      .image table td {
        color:rgb(255, 0, 106);
      }
      footer {
        border: 1px;
        padding: 10px;
        font-weight: 700;
        transition: 0.5s;
        cursor: pointer;
        border-radius: 30px;
        background: rgb(230, 6, 77);
        color: #4c035b;
        box-shadow: 0 0 20px rgb(230, 6, 77);
      }
      .space{
        color: #e5086b;
        padding-left: 30px;
        font-style: oblique;
        font-weight: 700;
      }
    </style>
  </head>
  <body>
    <div class="banner">
      <br />
      <div class="navbar">
        <h1 class="logo">ABC SOLUTIONS</h1>
          <li><a href="home.html"> home </a></li>
          <li><a href="product.html"> Services </a></li>
          <li><a href="people.html" class="bg-people"> People </a></li>
          <li><a href="contact.html"> Contact Us </a></li>
        </ul>
        <form action="" method="get">
          <input type="text" placeholder="Enter to Search" />
          <button type="submit">Search</button>
        </form>
      </div>
      <div class="image">
        <table cellspacing="80" >
          <tr align="center">
            <td><img src="/static/Screenshot 2025-10-31 082651.png" /></td>
            <td><img src="/static/SUNDAR.png" /></td>
            <td><img src="/static/SUNDAR JR.png" /></td>
            <td><img src="/static/MRS SUNDAR .png"/></td>
           
          </tr>
          <tr align="center" class="space">
            <th>NIRANJAN</th>
            <th>SUNDAR PICHAI</th>
            <th>SUNDAR PICHAI JR</th>
            <th>SUNDARI PICHAI</th>
            
            
          </tr>
          <tr align="center">
            <td>Founder</td>
            <td>Co-Founder</td>
            <td>CEO</td>
            <td>HR</td>
          
            
          </tr>
        </table>
      </div>
    </div>
    <footer>
      <center>Niranjan S(212224040221)</center>
    </footer>
  </body>
</html>
```
contact.html
```
<html>
  <head>
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Contact Page</title>
    <style type="text/css">
      * {
        margin: 0;
        padding: 0;
        font-family: Arial, Helvetica, sans-serif;
      }
      .banner {
        width: 100%;
        height: 95vh;
        background-image: linear-gradient(
            rgb(52, 2, 90),
            rgba(12, 1, 39, 0.892)
          ),
          url(niranjan\ softapp.webp);
        background-size: cover;
        background-position: center;
      }
      .navbar {
        width: 85%;
        margin: auto;
        padding: 35px 0;
        display: flex;
        align-items: center;
        justify-content: space-between;
      }
      .bg-contact {
        border: 1px;
        padding: 10px;
        color: white;
        background-color: rgba(12, 1, 39, 0.892);
        border-radius: 20px;
      }
      .logo {
        color: pink;
        font-size: 40px;
        font-weight: 700;
        letter-spacing: 3px;
      }
      span {
        color: palevioletred;
      }
      .navbar form {
        width: 300px;
        height: 40px;
        display: flex;
        background: rgb(39, 1, 60);
        padding: 1px 1px;
        font-size: 15px;
        border-radius: 10px;
        backdrop-filter: blur(4px) saturate(180%);
      }
      .navbar form input {
        background: transparent;
        flex: 1;
        border: 0;
        outline: none;
        padding: 12px 20px;
        font-size: 15px;
        color: white;
      }
      ::placeholder {
        color: white;
      }
      .navbar form button {
        border: 0;
        outline: none;
        padding: 5px 20px;
        color: bl;
        border-radius: 10px;
        background: rgb(248, 4, 118);
        cursor: pointer;
      }
      .navbar li {
        list-style: none;
        display: inline-block;
        margin: 0 20px;
        position: relative;
      }
      .navbar li a {
        text-decoration:wavy;
        color: rgb(230, 6, 77);
        text-transform: uppercase;
        font-weight: 700;
        font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
      }
      .navbar li:hover {
        border: 1px;
        padding: 10px;

        transition: 0.5s;
        cursor: pointer;
        border-radius: 30px;
        background: rgba(12, 1, 39);
        color: #081b29;
        box-shadow: 0 0 20px rgb(230, 6, 77);
      }
      .box {
        display: flex;
        column-gap: 150px;
        background: transparent;
        position: relative;
        top: 50px;
        width: 220px;
      }
      .box-1 {
        height: 500px;
        width: 500px;
        border: 3px solid rgb(250, 0, 117);
        border-radius: 20px;
        background: transparent;
        position: relative;
        left: 250px;
      }
      .box-2 {
        height: 500px;
        width: 800px;
        border: 3px solid rgb(250, 0, 117);
        border-radius: 20px;
        background: transparent;
        position: relative;
        left: 300px;
      }
      .box-1 form {
        display: flex;
        color: rgb(255, 0, 132);
        background: transparent;
        padding: 10px;
        font-size: 15px;
        position: relative;
        top: 15px;
      }
      .box-1 form input {
        background: transparent;
        display: flex;
        border: 1px solid rgb(250, 0, 117);
        border-radius: 10px;
        padding: 15px 30px;
        font-size: 15px;
        color: rgb(250, 0, 117);
        position: relative;
        top: 30px;
      }
      .box-1 form textarea {
        background: transparent;
        color: rgb(49, 2, 59);
        padding: 15px 10px;
        position: relative;
        top: 30px;
        left: 20px;
        border: 1px solid rgb(250, 0, 117);
        border-radius: 10px;
        width: 300px;
      }
      .box-1 form button {
        border: 0;
        outline: none;
        padding: 10px 20px;
        color: rgb(250, 0, 117);
        border-radius: 30px;
        background: rgb(41, 1, 51);
        cursor: pointer;
        position: relative;
        top: 50px;
      }
      .box-2 h2 {
        color: rgb(250, 0, 117);
        position: relative;
        top: 25px;
        left: 50px;
        font-size: 30px;
      }
      .box-2 p {
        color: rgb(250, 0, 117);
        position: relative;
        top: 50px;
        padding: 10px 80px;
      }
      .box-2 span {
        color: rgb(255, 255, 255);
        font-size: 20px;
      }
      footer {
        border: 1px;
        padding: 10px;
        font-weight: 700;
        transition: 0.5s;
        cursor: pointer;
        border-radius: 30px;
        background: rgb(230, 6, 77);
        color: #4c035b;
        box-shadow: 0 0 20px rgb(230, 6, 77);
      }
    </style>
  </head>
  <body>
    <div class="banner">
      <br />
      <div class="navbar">
        <h1 class="logo">ABC SOLUTIONS</span></h1>
        <ul>
          <li><a href="home.html"> Home </a></li>
          <li><a href="product.html"> Services </a></li>
          <li><a href="people.html"> People </a></li>
          <li><a href="contact.html" class="bg-contact"> Contact Us</a></li>
        </ul>
        <form action="" method="get">
          <input type="text" placeholder="Enter to Search" />
          <button type="submit">Search</button>
        </form>
      </div>
      <div class="box">
        <div class="box-1">
          <form>
            <center>
              <h1>Contact Us</h1>
              <input type="text" placeholder="Your Name" />
              <br />
              <input type="email" placeholder="Your Email" />
              <br />
              
              <br />
              <button type="submit">Submit</button>
            </center>
          </form>
        </div>
        <div class="box-2">
          <h2>Contact Information</h2>
          <p>
            <span>Address</span> :Saveetha Nagar, Kanchipuram - Chennai Rd, Sriperumbadur, Chennai, Tamil Nadu 602105
          </p>
          <p><span>Email</span> : niranjan251006@gmail.com</p>
          <p><span>Phone</span> : 9977664422</p>
        </div>
      </div>
    </div>
    <footer>
      <center>Nirnajan S (212224040221)</center>
    </footer>
  </body>
</html>
```


## OUTPUT:
![alt text](<fwad exp7 ss1.png>)
![alt text](<fwad exp7 ss2.png>)
![alt text](<fwad exp7 ss3.png>)
![alt text](<fwad exp7 ss4.png>)
## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
