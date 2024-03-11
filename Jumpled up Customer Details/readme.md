## Jumbled Customer Details
The excel file contains some jumbled details of customers like customer name, address, age and gender. All of these details were there in a single line. 

And we need to transform this data into specific name, address, age and gender columns.

![1  Uncleaned data](https://github.com/fazilcmohammed/Data-Cleaning-in-Excel/assets/140707546/0a1f5601-6066-4aaa-a2a5-22e32089c04a)


## Cleaning the data
### __1) Text To Columns :__

I am going to seperate the single cell with the help of Text To Column feature in MS-Excel. We can use this option when we have delimiters on the specific column. In this case, fortunately we have some delimiters after name, address, age and gender. And the delimiter is the (-) symbol.

![2  delimiter](https://github.com/fazilcmohammed/Data-Cleaning-in-Excel/assets/140707546/ca65c964-718a-4243-be57-01d84312c467)

Here is the result.

![3](https://github.com/fazilcmohammed/Data-Cleaning-in-Excel/assets/140707546/a1ebb841-6f07-4a37-b926-148d05f1bf94)

### __2) Combining Names of Customers :__

Now, I am joining the names of customers which lies in two seperate columns with the help of __CONCAT__ function.   
__CONCAT__ allows us to combine text from different cells into one cell.

![4](https://github.com/fazilcmohammed/Data-Cleaning-in-Excel/assets/140707546/dd64bb4d-28a7-4f25-ba56-89a2dd902066)

And this is what happended...

![5](https://github.com/fazilcmohammed/Data-Cleaning-in-Excel/assets/140707546/58498da1-6b10-4bfb-b09b-872bf85dd8eb)

