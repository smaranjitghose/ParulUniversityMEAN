<h1 align = "center">Practical 2</h1>


Download the [restaurant.json](https://github.com/smaranjitghose/ParulUniversityMEAN/blob/main/practice_problems/datasets/restaurants.json) and add it to a new collection

Answer the following questions using MongoDB:

Q1. Display all the documents in the collection with

  - all fields
  - the fields - restaurant_id, name, borough, and cuisine
  - the fields - restaurant_id, name, borough, and cuisine but excluding the field _id
  - the field zip code excluding the field _id

Q2. From the restaurants present in the borough “Brooklyn”, display the details for:

  - all such restaurants
  - first five such restaurants
  - the next five such restaurants (after skipping the records for first five restaurants)

Q3. Find the restaurants that achieved a score of more than 70.

Q4. Find the restaurants that achieved a score of more than 70 but less than 100.

Q5. Find the restaurants that do not prepare any cuisine of ‘American’ and their grade score of more than 70.

Q6. Find the restaurants which do not prepare any cuisine of ‘American’ and achieved a grade point ‘A’ not belonging to the borough Brooklyn. NOTE: The documents must be displayed according to the cuisine in descending order.

Q7. Find the restaurant Id, name, borough, and cuisine for those restaurants which contain ‘Wil’ as the first three letters of their name.

Q8.  Find the restaurant Id, name, borough, and cuisine for those restaurants which contain ‘Food’ as the last three letters of their name.

Q9. Find the restaurant Id, name, borough, and cuisine for those restaurants which contain ‘Seafood’ as three letters somewhere in their name.

Q10.  Find the restaurants which belong to the borough Bronx and prepared either American or Chinese dishes.

Q11. Find the restaurant Id, name, borough, and cuisine for those restaurants which belong to the borough of Staten Island or Queens, or Bronx Brooklyn.

Q12. Find the restaurant Id, name, borough, and cuisine for those restaurants which do not belong to the borough Staten Island or Queens, or Bronx or Brooklyn

Q13. Find the restaurant Id, name, borough, and cuisine for those restaurants which achieved a score that is not more than 10.

Q14. Write a MongoDB query to find the restaurant Id, name, borough, and cuisine for those restaurants which prepared dishes except ‘American’ and ‘Chinese’ or the restaurant’s name begins with the letter ‘Sea’.

Q15. Arrange the name of the restaurants along with all columns in 

  - descending order 
  - ascending order

Q16.  Arrange the name of the cuisine in ascending order and for that same cuisine, the borough should be in descending order.

Q17. Check whether all the addresses contain the building or not.

Q18. Find the restaurant Id, name, and grades for those restaurants
where the 2nd element of the grades array contains a grade of “A” and score 9 on an ISODate “2013–09–11T00:00:00Z”.

Q19. Find the restaurant Id, name, and grades for those restaurants
which achieved a grade of “A” and scored 11 on an ISODate “2013–09–11T00:00:00Z” among many of the survey dates.

Q20. Select all documents in the restaurants' collection where the coord field value is double.

Q21. Select the restaurant Id, name, and grades for those restaurants which returns 0 as a remainder after dividing the score by 7.

Q22. Find the restaurants with more than three grade surveys (‘grades’ Array contains more than three elements) and display only the name and the number of grades.

Q23. Write an aggregation pipeline to count the number of restaurants in the borough “Bronx”
for each cuisine type. Display the number of restaurants that prepare Caribbean cuisine. A single query is expected that satisfies all the above requirements.
