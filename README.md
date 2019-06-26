# FOODOODOO

## Project Introduction
Foodoodoo is a web application that allows registered users to order food online and pickup for a later time. This application is built by Saad Hafa, Barry Chen, and Karine Seguin.

## Final Product Screenshots
- Upon visiting `http://localhost:8080/`, the user will be directed to the `Login` page:
![](https://github.com/leboss125/-midterm_project/blob/master/screenshots/Screen%20Shot%202019-06-24%20at%208.38.35%20PM.png)
- The user should click `Create Account` to register for an account and enter the required fields:
![](https://github.com/leboss125/-midterm_project/blob/master/screenshots/Screen%20Shot%202019-06-24%20at%208.39.18%20PM.png)
- Once logged in, the user will be redirected to the restaurant main page and see the available restaurants they can order from
![](https://github.com/leboss125/-midterm_project/blob/master/screenshots/Screen%20Shot%202019-06-24%20at%208.39.51%20PM.png)
- The user may click on the restaurant link which will redirect them to the restaurant menu page
![](https://github.com/leboss125/-midterm_project/blob/master/screenshots/Screen%20Shot%202019-06-24%20at%208.41.05%20PM.png)
- The user may choose the item and quantity they wish to order by clicking the `+` and `-` button beneath the items. An order summary including the total price will appear next to the menu.
- The user can click `Order Now` to place an order, an order request will be sent to the restaurant. Meanwhile, the user will be redirected to the `Order Status` page and can view the current status of the order as 'Pending'.
![](https://github.com/leboss125/-midterm_project/blob/master/screenshots/Screen%20Shot%202019-06-24%20at%208.54.09%20PM.png)
- Once the restaurant accepts the order. The user will then receive a corresponding sms message on their phone and the status of the order will be changed to 'Accepted'
![](https://github.com/leboss125/-midterm_project/blob/master/screenshots/64887449_796466794083165_5136017966680244224_n.jpg)
![](https://github.com/leboss125/-midterm_project/blob/master/screenshots/Screen%20Shot%202019-06-24%20at%208.54.35%20PM.png)

- Once the order is ready for pickup, the user shall receive another sms message on their phone and the status of the order will be changed to 'Ready'
![](https://github.com/leboss125/-midterm_project/blob/master/screenshots/65736145_593740377781669_680116304773906432_n.jpg)
![](https://github.com/leboss125/-midterm_project/blob/master/screenshots/Screen%20Shot%202019-06-24%20at%208.54.55%20PM.png)
- Finally, once the user picks up the food. They should receive a final text message saying their order is completed. The order will then be stored into the `Order History` page and its status labeled as 'Completed'
![](https://github.com/leboss125/-midterm_project/blob/master/screenshots/65378892_1095170254009096_7623004262439583744_n.jpg)
![](https://github.com/leboss125/-midterm_project/blob/master/screenshots/Screen%20Shot%202019-06-24%20at%208.57.05%20PM.png)
## Dependencies

- Node.js
- EJS
- Bootstrap 3
- jQuery
- node-sass-middleware
- knex.js
- pg
- cookie-session
- bcrypt
- body-parser
- dotenv
- express
- morgan
- twillio 

## Getting Started
1. Clone the repository
2. Install all dependencies using `npm install`
3. Run data migrations: `npm run knex migrate:latest`
4. Run the seed: `npm run knex seed:run`
5. Create your own Twilio account (https://www.twilio.com/try-twilio) and add your credentials in the order_route.js located in the routes directory. You will also need two phone numbers, one to represent the client and one to represent the restaurant. Note that to use these phone numbers in the Twilio free trial version, you need to verify them first. 
6. Run the server: `node server.js`
7. Visit `http://localhost:8080/`
