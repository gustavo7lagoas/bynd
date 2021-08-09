# bynd

## Bug 1

### Ticket Example
Title: "Sort By" is not working as expected.
Description: Steps to reproduce:
1. Go to any main category. Example: Women
1. In the Sort by dropdown select an option. Example: "Price: Highest first"
**Expected result**: the list of products should be sorted by the chosen option.
**Actual result**: the list does not get sorted. The loading component is displayed indefinitely.
Check the pictures attached for more details
![sort by issue](https://github.com/gustavo7lagoas/bynd/blob/main/sortBy.png?raw=true)

### Automation proposition
Using Selenium or any other tools perform some sort operations and check the displayed results. For example this dropdown is a HTML form Select with the ID=selectProductSort.
The sorted products can be find by the following CSS locator li.ajax_block_product. Since there is only seven products displayed it is easy to get a sorted list for each of the options available at the dropdown.
Check if the list is sorted by any of the available values in the Sort By dropdown.

## Bug 2

### Ticket Example
Title: Products does not get highlighted in the mobile version.
Description: Steps to reproduce:
1. Change the browser to the mobile version. 
1. Go to a product category. Example Dresses
1. Check the screen displayed
**Expected result**: the products should be easily displayed and highlighted in the mobile version
**Actual result**: the user have to scroll down to see the first product. Check the pictures attached for more details:
**Our website**
![mobile version top](https://github.com/gustavo7lagoas/bynd/blob/main/mobileVersionTop.png?raw=true)
![mobile version product](https://github.com/gustavo7lagoas/bynd/blob/main/mobileVersionProduct.png?raw=true)
**Competidor Website**
![competidor website](https://github.com/gustavo7lagoas/bynd/blob/main/highlightedProduct.png?raw=true)

### Automation proposition
This is a problem that can impact the sales since the user is not seeing products right away after selecting a category. Today we have tools that performs visual testing and can be used in this case. Selenium can be used to do the navigation between pages and Applitools for visual checking.

## Bug 3

### Ticket Example
Title: "Add to cart" does not allow users to select size for quick buy
Description: Steps to reproduce:
1. Mouse Hover a product. 
1. Select add to cart
1. Check the displayed dialog
**Expected result**: user should be able to select size when doing a quick buy by selecting "Add to cart"
**Actual result**: always the size S is select and the user can not change it.  
![shopping cart](https://github.com/gustavo7lagoas/bynd/blob/main/shoppingCart.png?raw=true)
![add to cart](https://github.com/gustavo7lagoas/bynd/blob/main/addToCart.png?raw=true)

### Automation proposition
For this situation after the bug gets fixed it is possible to add a test that performs a add to cart and change the size for selected product. This can be done using Selenium too.


## Bug 4

### Ticket Example
Title: The Categories names displayed are not consistent
Description: Steps to reproduce:
1. Go to Women category 
1. In the list of subcategories, compare the name displayed in the Subcategories component and the Website's navigation
**Expected result**: the subcategory T-Shirts has a higher hierarchy than Tops. It should be consistent with Dresses categorization
**Actual result**: The T-shirt subcategory is displayed it should be Top. Check the pictures attached for more details  
![shopping cart](https://github.com/gustavo7lagoas/bynd/blob/main/Categories.png?raw=true)

### Automation proposition
This is more of a feeling bug. It can even be correct from the business point of view. Automating this situation in the case of displaying the save level of subcategories can be done by using Selenium Webdriver. 
