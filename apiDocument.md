# Page 1

# List of city

  # https://localhost:9700/location
  # https://myrestproject.herokuapp.com/location

# List of restaurants
  # http://localhost:9700/restaurants
  # https://myrestproject.herokuapp.com/restaurants

# List of restaurants wrt to city

  # http://localhost:9700/restaurants/?state_id=1
  # https://myrestproject.herokuapp.com/restaurants/?state_id=1

# List of MealType

  # http://localhost:9700/mealType
  # https://myrestproject.herokuapp.com/mealType

# list of cost 

  # http://localhost:9700/cost

# Page 2

# List of restaurant on basis of meal

  # http://localhost:9700/restaurants/?meal_id=1
  # https://myrestproject.herokuapp.com/restaurants/?meal_id=1

# Filter on basis of cuisine

  # http://localhost:9700/restaurants/?cuisine_id=1
  # https://myrestproject.herokuapp.com/restaurants/?cuisine_id=1

# Filter on basis of cost

  # https://localhost:9700/restaurants/?cost_id=

# page 3

# Details of restaurants

  # http://localhost:9700/details/25cb97d5a04689830994708
  # https://myrestproject.herokuapp.com/details/62634dd07f2364ff459357fc

# Menu on basis of restaurants

  # http://localhost:9700/menu/?rest_id=1
  # https://myrestproject.herokuapp.com/menu/?restId=1

# page 4

# Menu detail of item selected

  # (POST)  http://localhost:9700/menuItem
    (body)> [1,2] 

  # (POST) https://myrestproject.herokuapp.com/menuItem
    (Body) [1,2,4]

# Place Order

   # (POST) http://localhost:9700/placeOrder
     (body) 
          {
            "name": "Eman",
            "email": "eman@gmail.com",
            "address": "Almuhandseen Block No.30",
            "phone": "0912133448",
            "cost": 4000,
            "menuItem": [
                1,
                5
            ],
            "status": "pending"
          }

  # (POST) https://myrestproject.herokuapp.com/placeOrder
    (Body) 
          {
            "name": "Emaa",
            "email": "emaa2022@gmail.com",
            "address": "Almuhandseen Block No.30",
            "phone": "0912133444",
            "cost": 3500,
            "menuItem": [
                2,
                6
            ],
            "status": "pending"
          }
    
# page 5

# See all place order

   # http://localhost:9700/viewOrder
   # https://myrestproject.herokuapp.com/viewOrder

# Get order on basis of emailId

   # http://localhost:9700/viewOrder?eman@gmail.com
   # https://myrestproject.herokuapp.com/viewOrder?emaa2022@gmail.com

# Update order

   # (PUT) localhost:9700/updateOrder/625d255e5b5070060e2250db
     (body)  
            {
                "status":"Delivered",
                "cost":"1200"
            }

   # (PUT) https://myrestproject.herokuapp.com/updateOrder/6264a0fd5e0281f186a4ac74
     (Body) 
          {
           "status":"Delivered",
            "cost":"3000"
          }


# Rest login Api 

# GetAllUser

# (GET)  http://localhost:5000/api/auth/users
# (GET)  https://rest-loginapp.herokuapp.com/api/auth/users

# Register

# (POST) http://localhost:5000/api/auth/register
   (body)   
        {
            "name":"Wagea",
            "email":"wagea@gmail.com",
            "password":"wagea@1997",
            "phone":"0123123124",
            "role":"user"
        }
# (POST) https://rest-loginapp.herokuapp.com/api/auth/register
   (Body) 
        {
            "name":"Hager",
            "email":"hager@hotmail.com",
            "password":"Hager8080",
            "phone":"0123123445",
            "role":"user"
        }  

# Login

# (POST)  http://localhost:5000/api/auth/login
    (body) 
        {
           "email":"wagea@gmail.com",
           "password":"wagea@1997"
        }
    (response) =>{"auth": true,token:'eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.'}

# (POST) https://rest-loginapp.herokuapp.com/api/auth/login
    (Body)
        {
            "email":"hager@hotmail.com",
            "password": "Hager8080"
        }
    
    (response) => {"auth": true,token:'eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.'}

# UserInfo

# (GET) => http://localhost:5000/api/auth/userinfo
  (Header) => {'x-access-token':'token value from login'}

# (GET)  https://rest-loginapp.herokuapp.com/api/auth/userinfo
  (Header) => {'x-access-token':'token value from login'}







