
# Inventory Management System

An Inventory management system enables a company to maintain a centralized record of every asset and item in the control of the organization, providing a single source of truth for the location of every item, vendor and supplier information, specifications, and the total number of a particular item currently in stock.
## Demo

link to demo video ( will uploaded soon )

## Repository Files

  | Files             | What they Contains ?                                                               |
| ----------------- | ------------------------------------------------------------------ |
| IMS.ipynb |Inventory Management System Jupyter Notebook Code |
| originalRecord.json |Original record file contained all the initial item details in .json format |
| salesRecord.json |  Updated record file after Buy/Add/Update operation|
| purchaseRecord.json | Purchased history of customer, it can be access by their unique customer id |

## Features

- Buy multiple product
    - Can Inform when the product is not available in the stock.
    - Can Inform when the product quatity in stock is less than customer demand.

- Update the item details
    - Product Name, Category, Unit Price, Qyantity, Discount Available

- Add the new items in the stock.
- Print the purchase detail using the unique customer id.
- Generate well indented bills.
- Print the inventory list.## Repository Files Overview



## Product Feature


    - Stored/updated in salesRecord.json 
     
        - Product ID
        - Product Name
        - Product Categoery
        - Product Quantity available in stock
        - Product Unit Price
        - Product Discount Available
        - Product Stock Price
  
## Bill Feature

    - Date/Time of Purchase
    - Product ID
    - Product Name
    - Quantity
    - Discount
    - Total Price after Discount
    - Grand Total
![Bill](https://github.com/ajaman190/ETG_Inventory_Management_System_Project/blob/main/Images/Screenshot%202021-09-06%20203138.png)

  
## Transaction Feature

    - Stored in purchasedRecord.json
  
        - Customer ID
        - Product ID
        - Product Name
        - Purchased quantity
        - Total Price

  ![Purchased Record](https://github.com/ajaman190/ETG_Inventory_Management_System_Project/blob/main/Images/Screenshot%202021-09-06%20203219.png)

## Working of Code


```bash
● Press 'A' - To Add new product in the inventory

                - Call checkItem() funtion, to check wether it is already present in the inventory or not

                    - If present, throw a message that it is already available in the inventory, you need to update it and call updateItem() function
                    - If it is not there then it will call addItem() funtion

● Press 'B' - To Buy mutiple products at a time

                - Ask you to enter the product id:
                    - If the product id is not available, then it will ask you to enter a valid product id
                    - If the product id will available:

                            - Then ask you to enter the product quantity that you want to buy:
                            - If required product quantity is available in stock:
                                    - It will update the product quantity and product stock price in products dict
                                    - Save the purchased date/time, product name, quantity and total price
                                    - Call purchaseRecord() funtion to store the details of sold product in json format
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

● Press 'C' - To Print product list

● Press 'D' - To Update product details in the inventory

                - Call checkItem() funtion, to check wether it is already present in the inventory or not

                    - If present, then it will call updateItem() funtion 
                    - If it is not there then throw a message that it is not available in the inventory, you need to add it and call addItem() function


● Press 'P' - To print the purchase detail of Customer with their customer id.
                  
                - Call purchaseDetial() funtion and ask to enter customer id.

● Press 'E' - To Exit
```

  
## 🚀 About Me
I'm Aman Kumar. I am a 2nd year undergraduate of IIT Kharagpur and I have successfully completed my first mini project of Inventory Management System given by ETG in Skill India Python for ML/AI Internship. Thanks for giving us such a great opportunity to enhance our skills.



## 🔗 Contact Me

[![portfolio](https://github.com/ajaman190/ETG_Inventory_Management_System_Project/blob/main/Images/Social%20Media%20Logo/1964417_github_logo_media_social_icon.png)](https://github.com/ajaman190)[![kaggle](https://github.com/ajaman190/ETG_Inventory_Management_System_Project/blob/main/Images/Social%20Media%20Logo/4373210_kaggle_logo_logos_icon.png)](https://www.kaggle.com/aman190)[![linkedin](https://github.com/ajaman190/ETG_Inventory_Management_System_Project/blob/main/Images/Social%20Media%20Logo/5296501_linkedin_network_linkedin%20logo_icon.png)](https://www.linkedin.com/in/aman-kumar-586b23216/)

