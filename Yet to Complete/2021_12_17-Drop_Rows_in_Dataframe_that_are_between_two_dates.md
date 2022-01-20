Given the following dataframe, df, drop all the rows where the contract_sign_date is between 2018-09-01 and 2018-10-13 (inclusive):
    


    
    
vendor_id	name	contract_sign_date	total_spend
0	1	vendor_schmendor	2018-09-01	34324
1	2	parts_r_us	2018-09-03	23455
2	3	vendor_king	2018-10-11	77654
3	4	vendor_diagram	2018-08-21	23334
4	5	venny	2018-08-13	94843
5	6	vendtriloquist	2018-10-29	23444
    
Here is code to create the dataframe yourself, to help get you started:


    
    
import pandas as pd
    

raw_data = {'vendor_id': [1, 2, 3, 4, 5, 6], 'name': ['vendor_schmendor', 'parts_r_us', 'vendor_king', 'vendor_diagram', 'venny', 'vendtriloquist'], 'contract_sign_date': ['2018-09-01', '2018-09-03', '2018-10-11', '2018-08-21', '2018-08-13', '2018-10-29'],'total_spend' :[34324, 23455, 77654, 23334, 94843, 23444]}
    

df = pd.DataFrame(raw_data, columns = ['vendor_id', 'name', 'contract_sign_date', 'total_spend'])