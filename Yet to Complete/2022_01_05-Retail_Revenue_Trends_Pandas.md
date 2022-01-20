Given the table below, called 'orders', write code to show the average revenue by month by channel. The format of the result should look like the following:


    

    
Month | Channel | Avg. Revenue

    

    
    
    
order_id	channel	date	month	revenue
0	1	Online	2018-09-01	09	100
1	2	Online	2018-09-03	09	125
2	3	In_store	2018-10-11	10	200
3	4	In_store	2018-08-21	08	80
4	5	Online	2018-08-13	08	200
5	6	Online	2018-10-29	10	100
    

    
Here is code to create the above dataframe, to help get you started:


    
    
import pandas as pd
    

raw_data = {'order_id': [1, 2, 3, 4, 5, 6],'channel': ['Online', 'Online', 'In_Store', 'In_Store', 'Online', 'Online'], 'date': ['2018-09-01', '2018-09-03', '2018-10-11', '2018-08-21', '2018-08-13', '2018-10-29'], 'month': ['09', '09', '10', '08', '08', '10'],'revenue' :[100, 125, 200, 80, 200, 100]}
    

df = pd.DataFrame(raw_data, columns = ['order_id', 'channel', 'date', 'month', 'revenue'])