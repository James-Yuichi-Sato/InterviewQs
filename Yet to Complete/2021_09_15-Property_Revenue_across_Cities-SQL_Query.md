Suppose you work for Airbnb as an analyst. A team has come to you asking which cities generate the highest revenue for the company in 2017. Using the schemas below, write a SQL query to answer this question.


    
    
You have a table with property location information and another table with stay information. The schema of the tables are below:


    
Table: property_location_info


    
Column Name	Data Type	Description
property_id	integer	ID of the property location
country	string	country code of the property location
city_name	string	name of city (note there can be multiple cities with the same name)
subregion_name	string	provence, state, or subregion name
address	string	address of property location

    

    
Table: stays_info


    
Column Name	Data Type	Description
guest_id	integer	ID of guest
property_id	integer	ID of the property location
host_id	integer	ID of the host managing the property
revenue	integer	cost of stay for guest in USD
date_start	string	start day of stay, format is "YYYY-mm-dd"
date_end	string	end day of stay, format is "YYYY-mm-dd"
stay_length	integer	number of days for the stay
airbnb_revenue	integer	revenue that Airbnb collected on stay
