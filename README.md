# queries

1. Write a query to list the 10 biggest custermers in last years
db.getcollections("customers").find({year:2015}).limit(10).sort(quantity:1);
2. write a query to list the firstname and phone number for the users who lives in Fremont
db.getcollections("users").find({fn:1,phone:1,_id:0},{city:"Fremont"});
3. write a query to list all the users who's phone area code is 408
db.getcollections("users").find({phone:/408/});
