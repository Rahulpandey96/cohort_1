# Week 2 - Day 1

**NOTE:** Follow the instructions carefully and follow coding discipline



## FSD.W2.1.A (15 min)

**NOTE: SAVE ALL THE COMMANDS ON HOW YOU ARRIVED AT THE ANSWER YOU NEED TO SUBMIT THEM**

Download the file https://raw.githubusercontent.com/masai-school/assignments-data/master/data/junk/marks_rand_2000.csv

The files contains marks the data of 2000 students from India and Pakistan one for each line in the below format

``` 
23 India 5cf9c9be70765c6c741bd34a
43 Pakistan 5cf9c9be70765c6c741bd352
.
.

```
1. Find the total number of students from Pakistan

```
   500
```

Commands on how you got the answer

```
 grep -i "pakistan" marks_rand_2000.csv |wc -l

```
2. No of students from India who are in the bottom 200 list based on the marks scored
```
 156
```
Commands on how you got the answer

```
 sort -n -r marks_rand_2000.csv | tail -n 200  |grep -i "india"  | wc -l

```


## FSD.W2.1.B (30 min)

**NOTE: SAVE ALL THE COMMANDS ON HOW YOU ARRIVED AT THE ANSWER YOU NEED TO SUBMIT THEM**

Download the file https://raw.githubusercontent.com/masai-school/assignments-data/master/data/junk/city_names_orders_rand.csv
The files contains orders from an e commerce website with the city and name of person who placed the order one for each line in the below format.

``` 
Bangalore,Maggy L. Wiggins
Mumbai,Isadora U. Ward
.
.

```

1. Find the total number of orders from Mumbai

```
 269
```

Commands on how you got the answer

```
 grep -i "mumbai" city_names_orders_rand.csv | wc -l

```
2. Find the total number of users from Bangalore

```
 100
```

Commands on how you got the answer

```
 sort -r city_names_orders_rand.csv |uniq |grep -i "bangalore"|wc -l

```
3. Total no of users who have more than one order

```
  102
```

Commands on how you got the answer

```
 sort city_names_orders_rand.csv |uniq -d | wc -l

```
4. User having the most no of orders
```
USERNAME Pratt 
```
```
COUNT OF ORDERS 18
```
Commands on how you got the answer

```
 sort -r city_names_orders_rand.csv |uniq -c|sort -n -r| head -n 1

```
5. User from Mumbai having the most no of orders
```
USERNAME Russell T. Compton
```
```
COUNT OF ORDERS 11
```
Commands on how you got the answer

```
 sort -r city_names_orders_rand.csv |uniq -c|sort -n -r| grep -i "mumbai"|head -n 1
     
```

## FSD.W2.1.C (30 min)

**NOTE: SAVE ALL THE COMMANDS ON HOW YOU ARRIVED AT THE ANSWER YOU NEED TO SUBMIT THEM**

Clone the repo https://github.com/jlevy/the-art-of-command-line
1. Total no of commits made to the repository
```
 1218
```

Commands on how you got the answer

```
 git log |grep commit|wc -l

```
2. No. of contributors to the repository
```
 190
```

Commands on how you got the answer

```
 git log | grep Author | sort |uniq | wc -l

```

3. User with the maximum no of commits to the repository
```
USER IDENTITY Joshua Levy
```
```
NO OF COMMITS 24
```

Commands on how you got the answer

```
 git log | grep Author | uniq -c | sort -n | tail -n 1

```

4. Commits made in the month of January for the year 2018
```
 8
```
Commands on how you got the answer

```
 git log | grep Author | uniq -c | sort -n | tail -n 1

```
5. Commits made on Sundays for the year 2019
``
 0
```
Commands on how you got the answer

```
 git log | grep Sun |grep 2019 |wc -l

```



## FSD.W2.1.D (15 min)

- Clone the repo https://github.com/masai-school/full-stack-dev inside `~/repos` folder (Pull if the repo already exists)
- Clone the repo https://github.com/masai-school/cohort_1 inside `~/repos` folder (Pull if the repo already exists)
- Navigate to the folder `~/repos/full-stack-dev/`
- Copy the `course/week_2/day_1/w2_day_1_assignments.md` file to the `cohort_1` repository which should be at `~/repos/cohort_1` into the folder `assignments/week_2/day_1` with the name `firstname_lastname.md`
- Open the file `assignments/week_2/day_1/firstname_lastname.md` inside the `cohort_1` repo in the text editor (nano) and fill all the answers
- Sync the `cohort_1` back to the online repository
