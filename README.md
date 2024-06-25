# MySQL

# Collect the dataset from this link or collect from the attachment section
https://archive.ics.uci.edu/ml/datasets/bank+marketing

# for showing all database

    show databases 

# create database 

    create database database_name 

# use database

    use database_name 


# Create a table inside of the database(bank_details is the table name) and the entered data is  the column name. default, day, the month is a keywork of SQL if you need to keep it as a column name then you need to use `` this symbol. Otherwise can't work
# Coloum Names with data type: 

    CREATE TABLE IF NOT EXISTS bank_details (
        age INT,
        job VARCHAR(30),
        marital VARCHAR(30),
        education VARCHAR(30),
        `default` VARCHAR(30),
        balance INT, 
        housing VARCHAR(30),
        loan VARCHAR(30), 
        contact VARCHAR(30),
        `day` INT,
        `month` VARCHAR(30), 
        duration INT, 
        campaign INT,
        pdays INT, 
        previous INT, 
        poutcome VARCHAR(30), 
        y VARCHAR(30)
    );

# Show the table
    SELECT * FROM bank_details 
# Insert the one value/row inside of table 
    INSERT INTO bank_details VALUES (58,"management","married","tertiary","no",2143,"yes","no","unknown",5,"may",261,1,-1,0,"unknown","no") 
