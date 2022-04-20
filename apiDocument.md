# Page 1

# List of city
>> https://localhost:9700/location

# List of restaurants
>? http://localhost:9700/restaurants

# List of restaurants wrt to city
>> // http://localhost:9700/restaurants/?state_id=1

# List of MealType
>> http://localhost:9700/mealType

# Page 2

# List of restaurant on basis of meal
>> http://localhost:9700/restaurants/?meal_id=1

# Filter on basis of cuisine
>> http://localhost:9700/restaurants/?cuisine_id=1

# Filter on basis of cost
>> https://localhost:9700/restaurants/?cost_id=

# page 3
# Details of restaurants
>> // http://localhost:9700/details/25cb97d5a04689830994708

# Menu on basis of restaurants
>> http://localhost:9700/menu/?rest_id=1

# page 4
# menu detail of item selected
(post) > http://localhost:9700/menuItem
(body)> [1,2] 

# place Order
    (post)> http://localhost:9700/placeOrder
    <body)> 
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
    },
    
# page 5

# see all place order
    >> http://localhost:9700/viewOrder

# get order on basis of emailId
    >> http://localhost:9700/viewOrder?eman@gmail.com

# update order
    (put) localhost:9700/updateOrder/625d255e5b5070060e2250db
    (body)  
        {
        "status":"Delivered",
        "cost":"1200"
        }






