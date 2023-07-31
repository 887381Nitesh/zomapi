* Zomato App

// page1
> List of city
* http://localhost:3022/location

>rest wrt to city
*http://localhost:3022/restaurants?stateId=2

> List of Quick Search
*http://localhost:3022/mealtype

//page2
> Rest wrt to mealtype
* http://localhost:3022/restaurants?mealId=4
* http://localhost:3022/restaurants?stateId=1&mealId=2

> Rest wrt to mealtype + cuisine
* http://localhost:3022/filter/1?cuisineId=2

> Rest wrt to mealtype + cost
* http://localhost:3022/filter/1?lcost=200&hcost=1000

//Page3
> Details of Restaurant
* http://localhost:3022/details/64bbeef9fc96de57e14c5bfe
> Menu of restaurant
* http://localhost:3022/menu/2


//Page4
> Details of Menu selected
* http://localhost:3022/menuDetails
 {"id":[4,8,21,9]}

> Place Order
*  https://localhost:3022/placeOrder
{
	"orderId" : 2,
	"name" : "Amit",
	"email" : "amit@gmail.com",
	"address" : "Hom 65",
	"phone" : 8934645457,
	"cost" : 612,
	"menuItem" : [
		45,
		34,
		41
	],
	"status" : "Delivered"
}


// Page5
> List of all the orders
* http://localhost:3022/orders

> Update orders details
* http://localhost:3022/updateOrder
{
    "_id":"647c9ef070ab7d9b545a4090",
    "status":"Out for delivery"
}

> Delete Orders
* http://localhost:3022/deleteOrder
{"_id":"647c9f2e36e6ecf8fde6722b"}