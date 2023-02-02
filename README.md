# Hotel Bookings Exploratory Data Analysis

## Objective
This project aims to perform exploratory data analysis (EDA) on a dataset of hotel bookings. The objective is to gain insights into various aspects of hotel bookings, such as the busiest seasons, the most prefered room type,meal type,number of guests,how long the stay was,market segment distribution,deposite type,required parking space,highest year of booking , and the factors that influence booking cancellations.

## Dataset
A dataset containing 119390 records across 32 features has been given with information regarding bookings of two hotels from July 2015 to August 2017. These two hotels are City Hotel and Resort Hotel.

The main objective is to explore the given dataset and discover the factors which govern the bookings. The dataset will be analyzed and from the conclusions drawn from it will be used to recognize the missteps taken by the manager. With this information, hotels will be equipped to improve their performance.

Data analysis is performed to answer the following questions:

Which hotel is more preferred among travelers?

Which hotel retains more customers?

Which is the busiest month?

Which is the most popular room type?

From which country the greatest number of bookings were made?

How Long People Stay in the hotel?

How many bookings were cancelled?

Prefered meal types of guest

which hotel makes more revenue

## Files

The project consists of the following files:

hotel_bookings.csv: https://drive.google.com/file/d/1x2Zk8X_mkBKic-FEne6QqkhXs_eLis9N/view?usp=share_link

hotel_bookings_eda.ipynb: https://colab.research.google.com/drive/10colv_bVvoO3Qt3AhD7RsiFgLra8eBt2?usp=share_link

README.md: this file

## Data cleaning 
### (1) Removing Duplicate rows
All duplicate rows were dropped.

### (2) Handling null values
-As the country and children columns having minimal pertage of missing value we replace their value by other and zero for country and children respectively
  

### (3) Converting columns to appropriate data types

converted the datatypes arrival date year,month and day to string and after combaning them into a date structer have changed the dtatype of combination from string to datetime.

### (4) Creating new columns
- Created new column `total_stay` by adding `stays_in_weekend_nights`+`stays_in_week_nights`.
- Created new column `total_members` by adding `adults`+`children`+`babies`.

## Requirements
The following libraries are required to run the code in this project:

pandas
numpy
matplotlib
seaborn

```

Mainly performed using Matplotlib and Seaborn library and the following graph and plots had been used:
  -  Bar Plot.
  -  Histogram.
   - Scatter Plot.
   - Pie Chart.
   - Line Plot.
   - Heatmap.
- Box Plot
            
```

## Conclusion

The hotel booking analysis project has provided valuable insights into customer behavior and the factors that influence booking decisions. Through the exploration of booking data, the project has identified key trends, patterns, and relationships that can be used to improve the hotel's booking process and customer satisfaction. The insights in this project, such as:
1. City Hotel seems to be more preferred among travellers and it also generates more revenue & profit.

2. Most number of bookings are made in July and August as compared rest of the months.

3. Room Type A is the most preferred room type among travellers.

4. Most number of bookings are made from Portugal & Great Britain.

5. Most of the guest stays for 1-4 days in the hotels.Most common stay length is less than 4 days and generally people prefer City hotel for short stay, but for long stays, Resort Hotel is preferred

6. City Hotel retains more number of guests.

7. Around one-fourth of the total bookings gets cancelled. More cancellations are from City Hotel.41.7% of the total bookings were cancelled for City hotel and 21.7% for the Resort hotel.

8. New guest tends to cancel bookings more than repeated customers.

9. Number of days that elapsed between the entering date of the booking and the arrival date is less for the people who cancelled.

10. As the hotels are in Portugal Europe, the bookings are mostly with European countries, Highest is Portugal with 48.59k bookings.

11. Only 3% are repeated guests.

12. 77% of the bookings are made with bed and breakfast.

13. Transite type custemers having most of the bookings

14. As expected , Most Bookings are done with 'No deposite' and most cancellations are also in 'no deposit' bookings. It is a surprise to see cancellations with 'Non-refundable' bookings.

15. Bookings for city hotels are higher than resort hotels over the years and in year 2016 the bookings for both the hotels were maximum.

Overall, this project demonstrates the importance of data-driven decision making in the hospitality industry. By using data to understand customer behavior and identify key trends, hotels can make informed decisions that improve their business performance and meet the needs of their customers. The insights gained from this project provide a solid foundation for the hotel to continue improving its booking process and customer satisfaction in the future.

## Challenges
(1) There was a lot of duplicate data.

(2) Data was present in wrong datatype format.

(3) Choosing appropriate visualization techniques to use was difficult.

(4) A lot of null values were there in the dataset.


