# excludeEmail
Bash script to remove email addresses from a csv file of users exported from website or database

This is a rather odd and specific script for quickly eliminating certain emails from a set of emails contained in a csv file. 

Due to some rather odd operating requirements, we found ourselves with a csv export of users from a database. We needed to send
emails to these users, but not all of them (a.k.a a list of do not contacts or bad emails). Since, for whatever reason, we couldn't
actually do this in the database, I threw together this script that does it. 

## USAGE: excludeEmail [mainFile.csv] [donotemaillist.txt] >> [output file]

#### MainFile.csv          
The main csv file containing the emails in the 13th column

#### donotemaillist.txt    
The text file containing the emails you want removed from the list. Each email should be on its own line in quotes.

#### Output
By defualt the script prints to the screen. However, by using the redirection operator `>>` you can point the output into
any file you want. 
