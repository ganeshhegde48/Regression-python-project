# Project Summary

In summary, the project aims to create a model that predicts the number of seats sold for each ride on specific routes, dates, and times for Mobiticket. The routes originate from 14 towns towards Lake Victoria, ending in Nairobi. The journey takes around 8 to 9 hours to reach the outskirts of Nairobi and an additional 2 to 3 hours to reach the main bus terminal. Passengers are influenced by traffic conditions during their travel into the city and onward to their final destinations in Nairobi. Understanding these patterns can help improve service planning and optimize operations for Mobiticket.

To enhance the performance of the model, additional features have been generated. These new features aim to provide more relevant information and contribute to improved predictions. The dataset has been subjected to testing using multiple regression models. These models have been employed to analyze the data and derive insights, allowing for a comprehensive evaluation of the predictive capabilities. The most significant features identified by the model are highlighted and displayed. These key features play a crucial role in determining the number of seats sold for each ride. By showcasing these important factors, stakeholders can gain a better understanding of the influential elements driving seat sales.

# Problem Description

This challenge asks you to build a model that predicts the number of seats that Mobiticket can expect to sell for each ride, i.e. for a specific route on a specific date and time. There are 14 routes in this dataset. All of the routes end in Nairobi and originate in towns to the North-West of Nairobi towards Lake Victoria.

The towns from which these routes originate are:

Awendo

Homa Bay

Kehancha

Kendu Bay

Keroka

Keumbu

Kijauri

Kisii

Mbita

Migori

Ndhiwa

Nyachenge

Oyugis

Rodi

Rongo

Sirare

Sori

The routes from these 14 origins to the first stop in the outskirts of Nairobi takes approximately 8 to 9 hours from time of departure. From the first stop in the outskirts of Nairobi into the main bus terminal, where most passengers get off, in Central Business District, takes another 2 to 3 hours depending on traffic.

Passengers of these bus (or shuttle) rides are affected by Nairobi traffic not only during their ride into the city, but from there they must continue their journey to their final destination in Nairobi wherever that may be. Traffic can act as a deterrent for those who have the option to avoid buses that arrive in Nairobi during peak traffic hours. On the other hand, traffic may be an indication for people’s movement patterns, reflecting business hours, cultural events, political events, and holidays.


# Data Description

Nairobi Transport Data.csv (zipped) is the dataset of tickets purchased from Mobiticket for the 14 routes from “up country” into Nairobi between 17 October 2017 and 20 April 2018. This dataset includes the variables: ride_id, seat_number, payment_method, payment_receipt, travel_date, travel_time, travel_from, travel_to, car_type, max_capacity.

Variables description:

ride_id: unique ID of a vehicle on a specific route on a specific day and time.

seat_number: seat assigned to ticket

payment_method: method used by customer to purchase ticket from Mobiticket (cash or Mpesa)

payment_receipt: unique id number for ticket purchased from Mobiticket

travel_date: date of ride departure. (MM/DD/YYYY)

travel_time: scheduled departure time of ride. Rides generally depart on time. (hh:mm)

travel_from: town from which ride originated

travel_to: destination of ride. All rides are to Nairobi.

car_type: vehicle type (shuttle or bus)

max_capacity: number of seats on the vehicle

# Conclusion

In this project, we have used different regression models to predict transport demand from various places to nairobi.

Using the data, we have created the target variable and several other features that contribute to our model performance.

We have used regression models including:

Linear Regression, Lasso (L1), Ridge (L2),XGBoost.

We have also performed hyperparameter tuning to improve the performance of these models.

Out of all these models, the hyperparameter tuned XGBoost gives the best result with an accuracy of around 88%
