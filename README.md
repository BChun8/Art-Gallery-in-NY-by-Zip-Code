# Art-Gallery-in-NY-by-Zip-Code
In this Dashboard, I was looking at NY bourough data and filtering them to see which bourough had art galleries versus boroughs that did not have art galleries. 

DATASET GATHERING:
I gathered the data at www.data.gov and was able to find a database (ART_GALLERY.csv) that had data pertaining to NYC art galleries. Then, I merged (LEFT Join) a dataset that had zip code data with longitutde and latitude data in the US. with the art gallery database.

DATA VISUALIZATION PROCESS:
I created a calculated field in order to count the number of Art Galleries relative to each zip code. Since the column on the dataset was identified by the name of the Art Gallery, I created a calculated field based on the COUNT({Name}) and named it Art Gallery Count. Then I placed this measure on the tooltip.
Then, I created a Calculated Field called ISNULL which identiefied all of fields that were null by Name. ISNULL({Name}). The logic of why I did this was because in the case that a scenario was based where I was to examine art galleries in the United States relative to art galleries in NYC, I wanted to be able to make that distinction. Therefore, in my visualization on the ISNULL legend, areas that are marked blue are art galleries within the NYC data set, while the Orange is beyond the scope of art galleries within NYC.
Furthermore, I used the lasso tool to hone in on the granularity of analysis that I have done to see where that distinction was made.
