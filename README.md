# CodeOps-Tech
Task to read data and print without exact and semantic duplicates
Task to complete: 
From a dataset
Print the contents in a human readable format, e.g.: “San Antonio CyberSecurity Conference”,  November 6th, 2019, San Antonio, TX, US, Paid. https://futureconevents.com/events/san-antonio/” 
Identify exact duplicates (if any)
Identify semantic duplicates (i.e., the conferences are same but the details provided are slightly different, e.g., “React Conference 2019” in one entry and “ReactConf ‘19” in another entry but the other fields are same or similar). 

Loaded JSON dataset in dataframe
Checked the keys of JSON data and their valuetypes
"paid" and "free" types were found to have the required data
Extracted both types separately in pandas dataframe, transposed them
Concatinated the two dataframes to get one dataframe
Checked and removed excat duplicates
Stored the original dataframe in another variable for future reference while printing
Now converted data into a standard format by converting all strings to lower, 
removing spaces from before and after texts,
matched words from a hash table
After this duplicates are again checked and deleted
Now for semantic duplicates, compared records with same 'confStartDate','city','state','country','entryType'
and looked for similarity in pairs of their 'confName', if similar then one of them is removed from dataframe
The indexes of the clean dataframe is used to print data from the original dataframe.
