### Data Gathering

#### Oscar Winning Movie List

This project started with the Oscar Winning Movies List  from 1929 to 2022, file is <Resources/oscar.csv>. File contains the movie name, winning award count and nomination count.

#### API

Using omdb API we are able to request info by movie name. Due to the limitation of daily responses is 1000, The API request is runned by 2 teammates with splitting the rows to use in oscar dataframe. File is wroten at <Resources/oscar_omdb_1.csv> and <_2>.

#### Failed API Requests

Some movie names have punctuation or minor differences, omdb API only accepts exact matches. This is possible to avoid by searching movie names in other channels such as wikipedia API to correct searching titles, but we didn’t get a chance to work on the polish. Most movies are successfully requested.

### Data Cleaning <project1_clean.ipynb>

API ombd is very organized, all data are fulfilled as string including “NA”. For data cleaning part, the strings are converted to numeric data for values, such as Year, rating, boxoffice.

For strings containing multiple categories are splitted, and counted for each category, such as Genre.

Cleaned data is written as <Resources/oscar_clean.csv>.

### Analysis

#### Boxoffice <project1_boxoffice.ipynb> - Jiaolu Xie

Please find a writing summary in <project1_boxoffice.ipynb>.

Additional data are saved at <Resources/boxoffice/>

Output .png files are saved at <boxoffic_output/>


