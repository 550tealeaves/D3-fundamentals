# d3.line generator

## Dataset
- Obtained dataset from Kaggle that looks at all NBA draft picks from 1990-2021
- [Dataset](https://www.kaggle.com/datasets/benwieland/nba-draft-data) by Ben Wieland

### Cleaning data
1. Filtered out any players that never played after being drafted (NA in Years column)
2. Filtered down to number 1 picks of each team for each year, from 1990-2021 (original dataset contained all picks and it was too large N=1868. Filtered data now has n=32)
3. Renamed some of the columns because I did not know all the acronyms. 
4. After importing the data, used unary operator to convert desired columns to string
5. Parsed draft year

### Drawing
- Tried to create a group for the lines but did not know how to create new set of lines - tried a x1, y1, but did not work
- I had wanted to label lebron's total minutes played in 2023 (51563), the most of any #1 pick. 


![Number 1 NBA pick stats](NBA-stats.jpg)