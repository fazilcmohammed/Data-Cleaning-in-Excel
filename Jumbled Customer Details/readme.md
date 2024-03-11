# Jumbled Customer Details
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

### __3) Combining Address of Customers :__

Again we are going to combine the address by the __CONCAT__ function. But we are combining all other columns into address.

![6](https://github.com/fazilcmohammed/Data-Cleaning-in-Excel/assets/140707546/7cd7e3b8-039c-49bd-9c3c-a69b599441f0)


And then,

![7](https://github.com/fazilcmohammed/Data-Cleaning-in-Excel/assets/140707546/3a269ddd-1d7b-4b33-a541-f4538bebf2a7)

We can see, the age and gender column also got comnined in this address column. It happened because the length of address is varying from person to person. It's not a big problem, we can solve it easily at the last.

### __4) Extracting Age & Gender :__

Again we are using Text To Column feature for getting the age and gender of the customers from the address column.

![8](https://github.com/fazilcmohammed/Data-Cleaning-in-Excel/assets/140707546/5eed7c57-df9b-45ad-a500-b642a3496545)

And the result is 

![9](https://github.com/fazilcmohammed/Data-Cleaning-in-Excel/assets/140707546/2c56c70f-7813-4e74-a5af-d1e9b4f8940e)


### __4) Removing Unwanted Elements :__

Now, I am going to remove the texts like Age, Gender inside the columns. And giving header to columns.  
For removing unwanted text, I am using __LEFT__ and __FIND__ function. I will combine both the functions to delete the text.  

__Removing Age from address column:__

![10](https://github.com/fazilcmohammed/Data-Cleaning-in-Excel/assets/140707546/6ddb2c81-e551-46a5-aa4e-e9a7c85d0312)

It changed the entire address column.

![11](https://github.com/fazilcmohammed/Data-Cleaning-in-Excel/assets/140707546/797cd790-de10-4f2e-aa26-f382bd9dedc4)

__Removing Age from address column:__

![12](https://github.com/fazilcmohammed/Data-Cleaning-in-Excel/assets/140707546/a514723f-0ed1-4a2b-a435-be30d2ded202)

And then

![13](https://github.com/fazilcmohammed/Data-Cleaning-in-Excel/assets/140707546/363df1e0-d109-48ad-b701-ece9bf101d99)

### __5) Trimming Gender Column :__

There are some spaces at the beginning of the genders and I removed it by using __TRIM__ function. 
Here it is

![14](https://github.com/fazilcmohammed/Data-Cleaning-in-Excel/assets/140707546/a900c245-f169-4500-a25c-1be1d10881a8)

And after trimming

![15](https://github.com/fazilcmohammed/Data-Cleaning-in-Excel/assets/140707546/20345f70-14b6-43da-a4b3-455a353e1dc4)


## __OUTCOME__

![16](https://github.com/fazilcmohammed/Data-Cleaning-in-Excel/assets/140707546/9c43ca9e-73a2-4ac4-a4fb-b68976ce6ace)

## Conclusion

This repository contains a cleaned version of the customer details dataset. The data was originally in a single column, messy spreadsheet and has been transformed into a more organized and usable format suitable for further analysis.
