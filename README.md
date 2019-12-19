# An E-commerce Kata
Note: This is a Kata I'm currently designing in my free time, in an attempt to create the ultimate Kata that covers plenty of important development principles, .NET Core and building with a Clean Architecture approach!

You are a back-end developer and you've been on a one month holiday in sunny Hawaii. You have returned to work to find that in your absence, a new deal has been struck and your colleague who has left on their Christmas holidays began implementing... something.

## Part 1 - A deal has been struck.
Start by refactoring the pre-existing code and tests, left to you by your colleague. Take note of any code smells you have found along the way. Can you make any sense of some of the features they were trying to develop?

## Part 2 - A phone call was made.
Out of frustration, you have decided to phone your friendly neighbourhood team Business Analyst. He has provided you with an e-mail that summarises what your colleague was trying to implement:

The date is December 20th 2029 and the e-commerce company (LappyTops Ltd.) that you work for have struck a deal with a third-party supplier. The new business deal with the supplier means your company can now start to sell state of the art latest model Cranberry Laptops.

The release date of the latest model is on January 1st 2030, however you wish to start accepting pre-orders starting from December 26th 2029 as part of a Boxing Day offer on your website. As part of the pre-order deal, customers will have the choice to opt between two perks. The first perk is free delivery. The second perk involves a delivery charge but comes with a free set of wireless headphones worth £39.99. It is worth noting that customers who opt for the latter offer, pay £39.99 for the headphones however get them for free by claiming cashback within 30 days of receiving their order.

If an order is made on or after the Cranberry Laptop release date, neither of the two perks are eligible at checkout. If an order is made from the United Kingdom, the default delivery charge is £5.99. If the order is an international order, the default delivery charge is £9.99.

Create a new project titled "LappyTops.Domain" and test-drive this logic again from scratch. Does your code look any different to your refactored code? If so, why do you think so?

Continue developing your new project. You may now delete the old project if you wish.

## Part 3 - Your first customer.
Your front-end development team have created a SPA front-end to facilitate displaying the new Cranberry Laptops on the e-commerce company website. The front-end allows customers to choose between the two perks. They now need you to provide them with the following API endpoints:

    GET /api/items/laptops?sku={CRANB_001}
    Response:
    {
	    "sku": "CRANB_001",
	    "name": "Cranberry Laptop 2030",
	    "price": 999.99,
	    "perks": [...]
    }
    
    POST /api/addtobasket
    Request Body:
    {
	    "sku": "CRANB_001",
	    "price": 999.99,
	    "perkId": 1
	}

## Part 4 - Homer has made a mistake!
Homer is one of the Test Engineers involved in your development team. He has realised that whilst he can add products to his basket, he cannot remove them. Solve this problem.

## Part 5 - 
