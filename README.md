# Redbus

We have Cloned a bus ticketing and hiring platform called redbus.
redBus is an Indian online bus ticketing platform providing ticket booking facility through its website, iOS and Android mobile apps. It connects bus travellers with a network of over 2500 bus operators, across India, countries in South East Asia and Latin America.
It connects bus travellers with a network of over 2500 bus operators, across India, countries in South East Asia and Latin America.

In this project , we have tried to make a perfect clone of redbus.in.

### Live Link :  https://redbus.netlify.app/

# Steps to install the project:

## Update system
```bash
sudo apt update && sudo apt upgrade -y
```

## install git
```bash
sudo apt install git -y
```

##  install Node.js + npm
This project works best on Node 16 or 18.
```bash
curl -fsSL https://deb.nodesource.com/setup_18.x | sudo -E bash -
sudo apt install -y nodejs
```

## Install MongoDB
```bash
sudo apt install -y mongodb
sudo systemctl enable mongodb
sudo systemctl start mongodb
```
Check if its running. 
```bash
systemctl status mongodb
```

## Backend setup
```bash
cd back-end-redbus
npm install
```
Create .env file in back-end-redbus/.env
```bash
PORT=5000
NODE_ENV=development
MONGO_URI=mongodb://localhost:27017/redbus
JWT_SECRET=supersecretkey123
STRIPE_SECRET_KEY=sk_test_yourStripeSecretKey
STRIPE_PUBLIC_KEY=pk_test_yourStripePublicKey
CLIENT_URL=http://localhost:3000
```
Run backend:
```bash
npm start
```

## Frontend setup
Open a new terminal:
```bash
cd ~/redbus/front-end-redbus
npm install
```
Fix for Node17+
add this before running:
```bash
export NODE_OPTIONS=--openssl-legacy-provider
```
Then start:
```bash
npm start
```
Frontend will run at : http://localhost:3000
Backend will run at : http://localhost:5000


## Technologies used
  
  * React
  * CSS
  * Express
  * MongoDB
  * Mongoose
  * Libraries used
      
      * Redux
      * React-redux
      * Redux-thunk
      * material-ui/core
      * material-ui/icons
      * material-ui/lab
      * uuid
      * React-dom
      * React-icons
      * react-google-login
      * react-icons
      * react-modal
      * react-scripts
      * react-stripe-checkout
      
      
## How to use the product


 1. In order to use the product , you need to do npm start in your console.

  ![Landing Page](https://github.com/nitansh11/redbus/blob/master/Samples/HomePage1.PNG)

 2. Here you can see our landing page , If you are using this product for the first time , you are a new user and you can login by clicking on dropdown on the right side of navbar and currently we are serving buses between Lucknow and Faizabad, so enter Lucknow in source and Faizabad in destination and select any date as per your choice.

  ![Sign up](https://github.com/nitansh11/redbus/blob/master/Samples/GoogleSignIn.PNG)

 3. This page contains the list of all the buses between source and destination.On this page, user can use filtering and sorting as per his requirement.

  ![list_of_buses](https://github.com/nitansh11/redbus/blob/master/Samples/listOfbuseswithfilters.PNG)
 
 4. Here, you will get all the list of buses acoording to your location and you can also filter them as per your requirement.

 5. After this , you can click on the View Seat button to book the seats, and select the seats as per your requirement.
   Note : You cant select the red seats , since they are already booked.
  
   ![seet_booking](https://github.com/nitansh11/redbus/blob/master/Samples/seatBookUi.PNG)
 
 6.Now, select the boarding and dropping point and click on the continue button, now a form will open , here you need to enter the passenger details, and click on the Procced To Pay button.
  
   ![stripe payment](https://github.com/nitansh11/redbus/blob/master/Samples/StripePayment.PNG)

 7. On this page click on the button Pay with Stripe , here enter your email , card number as 4242 4242 4242 4242 , expiary date as 12/21 and cvv as 1234 and click on the pay button , your seat has been booked :relaxed:

  8. Now on this page you can see all your bookings.
  
  ![list_of_bookings](https://github.com/nitansh11/redbus/blob/master/Samples/ListOfBookings.PNG)
  
  9. Next feature that we have implemented is Bus Hire. Click on Bus Hire from the top bar. From this page, user can hire a bus for a round trip.
  
  ![bus hire landing page](https://github.com/nitansh11/redbus/blob/master/Samples/bushire1.png)
  
  10. On the Bus Hire landing page, click on Outstation, after that user will be asked to enter the few details.After entering those, click on proceed.

  ![bus hire form page](https://github.com/nitansh11/redbus/blob/master/Samples/bushire2.png)
  
  11. Select a bus as per your choice and click on View Details to proceed.

  ![bus select page](https://github.com/nitansh11/redbus/blob/master/Samples/bishire3.png)
  
  12.Click on Book, to book that particular vehicle and proceed for the payment.
  
  ![bus book page](https://github.com/nitansh11/redbus/blob/master/Samples/bushire4.png)
  
  13. On this page click on the button Pay with Stripe , here enter your email , card number as 4242 4242 4242 4242 , expiary date as 12/21 and CVV as 123 and click on the pay button , your bus has been booked :relaxed:
  
  ![payment page](https://github.com/nitansh11/redbus/blob/master/Samples/bushire5.png)

 
### End-notes
 
  We have tried our best to give mostly all the functionality available on the actual website.

  
  ### Contributors:

  * Nitansh Rastogi

    * Github : [nitansh11](https://github.com/nitansh11)

  * Uditanshu Kumar

    * Github : [udit22022000](https://github.com/udit22022000)

  * Rohan Kumar Banarwal

    * Github : [kumarrohan2804](https://github.com/kumarrohan2804)

 * Archana Singh

    * Github : [archana-sing](https://github.com/archana-sing)