# Inset the blug values/rows inside of table
    INSERT INTO bank_details VALUES 
    (58,"management","married","tertiary","no",2143,"yes","no","unknown",5,"may",261,1,-1,0,"unknown","no"),
    (44,"technician","single","secondary","no",29,"yes","no","unknown",5,"may",151,1,-1,0,"unknown","no"),
    (33,"entrepreneur","married","secondary","no",2,"yes","yes","unknown",5,"may",76,1,-1,0,"unknown","no"),
    (47,"blue-collar","married","unknown","no",1506,"yes","no","unknown",5,"may",92,1,-1,0,"unknown","no"),
    (33,"unknown","single","unknown","no",1,"no","no","unknown",5,"may",198,1,-1,0,"unknown","no"),
    (35,"management","married","tertiary","no",231,"yes","no","unknown",5,"may",139,1,-1,0,"unknown","no"),
    (28,"management","single","tertiary","no",447,"yes","yes","unknown",5,"may",217,1,-1,0,"unknown","no"),
    (42,"entrepreneur","divorced","tertiary","yes",2,"yes","no","unknown",5,"may",380,1,-1,0,"unknown","no"),
    (58,"retired","married","primary","no",121,"yes","no","unknown",5,"may",50,1,-1,0,"unknown","no"),
    (43,"technician","single","secondary","no",593,"yes","no","unknown",5,"may",55,1,-1,0,"unknown","no"),
    (41,"admin.","divorced","secondary","no",270,"yes","no","unknown",5,"may",222,1,-1,0,"unknown","no"),
    (29,"admin.","single","secondary","no",390,"yes","no","unknown",5,"may",137,1,-1,0,"unknown","no"),
    (53,"technician","married","secondary","no",6,"yes","no","unknown",5,"may",517,1,-1,0,"unknown","no"),
    (58,"technician","married","unknown","no",71,"yes","no","unknown",5,"may",71,1,-1,0,"unknown","no"),
    (57,"services","married","secondary","no",162,"yes","no","unknown",5,"may",174,1,-1,0,"unknown","no"),
    (51,"retired","married","primary","no",229,"yes","no","unknown",5,"may",353,1,-1,0,"unknown","no"),
    (45,"admin.","single","unknown","no",13,"yes","no","unknown",5,"may",98,1,-1,0,"unknown","no"),
    (57,"blue-collar","married","primary","no",52,"yes","no","unknown",5,"may",38,1,-1,0,"unknown","no"),
    (60,"retired","married","primary","no",60,"yes","no","unknown",5,"may",219,1,-1,0,"unknown","no"),
    (33,"services","married","secondary","no",0,"yes","no","unknown",5,"may",54,1,-1,0,"unknown","no"),
    (28,"blue-collar","married","secondary","no",723,"yes","yes","unknown",5,"may",262,1,-1,0,"unknown","no"),
    (56,"management","married","tertiary","no",779,"yes","no","unknown",5,"may",164,1,-1,0,"unknown","no"),
    (32,"blue-collar","single","primary","no",23,"yes","yes","unknown",5,"may",160,1,-1,0,"unknown","no"),
    (25,"services","married","secondary","no",50,"yes","no","unknown",5,"may",342,1,-1,0,"unknown","no"),
    (40,"retired","married","primary","no",0,"yes","yes","unknown",5,"may",181,1,-1,0,"unknown","no"),
    (44,"admin.","married","secondary","no",-372,"yes","no","unknown",5,"may",172,1,-1,0,"unknown","no"),
    (39,"management","single","tertiary","no",255,"yes","no","unknown",5,"may",296,1,-1,0,"unknown","no"),
    (52,"entrepreneur","married","secondary","no",113,"yes","yes","unknown",5,"may",127,1,-1,0,"unknown","no"),
    (46,"management","single","secondary","no",-246,"yes","no","unknown",5,"may",255,2,-1,0,"unknown","no"),
    (36,"technician","single","secondary","no",265,"yes","yes","unknown",5,"may",348,1,-1,0,"unknown","no"),
    (57,"technician","married","secondary","no",839,"no","yes","unknown",5,"may",225,1,-1,0,"unknown","no"),
    (49,"management","married","tertiary","no",378,"yes","no","unknown",5,"may",230,1,-1,0,"unknown","no"),
    (60,"admin.","married","secondary","no",39,"yes","yes","unknown",5,"may",208,1,-1,0,"unknown","no"),
    (59,"blue-collar","married","secondary","no",0,"yes","no","unknown",5,"may",226,1,-1,0,"unknown","no"),
    (51,"management","married","tertiary","no",10635,"yes","no","unknown",5,"may",336,1,-1,0,"unknown","no"),
    (57,"technician","divorced","secondary","no",63,"yes","no","unknown",5,"may",242,1,-1,0,"unknown","no"),
    (25,"blue-collar","married","secondary","no",-7,"yes","no","unknown",5,"may",365,1,-1,0,"unknown","no"),
    (53,"technician","married","secondary","no",-3,"no","no","unknown",5,"may",1666,1,-1,0,"unknown","no"),
    (36,"admin.","divorced","secondary","no",506,"yes","no","unknown",5,"may",577,1,-1,0,"unknown","no"),
    (37,"admin.","single","secondary","no",0,"yes","no","unknown",5,"may",137,1,-1,0,"unknown","no"),
    (44,"services","divorced","secondary","no",2586,"yes","no","unknown",5,"may",160,1,-1,0,"unknown","no"),
    (50,"management","married","secondary","no",49,"yes","no","unknown",5,"may",180,2,-1,0,"unknown","no"),
    (60,"blue-collar","married","unknown","no",104,"yes","no","unknown",5,"may",22,1,-1,0,"unknown","no"),
    (54,"retired","married","secondary","no",529,"yes","no","unknown",5,"may",1492,1,-1,0,"unknown","no"),
    (58,"retired","married","unknown","no",96,"yes","no","unknown",5,"may",616,1,-1,0,"unknown","no"),
    (36,"admin.","single","primary","no",-171,"yes","no","unknown",5,"may",242,1,-1,0,"unknown","no"),
    (58,"self-employed","married","tertiary","no",-364,"yes","no","unknown",5,"may",355,1,-1,0,"unknown","no"),
    (44,"technician","married","secondary","no",0,"yes","no","unknown",5,"may",225,2,-1,0,"unknown","no"),
    (55,"technician","divorced","secondary","no",0,"no","no","unknown",5,"may",160,1,-1,0,"unknown","no"),
    (29,"management","single","tertiary","no",0,"yes","no","unknown",5,"may",363,1,-1,0,"unknown","no"),
    (54,"blue-collar","married","secondary","no",1291,"yes","no","unknown",5,"may",266,1,-1,0,"unknown","no"),
    (48,"management","divorced","tertiary","no",-244,"yes","no","unknown",5,"may",253,1,-1,0,"unknown","no"),
    (32,"management","married","tertiary","no",0,"yes","no","unknown",5,"may",179,1,-1,0,"unknown","no"),
    (42,"admin.","single","secondary","no",-76,"yes","no","unknown",5,"may",787,1,-1,0,"unknown","no"),
    (24,"technician","single","secondary","no",-103,"yes","yes","unknown",5,"may",145,1,-1,0,"unknown","no"),
    (38,"entrepreneur","single","tertiary","no",243,"no","yes","unknown",5,"may",174,1,-1,0,"unknown","no"),
    (38,"management","single","tertiary","no",424,"yes","no","unknown",5,"may",104,1,-1,0,"unknown","no"),
    (47,"blue-collar","married","unknown","no",306,"yes","no","unknown",5,"may",13,1,-1,0,"unknown","no"),
    (40,"blue-collar","single","unknown","no",24,"yes","no","unknown",5,"may",185,1,-1,0,"unknown","no"),
    (46,"services","married","primary","no",179,"yes","no","unknown",5,"may",1778,1,-1,0,"unknown","no"),
    (32,"admin.","married","tertiary","no",0,"yes","no","unknown",5,"may",138,1,-1,0,"unknown","no"),
    (53,"technician","divorced","secondary","no",989,"yes","no","unknown",5,"may",812,1,-1,0,"unknown","no"),
    (57,"blue-collar","married","primary","no",249,"yes","no","unknown",5,"may",164,1,-1,0,"unknown","no"),
    (33,"services","married","secondary","no",790,"yes","no","unknown",5,"may",391,1,-1,0,"unknown","no"),
    (49,"blue-collar","married","unknown","no",154,"yes","no","unknown",5,"may",357,1,-1,0,"unknown","no"),
    (51,"management","married","tertiary","no",6530,"yes","no","unknown",5,"may",91,1,-1,0,"unknown","no"),
    (60,"retired","married","tertiary","no",100,"no","no","unknown",5,"may",528,1,-1,0,"unknown","no"),
    (59,"management","divorced","tertiary","no",59,"yes","no","unknown",5,"may",273,1,-1,0,"unknown","no"),
    (55,"technician","married","secondary","no",1205,"yes","no","unknown",5,"may",158,2,-1,0,"unknown","no"),
    (35,"blue-collar","single","secondary","no",12223,"yes","yes","unknown",5,"may",177,1,-1,0,"unknown","no"),
    (57,"blue-collar","married","secondary","no",5935,"yes","yes","unknown",5,"may",258,1,-1,0,"unknown","no"),
    (31,"services","married","secondary","no",25,"yes","yes","unknown",5,"may",172,1,-1,0,"unknown","no"),
    (54,"management","married","secondary","no",282,"yes","yes","unknown",5,"may",154,1,-1,0,"unknown","no"),
    (55,"blue-collar","married","primary","no",23,"yes","no","unknown",5,"may",291,1,-1,0,"unknown","no"),
    (43,"technician","married","secondary","no",1937,"yes","no","unknown",5,"may",181,1,-1,0,"unknown","no"),
    (53,"technician","married","secondary","no",384,"yes","no","unknown",5,"may",176,1,-1,0,"unknown","no"),
    (44,"blue-collar","married","secondary","no",582,"no","yes","unknown",5,"may",211,1,-1,0,"unknown","no"),
    (55,"services","divorced","secondary","no",91,"no","no","unknown",5,"may",349,1,-1,0,"unknown","no"),
    (49,"services","divorced","secondary","no",0,"yes","yes","unknown",5,"may",272,1,-1,0,"unknown","no"),
    (55,"services","divorced","secondary","yes",1,"yes","no","unknown",5,"may",208,1,-1,0,"unknown","no"),
    (45,"admin.","single","secondary","no",206,"yes","no","unknown",5,"may",193,1,-1,0,"unknown","no"),
    (47,"services","divorced","secondary","no",164,"no","no","unknown",5,"may",212,1,-1,0,"unknown","no"),
    (42,"technician","single","secondary","no",690,"yes","no","unknown",5,"may",20,1,-1,0,"unknown","no"),
    (59,"admin.","married","secondary","no",2343,"yes","no","unknown",5,"may",1042,1,-1,0,"unknown","yes"),
    (46,"self-employed","married","tertiary","no",137,"yes","yes","unknown",5,"may",246,1,-1,0,"unknown","no"),
    (51,"blue-collar","married","primary","no",173,"yes","no","unknown",5,"may",529,2,-1,0,"unknown","no"),
    (56,"admin.","married","secondary","no",45,"no","no","unknown",5,"may",1467,1,-1,0,"unknown","yes"),
    (41,"technician","married","secondary","no",1270,"yes","no","unknown",5,"may",1389,1,-1,0,"unknown","yes"),
    (46,"management","divorced","secondary","no",16,"yes","yes","unknown",5,"may",188,2,-1,0,"unknown","no"),
    (57,"retired","married","secondary","no",486,"yes","no","unknown",5,"may",180,2,-1,0,"unknown","no"),
    (42,"management","single","secondary","no",50,"no","no","unknown",5,"may",48,1,-1,0,"unknown","no"),
    (30,"technician","married","secondary","no",152,"yes","yes","unknown",5,"may",213,2,-1,0,"unknown","no"),
    (60,"admin.","married","secondary","no",290,"yes","no","unknown",5,"may",583,1,-1,0,"unknown","no"),
    (60,"blue-collar","married","unknown","no",54,"yes","no","unknown",5,"may",221,1,-1,0,"unknown","no"),
    (57,"entrepreneur","divorced","secondary","no",-37,"no","no","unknown",5,"may",173,1,-1,0,"unknown","no"),
    (36,"management","married","tertiary","no",101,"yes","yes","unknown",5,"may",426,1,-1,0,"unknown","no"),
    (55,"blue-collar","married","secondary","no",383,"no","no","unknown",5,"may",287,1,-1,0,"unknown","no"),
    (60,"retired","married","tertiary","no",81,"yes","no","unknown",5,"may",101,1,-1,0,"unknown","no"),
    (39,"technician","married","secondary","no",0,"yes","no","unknown",5,"may",203,1,-1,0,"unknown","no"),
    (46,"management","married","tertiary","no",229,"yes","no","unknown",5,"may",197,1,-1,0,"unknown","no");

