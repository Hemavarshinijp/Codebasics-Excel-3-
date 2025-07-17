# Codebasics-Excel-3-

In this dataset there were Budget, revenue. I have to convert budget and revenue in INR and USD, Billions to Millions using IF 

# Budget (MIL) --> =IF([@Unit]="Billions",[@Budget]*1000,[@Budget])
# Revenue (MIL) --> =IF([@Unit]="Billions",[@[Revenue ]]*1000,[@[Revenue ]])
# Budget (INR) --> =IF([@[Currency]]="USD",[@[Budget MIL]]*80,[@[Budget MIL]])
# Revenue (INR) --> =IF([@[Currency ]]="USD",[@[Revenue MIL]]*80,[@[Revenue MIL]])
# Budget (USD) --> =IF([@[Currency ]]="INR",[@[Budget MIL]]/80,[@[Budget MIL]])
# Revenue (USD) --> =IF([@[Currency ]]="INR",[@[Revenue MIL]]/80,[@[Revenue MIL]])

Total Budget INR  =SUM(Movies[Budget INR])
Total Revenue INR  =SUM(Movies[Revenue INR])

Total Movies                   =Count(movies[movie_id])
Total Bollywood Movies         =Countif(movies[industry],"Bollywood")
Total Bollywood Revenue INR    =sumif(movies[industry],"Bollywood", movies[revenue inr])
Avg Bollywood Revenue INR      =Total Bollywood Revenue INR/ Total Bollywood Movie
Avg Bollywood Revenue INR %    =Total Bollywood revenue inr/ Total Revenue inr
