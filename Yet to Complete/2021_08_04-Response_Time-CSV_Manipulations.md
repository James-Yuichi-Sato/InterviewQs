You are [given](https://raw.githubusercontent.com/erood/interviewqs.com_code_snippets/master/Datasets/sample_message_dataset.csv) a dataset with information around messages sent between users in a P2P messaging application. Below is the dataset's schema:


    
    
Column Name	Data Type	Description
date	string	date of the message sent/received, format is 'YYYY-mm-dd'
timestamp	integer	timestamp of the message sent/received, epoch seconds
sender_id	integer	id of the message sender
receiver_id	integer	id of the message receiver

    

    
Given this, write code to find the fraction of messages that are sent between the same sender and receiver within five minutes (e.g. the fraction of messages that receive a response within 5 minutes). 