London Airbnb Listings
— Exploratory Data
Analysis
Exploratory data analysis of ~69,351
Airbnb listings across London, built in
Python within Jupyter Notebook.
🛠 Tech Stack
Python Pandas Matplotlib Jupyter
Notebook

📂 Dataset
69,351 rows × 18 columns
Columns include: id , name , host_id ,
host_name , neighbourhood ,
latitude , longitude , room_type ,

price , minimum_nights ,
number_of_reviews , last_review ,
reviews_per_month ,
calculated_host_listings_count ,
availability_365 ,
number_of_reviews_ltm
🧹 Data Cleaning
Dropped the empty

neighbourhood_group column (0 non-
null values)

Checked for missing values with
.isnull().sum() :
name : 5 missing
host_name : 5 missing
last_review /
reviews_per_month : 1,678
missing (listings with no reviews
yet)

Verified structure with .info() ,
.describe() , and .shape()
📊 Key Findings
Room type distribution
Room Type % of Listings
Entire home/apt 59.4%
Private room 39.6%
Shared room 0.6%
Hotel room 0.4%

Average price by room type
Room Type Avg. Price (£)
Hotel room 245.8
Entire home/apt 227.1
Private room 103.3

Room Type Avg. Price (£)
Shared room 66.2

Most expensive boroughs (avg. price)
1. Kensington and Chelsea — £302.9
2. Westminster — £297.0
3. City of London — £269.1
Most affordable boroughs (avg. price)
1. Croydon — £82.6
2. Sutton — £84.7
3. Bexley — £89.7
Highest listing volume by borough
1. Westminster — 7,763 listings
2. Tower Hamlets — 5,595 listings
3. Hackney — 5,168 listings
Price distribution
Right-skewed: most listings priced
under £200/night

Extreme outliers present (max
£25,000, min £0) — worth flagging for
further cleaning
Boxplot by room type confirms Hotel
room and Entire home/apt carry the
widest price ranges
📈 Visualizations
Bar chart — Room type distribution
Histogram — Price distribution (0–
£500 range)
Boxplot — Price distribution by room
type
Scatter plot — Geographic price
distribution across London (lat/long,
colored by price)
🔍 Next Steps
Investigate and handle price outliers
(e.g., £0 and £25,000 listings)

Add correlation analysis between
price and availability/review count
Build an interactive dashboard version
(Power BI/Tableau)

Part of a data analytics portfolio — see
more projects on GitHub.
