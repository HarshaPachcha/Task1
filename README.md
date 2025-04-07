# Task1
Summary of Data Cleaning Steps of Netflix Data Analytcs

I started by loading the Netflix dataset into a Pandas DataFrame.

I removed all duplicate rows to ensure there were no repeated records in the dataset.

I checked for missing values and handled them accordingly.
For columns like director, cast, and country, I replaced missing values with "Not Specified" to maintain consistency.
In the date_added column, I filled missing entries using forward fill (ffill) to propagate the last valid date.
I filled missing values in the rating column using the most frequent value (mode).
For any missing durations, I filled them with "Unknown" to avoid blanks.

I standardized text formatting by removing leading/trailing spaces and converting:
the type column to Title Case (e.g., "movie" → "Movie"),the country column to Title Case (e.g., "united states" → "United States"),and the rating column to Uppercase (e.g., "pg" → "PG").

I converted the date_added column to a consistent datetime format.

I renamed all column headers to lowercase and replaced spaces with underscores to improve readability and code usability.

I ensured all data types were correct, like setting release_year as an integer and date_added as a datetime object.
Finally, I exported the cleaned dataset to a new CSV file named netflix_titles_cleaned.csv.

