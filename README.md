# **Exploratory Hotel Booking Analysis**

## **Abstract:**

Hotels keep information about their customers, like when the customer made the reservation and for how many members, the mode of payment, and much such relevant information to use to make the hotel stay experience better for future customers.

## **Introduction**
We are given with a data set containing information on hotel bookings for the years 2015, 2016, and 2017. Personal information of customers has been eliminated. Our aim is to analyse the data and answer the mentioned problems.

The given dataset has 119390 observations and 32 variables. Most of the variables are self-explanatory, the only two variables which require explanation are:

1. 	lead_time: The time between reservation of hotel and arriving at the hotel.

2. 	adr: adr stands for average daily rate of stay for a customer.

## **Null Value treatment**

Out of the 32 variables we have, we first keep our focus on a few of the relevant (to our problems) variables. Our focus will be on:

1. 	hotel

2. 	is_canceled

3. 	arrival_date_month

4. 	reserved_room_type

5. 	assigned_room_type

6. 	lead_time

7. 	Adr

8. Meal_type

9. Assigned_room_type/reserved_room type

10. Country

Now we analyse each of the variables.

First import the dataset as df, then analyse each column using the syntax

df[‘variable_name’]. describe( )

to find that all of these variables have zero null values, so we don’t have to fill or remove the Null values.

However, on exploring the variable ‘adr’ we see that the minimum value is negative but, the average daily rate cannot be negative. So, we change the negative adr value 0.

On plotting the boxplot for adr we also see that one value is way out of the range of outliers.  While one value is 5400 and the rest is in between range of 0 to 500. We remove this observation.

Further, we plot the boxplot for all the numerical columns and see that some of the columns have a lot of outliers. So, we make some required changes.

## **Problem statement:**

The data provided to us is vast and contains plenty of information but we focus only on the columns which can give us some relevant and useful information, from both customer and business points of view.

### **Percentage of booking in each hotel type**

This will give us insight into which hotel sees more cancellations so the management can make decisions according to the type of hotel.

### **From which country do most guests come.**

This can give the management information to make changes in the hotels for the customers from some particular country. For example, employing more staff familiar with the language of the most visited country can give the customers a better experience.

### **Which is the busiest month.**

This will help the employees to hire extra staff during which of the months.

### **Which room is most in demand, which is the most expensive room, and which room type generates most of the revenue?**

So that the management can make decisions on whether to decrease or increase the number of any type of room.

### **Most famous meal type?**

So that the management can give more options for that specific meal type.

### **How many cancelations do we see because of not getting the same room and which months does it peak? Furthermore, if a customer does not get the desired room then do they pay less money?**

This will give the management an idea of what room numbers should be increased and which months they need to increase a particular room type.

### **How average_adr, No. of bookings, average waiting time, and average lead_time varies monthly.**

This will give information on the monthly performance of the hotel in terms of revenue and other factors regarding reservations.

### **How cancellation varies with lead time and how many days to people usually stay in the hotel. What distribution channel through which do we get most of our customers, what customer type book and cancel the most.**

Such data will give the management insights into the behaviour of customers depending on the mentioned factors.

We use groupby and a lot of visualization to understand these.


### **Conclusion:**

That’s it, we have evaluated the data and performed analysis on various variables, and obtained plenty of information that can be used by the management to improve the business. Moreover, obtained observation can be used by the customers to get the best price on hotels.

