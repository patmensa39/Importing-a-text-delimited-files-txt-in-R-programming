# Importing-a-text-delimited-files-txt-in-R-programming
# Importing a text delimited files (txt) in R programming 

library(tidyverse) 

### Work stoppages in the United States 
stoppages <- read_delim('http://594442.youcanlearnit.net/workstoppages.txt', delim = '^')

glimpse(stoppages)


### you can also use the delim function to read both csv and tsv file 
###From the previous example, reading the inspections csv file with delim function

inspections <- read_delim('http://594442.youcanlearnit.net/inspections.csv',
                          delim = ',')
glimpse(inspections)

###From the previous example, reading the tsv file with delim function
inpatient <- read_delim('http://594442.youcanlearnit.net/inpatient.tsv', 
                      delim = '\t')
glimpse(inpatient)
