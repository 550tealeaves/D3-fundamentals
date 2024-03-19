# d3.line generator

## Dataset
- Obtained dataset from Kaggle that looks at all NBA draft picks from 1990-2021
- [Markdown Guide](https://www.kaggle.com/datasets/benwieland/nba-draft-data)

### Cleaning data
1. Filtered out any players that never played after being drafted (NA in Years column)
2. Filtered down to the top 5 picks of each team for each year, from 1990-2021 (original dataset contained all picks and it was too large N=1868. Filtered data now has n=160)
3. Renamed some of the columns because I did not know all the acronyms. 
4. After importing the data, used unary operator to convert desired columns to string
5. Parsed draft year