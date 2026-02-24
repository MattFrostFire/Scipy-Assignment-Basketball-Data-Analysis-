# Scipy-Assignment-Basketball-Data-Analysis-
This program filters data in a csv file containing basketball data from different leagues around the world to only show NBA data. It identifies the NBA player with the most seasons played in a csv file, then it prints out data about the player, linear regression, and summary statistics. After the program is finished a csv file with data on the player with most seasons played is exported to the same directory as the ipynb file along with a linear regression image. :)

*Additional code for the three best players is located below the linear regression graph, and compares the top three players who scored the most points overall, and the top 3 players who scored the most points per game*

**Purpose:**
  
  To apply the scipy ecosystem (stats, integrate, interpolate) to analyze real-world basketball data, uncovering career trends and performing hypothesis testing on player performance metrics.

**Class Design & Implementation**

    The solution is structured around a data-driven approach:
    
    Data Ingestion: Reading the CSV using pandas.
    
    Filtering: Utilizing boolean indexing for NBA-specific insights.
    
    Numerical Analysis: Using linregress for trends and quad for smoothing.
    
    Prediction: Using interp1d to fill gaps in historical data.

**Attributes & Methods**
  
  _Dataframe: The core dataset containing player names, seasons, and shooting stats._
    
  _player_data.to.csv: A method that saves the Player with most played seasons' data to computer as csv with name f'{top_player} to insure player name is known and not separated from printed data._
      
  _integrate_accuracy(): A method that defines the regression function and calculates the area under the curve to find the average._
      
  _compare_t_tests(): A method to evaluate the difference between paired and independent sample variances._

**Limitations**
  
    Historical Gap: The dataset starts in 1999. Any players who began their careers before 1999 (like Vince Carter) have incomplete early-career data.
  
    Linear Assumption: A linear fit assumes a constant rate of change, which may not capture the "peak and decline" arc of a typical athletic career.

