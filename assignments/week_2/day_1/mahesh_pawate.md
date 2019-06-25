Week 2 - Day 1
NOTE: Follow the instructions carefully and follow coding discipline

FSD.W2.1.A (15 min)
NOTE: SAVE ALL THE COMMANDS ON HOW YOU ARRIVED AT THE ANSWER YOU NEED TO SUBMIT THEM

Download the file https://raw.githubusercontent.com/masai-school/assignments-data/master/data/junk/marks_rand_2000.csv

The files contains marks the data of 2000 students from India and Pakistan one for each line in the below format

23 India 5cf9c9be70765c6c741bd34a
43 Pakistan 5cf9c9be70765c6c741bd352
.
.

Find the total number of students from Pakistan
ANSWER 500
Commands on how you got the answer

<COMMAND 1>  grep Pakistan marks_rand_2000.csv | wc -l > pakistan_std.txt
<COMMAND 2>
<COMMAND 3>
No of students from India who are in the bottom 200 list based on the marks scored
ANSWER
Commands on how you got the answer

<COMMAND 1> sort -n -r marks_rand_2000.csv | tail -n 200 | grep -i india | wc -l
<COMMAND 2>
<COMMAND 3>
FSD.W2.1.B (30 min)
NOTE: SAVE ALL THE COMMANDS ON HOW YOU ARRIVED AT THE ANSWER YOU NEED TO SUBMIT THEM

Download the file https://raw.githubusercontent.com/masai-school/assignments-data/master/data/junk/city_names_orders_rand.csv The files contains orders from an e commerce website with the city and name of person who placed the order one for each line in the below format.

Bangalore,Maggy L. Wiggins
Mumbai,Isadora U. Ward
.
.

Find the total number of orders from Mumbai
ANSWER  269 
Commands on how you got the answer

<COMMAND 1> grep -i mumbai city_names_orders_rand.csv |wc -l
<COMMAND 2>
<COMMAND 3>
Find the total number of users from Bangalore
ANSWER  371
Commands on how you got the answer

<COMMAND 1>   grep -i Bangalore city_names_orders_rand.csv | wc -l
<COMMAND 2>
<COMMAND 3>
Total no of users who have more than one order
ANSWER
Commands on how you got the answer

<COMMAND 1> sort city_names_orders_rand.csv | uniq -d | wc -l
<COMMAND 2>
<COMMAND 3>
User having the most no of orders
USERNAME   18 Bangalore,Yuli Z. Pratt

COUNT OF ORDERS 18
Commands on how you got the answer

<COMMAND 1>  sort city_names_orders_rand.csv | uniq -c | sort -n | tail -n 1
<COMMAND 2>
<COMMAND 3>
User from Mumbai having the most no of orders
USERNAME    Mumbai,Russell T. Compton
COUNT OF ORDERS 11
Commands on how you got the answer

<COMMAND 1> sort city_names_orders_rand.csv | grep -i mumbai | uniq -c | sort -n | tail -n 1
<COMMAND 2>
<COMMAND 3>
FSD.W2.1.C (30 min)
NOTE: SAVE ALL THE COMMANDS ON HOW YOU ARRIVED AT THE ANSWER YOU NEED TO SUBMIT THEM

Clone the repo https://github.com/jlevy/the-art-of-command-line

Total no of commits made to the repository
ANSWER 1218 
Commands on how you got the answer

<COMMAND 1> git log | grep commit | wc -l
<COMMAND 2>
<COMMAND 3>

No. of contributors to the repository
ANSWER  1186
Commands on how you got the answer

<COMMAND 1>  git log | grep Author | wc -l
<COMMAND 2>
<COMMAND 3>
User with the maximum no of commits to the repository
USER IDENTITY Author: Joshua Levy <joshua@cal.berkeley.edu>
NO OF COMMITS 466
Commands on how you got the answer

<COMMAND 1> git log | grep Author | sort |uniq -c|sort -n | tail -n 1
<COMMAND 2>
<COMMAND 3>
Commits made in the month of January for the year 2018
ANSWER  8

Commands on how you got the answer

<COMMAND 1> git log | grep Date | grep 2018 | grep Jan | wc -l
<COMMAND 2>
<COMMAND 3>
Commits made on Sundays for the year 2019
ANSWER 0

Commands on how you got the answer

<COMMAND 1> git log | grep Date |grep -i 2019 | grep sun | wc -l
<COMMAND 2>
<COMMAND 3>