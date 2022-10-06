# data-512-homework_1
## Keegan Freeman
### 10/6/22

## Project Description

The goal of this project is to practice reproducibility and replicability good practices, as defined in [The Basic Reproducible Workflow Template]([https://link-url-here.org](http://www.practicereproducibleresearch.org/core-chapters/3-basic.html)) and [Assessing Reproducibility]([https://link-url-here.org](http://www.practicereproducibleresearch.org/core-chapters/2-assessment.html)), within a data-science format. The data-science tasks of this project include

  1. Pulling data from Wikipedia using the Pageviews API ([documentation](https://wikitech.wikimedia.org/wiki/Analytics/AQS/Pageviews)), [endpoint]((https://wikimedia.org/api/rest_v1/#!/Pageviews_data/get_metrics_pageviews_aggregate_project_access_agent_granularity_start_end),[terms of use](https://www.mediawiki.org/wiki/REST_API#Terms_and_conditions)) on dinosaur web-traffic. The three datasets constructed include:
      a. dino_monthly_desktop_201506-202209.json
      b. dino_monthly_mobile_201506-202209.json
      c. dino_monthly_cumulative_201506-202209.json
  2. Analyzing the constructed datasets through the following visualizations
      a. Maximum Average and Minimum Average
          - Contains time series data for the articles that have the highest average page requests and the lowest average page requests for desktop access and mobile access. This graph havs four lines (max desktop, min desktop, max mobile, min mobile).
      b. Top 10 Peak Page Views
          - Contains time series data for the top 10 article pages by largest (peak) page views over the entire time by access type. This graph contains the top 10 for desktop and top 10 for mobile access (20 lines).
      c. Fewest Months of Data
          - Visualizes pages that have the fewest months of available data. This graph shows the 10 articles with the fewest months of data for desktop access and the 10 articles with the fewest months of data for mobile access.
