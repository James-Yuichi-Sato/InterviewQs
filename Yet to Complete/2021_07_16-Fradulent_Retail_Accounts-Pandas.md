Below is a daily table for an active acount at Shopify (an online ecommerce, retail platform). The table is called store_account and the columns are:
    

    

Column Name	Data Type	Description
store_id	integer	a unique Shopify store id
date	string	date
status	string	Possible values are: [‘open’, 'closed’, ‘fraud’]
revenue	double	Amount of spend in USD

    

    
Here's some additional information about the table:
    


    
The granularity of the table is store_id and day

    
Assume “closed” and “fraud” are permanent labels

    
Active = daily revenue > 0 

    
Accounts get labeled by Shopify as fraudulent and they no longer can sell product 

    
Every day of the table has every store_id that has ever used Shopify

    

    
    
    
    
    
Given the above, write code using Python (Pandas library) to show what percent of active stores were fraudulent by day. 
    

    

    
Some clarifications:
    


        
 We want one value for each day in the month. 

        
A store can be fraudulent and active on same day. E.g. they could generate revenue until 10AM, then be flagged as fradulent from 10AM onward.

    

    (Note: you should be able to write code here given solely the table schema (field names, descriptions above) -- it's fairly common in interviews to be provided the structure of tables and told to write a quick query.)