# ETG_InventoryMangementSystem
I'm Aman Kumar. I am a 2nd year undergraduate of IIT Kharagpur and I have successfully completed my first mini project of Inventory Management System given by ETG in Skill India Python for ML/AI Internship.
Thanks for giving us such a great opportunity to enhance our skills.

#Overview:
          
          #     An inventory management system enables a company to maintain a centralized record of every asset and item in the control of the organization, providing a single  
                source of truth for the location of every item, vendor and supplier information, specifications, and the total number of a particular item currently in stock.

#Files :

          #    - IMS.ipynb : IMS python code
          #    - originalRecord.json : Original inventory dict
          #    - salesRecord.json : Updated inventory dict after exiting the inventory
          #    - purchaseRecord.json : Stores all the purchased detail in dict


#Demonstration Video :

          

#Code Features:

          #    - Can Buy multiple product
          #    - Can Update the item details of the items in the inventory
          #    - Can New Add the items in the inventory 
          #    - Can Generate well indented bills
          #    - Can Print the purchase detail with the customer id
          #    - Can print the inventory list


#Product Features:

     #    - Stored/updated in salesRecord.json 
     
          #    - Product ID
          #    - Product Name
          #    - Product Categoery
          #    - Product Quantity available in stock
          #    - Product Unit Price
          #    - Product Discount Available
          #    - Product Stock Price
          
         
 #Transaction Features: 

      #    - Stored in purchasedRecord.json
      
          #    - Customer ID
          #    - Product ID
          #    - Product Name
          #    - Purchased quantity
          #    - Total Price
 
 
 #Working of the code:

          #    - Press 'C' - To Print product list
          #    - Press 'B' - To Buy mutiple products at a time

                              - Ask you to enter the product id:
                                  - If the product id is not available, then it will ask you to enter a valid product id
                                  - If the product id will available:

                                      - Then ask you to enter the product quantity that you want to buy:
                                      - If required product quantity is available in stock:
                                          - It will update the product quantity and product stock price in products dict
                                          - Save the purchased date/time, product name, quantity and total price
                                          - Call salesRecord() funtion to store the details of sold product in json format
                                          - Save the purchased item and quantity in purchased list
                                          - And ask you "To press (y/n) for continuing buying"

                                      - If required product quantity is not available stock:
                                          - It will thorw a message "Sorry!" with the qantity available in the stock
                                          - And ask you "To press (y/n) for continuing buying"

                              - Generate a well indented bill with all required things using the purchased list
                                  - Print store name, email address of the owner
                                  - Print the date and time of purchase
                                  - Print the list of item purchased:
                                      - Product ID, Product Name, Unit price, Discount, Total price after discount
                                      - Grand Total
                                  - Message "Thank You, Please do come again"

          #    - Press 'A' - To Add new product in the inventory

                            - Call checkItem() funtion, to check wether it is already present in the inventory or not

                                - If present, throw a message that it is already available in the inventory, you need to update it and call updateItem() function
                                - If it is not there then it will call addItem() funtion

          #    - Press 'D' - To Update product details in the inventory

                           - Call checkItem() funtion, to check wether it is already present in the inventory or not

                                - If present, then it will call updateItem() funtion 
                                - If it is not there then throw a message that it is not available in the inventory, you need to add it and call addItem() function


          #    - Press 'P' - To print the purchase detail of Customer with their customer id.

          #    - Press 'E' - To Exit


