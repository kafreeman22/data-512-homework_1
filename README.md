# data-512-homework_1
## Keegan Freeman
### 10/6/22

## Project Description

The goal of this project is to practice reproducibility and replicability good practices, as defined in [The Basic Reproducible Workflow Template](http://www.practicereproducibleresearch.org/core-chapters/3-basic.html) and [Assessing Reproducibility](http://www.practicereproducibleresearch.org/core-chapters/2-assessment.html), within a data-science format. The data-science tasks of this project include

  1. Pulling data from Wikipedia using the Pageviews API ([documentation](https://wikitech.wikimedia.org/wiki/Analytics/AQS/Pageviews), [endpoint](https://wikimedia.org/api/rest_v1/#!/Pageviews_data/get_metrics_pageviews_aggregate_project_access_agent_granularity_start_end), [terms of use](https://www.mediawiki.org/wiki/REST_API#Terms_and_conditions), [license](https://www.gnu.org/licenses/fdl-1.3.html)) on dinosaur web-traffic. The three datasets constructed include:
      - dino_monthly_desktop_201506-202209.json
          - Desktop views of dinosaurs within dinosaurs.csv between 06/15-09/22
      - dino_monthly_mobile_201506-202209.json
          - Mobile views of dinosaurs within dinosaurs.csv between 06/15-09/22
      - dino_monthly_cumulative_201506-202209.json
          - Cumulative views of dinosaurs (monthly and mobile) between 06/15-09/22
          
      *Data Note 1:* Because the instructions state "For all of the data sets we are only interested in actual user pageview requests. The three resulting datasets should be saved as a JSON files ordered using article titles as a key for the resulting time series data." my resulting dataframes include each **article title** associated with their **user pageview requests**
      
      *Data Note 2:* I assumed article titles of a given MM/YY with **no** data to indicate total views of 0 for given dinosaur and MM/YY. This assumption is bolstered by none of the article-title and date datapoints containing 0 views. 
          
  2. Analyzing the constructed datasets through the following visualizations
      - Maximum Average and Minimum Average
          - Contains time series data for the articles that have the highest average page requests and the lowest average page requests for desktop access and mobile access. This graph havs four lines (max desktop, min desktop, max mobile, min mobile).
          - x-axis represents time-series in form of MM/YY
          - y-axis represents views
          - This visualization is saved as Maximum_Average_and_Minimum_Average.png
      - Top 10 Peak Page Views
          - Contains time series data for the top 10 article pages by largest (peak) page views over the entire time by access type. This graph contains the top 10 for desktop and top 10 for mobile access (20 lines).
          - x-axis represents time-series in form of MM/YY
          - y-axis represents views
          - This visualization is saved as Top_10_Peak_Page_Views.png
      - Fewest Months of Data
          - Visualizes pages that have the fewest months of available data. This graph shows the 10 articles with the fewest months of data for desktop access and the 10 articles with the fewest months of data for mobile access.
          - x-axis represents time-series in form of MM/YY
          - y-axis represents views
          - This visualization is saved as Fewest_Months_of_Data.png
