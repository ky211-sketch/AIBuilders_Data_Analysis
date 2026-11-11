Project Overview:
 
This project is an Exploratory Data Analysis on Hotel Bookings Dataset, to apply learned knowlegde about exploring, cleanind and visualizing data.


About the Dataset: 
The dataset "hotel_bookings.csv" 
it has 4 columns with missing data (one is ~94% empty!), ~32,000 duplicate rows, dates stored as text, and some physically impossible values. 
Key columns:

hotel :Resort Hotel or City Hotel
is_canceled	1 = booking was cancelled, 0 = not
lead_time: Days between booking and arrival
arrival_date_month:	Month of arrival (text, e.g. "July")
adults / children / babies:	Number of guests of each type
meal, country, market_segment, customer_type :Categorical descriptors
adr: Average Daily Rate (price per night)
agent / company: IDs of the booking agent / company (lots of missing)
reservation_status_date: Date of the last status change (text)


Libraries:
pandas 
numpy 
matplotlib

EDA Workflow:

1. Exploring / diagnosing the data
2. Cleaning — missing values, duplicates, wrong data types, invalid values
3. Visualizing with matplotlib
4. Manipulating — sorting, filtering, new columns, `groupby`, `pivot_table`, `crosstab`
5. Drawing conclusions.

Conclusion:
After this detailed Exploratory Data Analysis and result visualization, we can conclude that: 
- cancellation rate changes according different factors (the city hotel has a higher cancellation than resort hotel, maybe we should study the time btw booking and arrival in each hotel type to estimate or better understand possible reasons of cancelling)
- bookings before a lomg time lead to a higher cancellation rate, while booking in the same day or few days before are less canceled.
- usually new guest cancels booking more than an old guest  (repeated guest becomes as a loyal customer or guest)


