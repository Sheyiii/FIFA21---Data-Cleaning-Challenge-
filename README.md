# FIFA21---Data-Cleaning-Challenge-

## Data Cleaning Steps
* Steps taken in Cleaning FIFA Raw Data.
* First step taken was to understand the data and devise methods on how to properly clean and reduce the errors to it lowest.

* I extracted individual player First and Last names by splitting  the Longname column.
* With the use of the appropriate delimiter I was able to Seperate the Start Contract year from the End contract year.
* Removed the Si units in  the Height and weight column then proceeded to convert both columns to the appropriate  with the =convert function. 
* For the value, wage and release clause columns I removed Delimiters and proceeded to change the M to million and K to thousands with the formula: For instance the first cell in value column; =ifna(left(cell, Len(cell)-1)*choose(match(right(cell,1),{“K”,”M”},0),1000,1000000),cell). Then you can apply the formula to the other two columns.
     OR
* With the use of Conditional column on Power Query, for the Value column use the condition where value ends at “k” replace with 1,000 add another column where value ends at “M” replace with 1,000000.

* With Replace value. I was able to replace the irregular characters in W/F, S/M and IR columns.
* The cells which has K in Hits column was also converted to thousand.
* Lastly, I Looked at Individual columns and proceeded to remove columns not needed.
Note: All steps taken can also be done through another method on Power query.
Thank you for reading and for your time.
![The San Juan Mountains are beautiful!](Fifa Dirty data.png…] "San Juan Mountains")
![The San Juan Mountains are beautiful!](Fifa Dirty data 2.png…] "San Juan Mountains")
![The San Juan Mountains are beautiful!](Fifa Dirty data 3.png…] "San Juan Mountains")
![The San Juan Mountains are beautiful!](Fifa Neat Data.png…] "San Juan Mountains")
![The San Juan Mountains are beautiful!](Fifa Neat Data 2.png…] "San Juan Mountains")
![The San Juan Mountains are beautiful!](Fifa Neat Data 3.png…] "San Juan Mountains")