# Showing all rows of table
    select count(*) FROM bank_details 
# Count the row number or check how many data have inside the table  
    select count(*) FROM bank_details 
# Show all data inside of a table
    SELECT * FROM bank_details 
# Filter the table with age, loan, and job  column
    SELECT age , loan , job from bank_details 
# Default is a keywork of SQL if you need to keep it as a column name then need to use `` this symbol. Otherwise can't work
    select `default` from bank_details 
# Filter the only 8 rows from this table
    select * from bank_details limit 8 
# Filter the data by age
    select * from bank_details where age = 33 
# Filter
    select * from bank_details where age > 40 
# Filter
    select * from bank_details where age = 60
# Multipule filter
    select * from bank_details where age = 60 and job = 'retired' 
# Show table full data
    SELECT * FROM bank_details 
# Multipule condition filter
    select * from bank_details where education = 'unknown' or marital = 'single' 
# Multipule condition filter
    select * from bank_details where (education = 'unknown' or marital = 'single') and balance < 500 
# Filter the unique value of the column
    select distinct job from bank_details
# Defult filter by ascending order
    select *from bank_details order by age 
# Defult filter by ascending order
    select *from bank_details order by marital 
# Filter by descending order
    select *from bank_details order by age desc
# Filter by descending order
    select *from bank_details order by marital desc 

