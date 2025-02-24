# Analysis of the Russian Film Distribution Market

This project focuses on analyzing the Russian film distribution market, with an emphasis on films that received government support. The study is conducted for the Ministry of Culture of the Russian Federation to identify current trends in the film industry and understand how appealing government-supported films are to audiences.

## Data Description

The project uses two datasets:

- **mkrf_movies.csv**: Contains information about film distribution certificates, box office revenues, government support, and other film characteristics.
- **mkrf_shows.csv**: Contains data on film box office revenues in Russian cinemas.

### Data Structure

#### `mkrf_movies` Table

| Column                | Description                                                                 |
|-----------------------|-----------------------------------------------------------------------------|
| `title`               | Film title                                                                   |
| `puNumber`            | Film distribution certificate number                                          |
| `show_start_date`     | Film premiere date                                                           |
| `type`                | Film type (e.g., "Feature", "Documentary")                                    |
| `film_studio`         | Film production studio                                                       |
| `production_country`  | Country of film production                                                   |
| `director`            | Director                                                                     |
| `producer`            | Producer                                                                     |
| `age_restriction`     | Age restriction                                                              |
| `refundable_support`  | Amount of refundable government support                                       |
| `nonrefundable_support`| Amount of nonrefundable government support                                   |
| `financing_source`    | Source of government financing                                               |
| `budget`              | Total film budget (including government support)                              |
| `ratings`             | Film rating on KinoPoisk                                                      |
| `genres`              | Film genre                                                                   |

#### `mkrf_shows` Table

| Column      | Description                                     |
|-------------|-------------------------------------------------|
| `puNumber`  | Film distribution certificate number            |
| `box_office`| Box office revenues of the film in Russian cinemas|

## Steps for Execution

1. **Merging Data**: Merge the data from both tables, ensuring that all films from `mkrf_movies` are included in the final dataframe.

2. **Data Preprocessing**:
   - Check and convert data types where necessary.
   - Handle missing values and duplicates, explaining the rationale behind the handling methods.
   - Analyze categorical and quantitative columns, correcting them and creating new columns (e.g., film release year, director's name, genre, and government support share).

3. **Data Analysis**:
   - Analyze the trends in film distribution over the years, including the minimum and maximum box office revenues.
   - Compare the average and median revenues for each year.
   - Investigate how the film's age rating correlates with its box office performance.

4. **Government-Supported Films**:
   - Analyze the financial support for these films, their profitability, and their ratings.

5. **Conclusions**: Summarize findings based on the data analysis.



To run this project, following libraries will be used:

- pandas
- matplotlib
- seaborn

