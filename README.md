Write queries for the following tasks: 
1. Create a table named 'matches' with appropriate data types for columns 2. Create a table named 'deliveries' with appropriate data types for columns 3. Import data from csv file 'IPL_matches.csv'attached in resources to 'matches'
 4. Import data from csv file 'IPL_Ball.csv' attached in resources to 'matches 5. Select the top 20 rows of the deliveries table. 
6. Select the top 20 rows of the matches table. 
7. Fetch data of all the matches played on 2nd May 2013.
 8. Fetch data of all the matches where the margin of victory is more than 100 runs. 
9. Fetch data of all the matches where the final scores of both teams tied and order it in descending order of the date. 
10. Get the count of cities that have hosted an IPL match. 
11. Create table deliveries_v02 with all the columns of deliveries and an additional column ball_result containing value boundary, dot or other depending on the total_run (boundary for >= 4, dot for 0 and other for any other number) 
12. Write a query to fetch the total number of boundaries and dot balls 
13. Write a query to fetch the total number of boundaries scored by each team 
14. Write a query to fetch the total number of dot balls bowled by each team 
15. Write a query to fetch the total number of dismissals by dismissal kinds 
16. Write a query to get the top 5 bowlers who conceded maximum extra runs 
17. Write a query to create a table named deliveries_v03 with all the columns of deliveries_v02 table and two additional column (named venue and match_date) of venue and date from table matches 
18. Write a query to fetch the total runs scored for each venue and order it in the descending order of total runs scored. 
19. Write a query to fetch the year-wise total runs scored at Eden Gardens and order it in the descending order of total runs scored. 
20. Get unique team1 names from the matches table, you will notice that there are two entries for Rising Pune Supergiant one with Rising Pune Supergiant and another one with Rising Pune Supergiants. Your task is to create a matches_corrected table with two additional columns team1_corr and team2_corr containing team names with replacing Rising Pune Supergiants with Rising Pune Supergiant. Now analyse these newly created columns. 
21. Create a new table deliveries_v04 with the first column as ball_id containing information of match_id, inning, over and ball separated by'(For ex. 335982-1-0-1 match_idinning-over-ball) and rest of the columns same as deliveries_v03) 
22. Compare the total count of rows and total count of distinct ball_id in deliveries_v04; 
23. Create table deliveries_v05 with all columns of deliveries_v04 and an additional column for row number partition over ball_id. (HINT : row_number() over (partition by ball_id) as r_num) 
24. Use the r_num created in deliveries_v05 to identify instances where ball_id is repeating. (HINT : select * from deliveries_v05 WHERE r_num=2;) 
25. Use subqueries to fetch data of all the ball_id which are repeating. (HINT: SELECT * FROM deliveries_v05 WHERE ball_id in (select BALL_ID from deliveries_v05 WHERE r_num=2); 

