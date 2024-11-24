## YourCabs
### YourCabs Capstone project

The business problem tackled here is trying to improve customer service for YourCabs.com, a cab company in Bangalore. The problem of interest is booking cancellations by the company due to unavailability of a car. The challenge is that cancellations can occur very close to the trip start time,thereby causing passengers inconvenience.

#### Objective
The goal of the competition is to create a predictive model for classifying new bookings as to whether they will eventually gets cancelled due to car unavailability



#### The dataset contains details of booking records with the following columns:

| **Column Name**        | **Description**                                                                                     |
|-------------------------|-----------------------------------------------------------------------------------------------------|
| `id`                   | Booking ID                                                                                         |
| `user_id`              | Unique ID of the customer (based on mobile number)                                                 |
| `vehicle_model_id`     | Type of vehicle model                                                                              |
| `package_id`           | Type of package:<br>1 = 4 hrs & 40 kms<br>2 = 8 hrs & 80 kms<br>3 = 6 hrs & 60 kms<br>4 = 10 hrs & 100 kms<br>5 = 5 hrs & 50 kms<br>6 = 3 hrs & 30 kms<br>7 = 12 hrs & 120 kms |
| `travel_type_id`       | Type of travel:<br>1 = Long distance<br>2 = Point-to-point<br>3 = Hourly rental                     |
| `from_area_id`         | Unique identifier of the area (applicable for point-to-point travel and packages)                  |
| `to_area_id`           | Unique identifier of the destination area (applicable for point-to-point travel)                   |
| `from_city_id`         | Unique identifier of the departure city                                                            |
| `to_city_id`           | Unique identifier of the destination city (only for intercity travel)                              |
| `from_date`            | Timestamp of the requested trip start                                                              |
| `online_booking`       | Indicates if the booking was made via the desktop website (1 = Yes, 0 = No)                        |
| `mobile_site_booking`  | Indicates if the booking was made via the mobile website (1 = Yes, 0 = No)                         |
| `booking_created`      | Timestamp of when the booking was created                                                          |
| `from_lat`             | Latitude of the departure area                                                                     |
| `from_long`            | Longitude of the departure area                                                                    |
| `to_lat`               | Latitude of the destination area                                                                   |
| `to_long`              | Longitude of the destination area                                                                  |
| `Car_Cancellation`     | Indicates if the booking was cancelled due to unavailability of a car (1 = Cancelled, 0 = Not Cancelled) |



Here’s a well-structured version for the **Solution** section in your GitHub README:

---

## Solution

In this project, **Exploratory Data Analysis (EDA)** was conducted on the entire dataset to gain insights and identify patterns. Based on the `travel_type_id`, the dataset was categorized into three subsets, as different `travel_type_id` values correspond to unique workflows.

Since this is a classification problem, the following classification algorithms were applied to each dataset:

- **Logistic Regression**  
- **Decision Tree**  
- **Random Forest**  
- **AdaBoost**  

The final prediction was made using the model that demonstrated the highest accuracy, along with good precision and recall scores, ensuring a robust and reliable solution.  

