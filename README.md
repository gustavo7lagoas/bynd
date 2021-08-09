# bynd

## Bug 1

### Ticket Example
Title: "Sort By" is not working as expected.
Description: Steps to reproduce:
1- Go to any main category. Example: Women
2- In the Sort by dropdown select an option. Example: "Price: Highest first"
Expected result: the list of products should be sorted by the chosen option.
Actual result: the list does not get sorted. The loading component is displayed indefinitely.
Check the pictures attached for more details
![alt text](https://github.com/[username]/[reponame]/blob/[branch]/image.jpg?raw=true)
![alt text](https://github.com/[username]/[reponame]/blob/[branch]/image.jpg?raw=true)

### Automation proposition
Using Selenium or any other tools perform some sort operations and check the displayed results. For example this dropdown is a HTML form Select with the ID=selectProductSort.
The sorted products can be find by the following CSS locator li.ajax_block_product. Since there is only seven products displayed it is easy to get a sorted list for each of the options available at the dropdown.
Check if the list is sorted by any of the available values in the Sort By dropdown.

## Bug 2

### Ticket Example
Title: Products does not get highlighted in the mobile version.
Description: Steps to reproduce:
1- Change the browser to the mobile version. 
2- Go to a product category. Example Dresses
3- Check the screen displayed
Expected result: the products should be easily displayed and highlighted in the mobile version
Actual result: the user have to scroll down to see the first product. Check the pictures attached for more details:
![alt text](https://github.com/[username]/[reponame]/blob/[branch]/image.jpg?raw=true)
![alt text](https://github.com/[username]/[reponame]/blob/[branch]/image.jpg?raw=true)

### Automation proposition
This is a problem that can impact the sales since the user is not seeing products right away after selecting a category. Today we have tools that performs visual testing and can be used in this case. Selenium can be used to do the navigation between pages and Applitools for visual checking.

## Bug 3

### Ticket Example
Title: Products does not get highlighted in the mobile version.
Description: Steps to reproduce:
1- Change the browser to the mobile version. 
2- Go to a product category. Example Dresses
3- Check the screen displayed
Expected result: the products should be easily displayed and highlighted in the mobile version
Actual result: the user have to scroll down to see the first product. Check the pictures attached for more details:
![alt text](https://github.com/[username]/[reponame]/blob/[branch]/image.jpg?raw=true)
![alt text](https://github.com/[username]/[reponame]/blob/[branch]/image.jpg?raw=true)

### Automation proposition
This is a problem that can impact the sales since the user is not seeing products right away after selecting a category. Today we have tools that performs visual testing and can be used in this case. Selenium can be used to do the navigation between pages and Applitools for visual checking.

