# Museum of Modern Art :classical_building: 
This is Brenda Roman repository containing solutions for the technical test

# Approching the Test
By solving this test I face some difficulties not only with the data itself but also with the way of solving like different scenarios impacting the solution

## Drive through Approching

* Set the libraries and the connection to the data then ensure the record data and fields match so we can get down to work!
* Analyze the fields for each table to get more used to the data and read the question one by one

## Detail Questions

* SQL : Which artist in this data set lived the longest? 
  * The first thing here is involving characteristics from artists table, we have death year and birth year so the operation will be death year - birth year and as some records are not provided we need to ensure to take the provided ones, the result was a company, not an artist, so look for the top 4 and the next 2 & 3 tied with 108 years
  * For the previous solution we are not counting on the artists that still alive and pass the threshold of 108 years so I test and for this we cannot assure who still alive and which is just missing values

* SQL : Who are the top 10 artists by the number of artworks?
  * Here we need to join the two tables artist & artworks, first to ensure the full artists listed appearing and count the artwortks (Artwork ID)
  * This question also have a second solution option this required only one table (artworks) grouping by Artist but some artworks has no linked artist
  
* SQL Which artist is created the most artwork by total surface area?
  * SDSD
  
* SQL : Did any artists have artwork acquired during their lifetime?
  * DDS
  
* Please review the quality of the data, and present any issues
  * Artist Table: 
    * The artist names is not homologate, meaning that it could be written First name, First Name and Second name, First letter of second name and first name, there was no nulls here
    * Nationality has 3310 null values, the data type is series
    * Gender has 6196 nulls and 5 males in lower case that doesnt fit Male category
    * Birth Year (7155) & Death Year (45211) have several null values so it impacted into two questions and are floats instead of int
   * Artwork Table:
     * Artist ID, presents in some of them more than one id and some with null values so we cannot link completly with artist table
     * Date field as well present non homologate values 
   
* SQL : Please group the artworks into as many clusters as you feel is appropriate, using attributes from both the artist and artworks tables, and assign each artwork to this new cluster. 


# Thanks!

Thanks to the team and time involved into review this test :grinning:

I really enjoy doing this test and find out the insights of the different industries like Arts