## Problem Solving
# 1. Try to find out the average balance
    select avg(balance) as average_balance from bank_details
# 2. Try to find out who has a minimum balance
    select * from bank_details where balance = (select min(balance) from bank_details)
# 3. Try to find out who has a maximum balance
    select * from bank_details where balance = (select max(balance) from bank_details)
# 4. Try to prepare a list of all the people who have loans
    select * from bank_details where loan = 'yes'
# 5. Try to find out the average balance for all the people whose job role is admin 
    select avg(balance) AS average_blance_for_admin from bank_details where job = 'admin.'
# 6. Try to find-out a record retired job whose age is below 45
    select * from bank_details where job = 'retired' and age < 45
# 7. Try to find-out a record where education is primary and the person is jobless 
    select * from bank_details where job = 'retired' and education = 'primary'
# 8. Try to find a record whose bank account has a negative balance
    select * from bank_details where balance < 0
# 9. Try to find out a record of who does not have a house
    select * from bank_details where housing = "no"

# Create function by procedure.

# Show the bank_details table by using the function
    DELIMITER &&
    create procedure bank_details_table()
    begin
    	select * from bank_details ;
    end &&
    
    call bank_details_table()

# Dinamic function: Create a function to find out a list of all the people who have and haven't any loans.
    DELIMITER &&
    create procedure loan_details(IN a varchar(30)) 
    begin
        select * from bank_details where loan = a ;
    END &&
    
    call loan_details( 'no' )
    call loan_details( 'Yes' )
# Dinamic function: Create a function with 2 variables.  where you can filter by education and Job status.
    DELIMITER &&
    create procedure sel_job_edu (In j varchar(30) , IN e Varchar(30))
    begin
    	select * from bank_details where job = j and education = e ;
    END &&
    
    call sel_job_edu('admin.','secondary')

# Create subtable by View

    create view bank_view as select age, job, balance, marital, education from bank_details ;
    select avg(balance) AS average_blance_for_admin from bank_view where job = 'admin.'


# DATASET:2 Dress 

# Create a table inside of database
    create table if not exists dress(
    Dress_ID int,
    Style varchar(30),
    Price Varchar(30),
    Rating int,
    Size varchar(30),
    Season Varchar(30),
    NeckLine Varchar(30),
    SleeveLength Varchar(30),
    waiseline Varchar(30),
    Material Varchar(30),
    FabricType Varchar(30),
    Decoration Varchar(30),
    `Pattern Type` Varchar(30),
    Recommendation int)
