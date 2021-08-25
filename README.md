<img align="right" src="https://i.pinimg.com/originals/a2/7d/b5/a27db560c85c50c53b53648c234d82e3.jpg" alt="" width="201" height="201" />

# projeto_SharkAttack

 ### Analyze the table and answer the following questions:
## Question 1: For the past 10 years, in which month occorred more shark attacks?

Steps:
-Import the Pandas library
-Read CSV file using encoding = latin-1
- Analyzing the data from flag 0, we can see that due to the variation in the input form, several years were not extracted.
    Option 1: Rewrite the filter so it captures more data. For example, a filter that captures the last 4 digits of the string.
    Option 2: Manually correct the relevant data.
          For the desired period only 5 dates would need correction, so I chose to do the manual correction
- Analyzing the data from flag 0, we can see that due to the variation in the input form, several years were not extracted. Again a manual correction will be made. 
- From the DataFrame 'df' it is observed that despite the Case Number being duplicated, the cases have different information from each other. In other words, it is not a question of duplicated cases, but an error in case numbering. I choose to keep all data 
- By grouping the cases by month, it is possible to observe that September is the month with the highest incidence of shark attacks

## Question 2: Why is there more shark attacks in September? 

- For the year va evaluation it was necessary to collect more data from the original 'df' table, for that a merge was done and duplicates were verified.
      Analyzing the duplicated values, I choose to drop the completely duplicated lines and keep the others 
- For a first assessment, I check the occurrence of shark attacks by activity and compare it to the activities in September. 
- After verifying that there is a rise in cases of shark attacks on surfers in September, I check if this rise is related to any specific region. 
- It is observed that in Florida the cases increase significantly during the month of September 
- Finally, I analyze the occurrence of multiple attacks on the same day, to see if they could be related, making the average attacks in September go up. I find that the attacks on the same day are not related to each other. 

## Conclusion:

### Hypothesis: With Florida's novice surfer season and before the temperature drops due to the arrival of winter plus the fall migration of bait fish to the warm Florida waters, September has a high in cases. 
