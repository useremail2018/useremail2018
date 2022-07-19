- 👋 Hi, I’m Ashish Kumar Bharti


Project
Coupon code creation in database and fetch through location coordinates

Working:
1. consists of Routes for creating GET and POST route
2. controller for writing logic of get and post request
3. Model for defining schemas
4. config.js for connection to MongoDB
5. app.js for running the project

The app demonstrates how we can create a coupon with Name, Description, Expiry Date and location coordinates details. 
Once database is created with different coupons we can fetch the coupon with the help of location(latitude &longitude) 

##To run the application 
npm install
npm start

## Api can be verified through postman 

## To insert coupon into database
Use Postman->Post-> http://localhost:3000/add-coupon

Insert in Body: {
    "name": "string",
    "description": "string",
    "location" : {
        "type": "Point",
        "coordinates": [latitude, longitude]
    }
    
}

##To search coupon from database 
Use Postman-> Get -> http://localhost:3000/search-coupon?cords=latitude, longitude






