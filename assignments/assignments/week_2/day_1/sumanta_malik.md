1:
Answer 500

command: 

sort marks_rand_2000.csv | grep Pakistan marks_rand_2000.csv | wc -l
//
2: 
Answer 100


Second Question
1 : 269

command :
grep Mumbai city_names_orders_rand.csv > mumbai.csv
wc -l mumbai.csv
//
2 : 371

command :
grep Bangalore city_name_rand.csv| wc -l
//
3: 55

command :
sort city_names_orders_rand.csv | uniq -d | uniq -c | wc -l
//
4:Bangalore,Yuli Z. Pratt
 18 orders
 
command :$ uniq -c city_names_orders_rand.csv > city_sorted.csv

$ uniq -d city_sorted.csv

$ sort -r city_sorted.csv
//
5 :Mumbai,Russell T. Compton
	 11 oders

command : grep Mumbai city_names_orders_rand.csv | uniq -c
//

Question Part :3
1: 1218

command : git log > commit.txt
		grep commit commit.txt
//
4 : 53

command :sort commt.txt | grep Jan commt.txt | grep 2018 commt.txt | wc -l
//	
5 : 3

command :sort commt.txt | grep Sunday commt.txt | grep 2019 commt.txt | wc -l
		



 



