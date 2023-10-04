Given the following datasets on state population and state deaths and births, create a list that has each state's population growth rate, sorted in descending order. Note you will need to join the two datasets.


                    
To help get you started, the code below loads in the datasets. You can also make a copy of this Google Colab notebook to get started!


                    
                        
# Import packages
                        

import numpy as np
                        

import pandas as pd
                        

# Import the data
                        

data_pop = pd.read_csv("https://raw.githubusercontent.com/erood/interviewqs.com_code_snippets/master/Datasets/us_state_populations.csv") 
                        

data_birth_death = pd.read_csv("https://raw.githubusercontent.com/erood/interviewqs.com_code_snippets/master/Datasets/us_state_births.csv") 
                        

#Display a few records
                        

data_pop.head()
                    

      
    
    
    
                    
State	Population
0	California	39865590
1	Texas	29206997
2	Florida	21299325
3	New York	19542209
4	Pennsylvania	12807060
