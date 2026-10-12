# MySQL-Queries-
•	SQL queries: 
•	SELECT truck_id,status
•	FROM Trucks
•	WHERE status = 'Active'
•	
•	SELECT driver_id,first_name,last_name,hire_date,date_of_birth,home_terminal,employment_status,years_experience
•	FROM Drivers
•	
•	SELECT COUNT(driver_id) as 'Total driver ID'
•	FROM Drivers
•	
•	SELECT load_id,customer_id,route_id,load_type,revenue,fuel_surcharge,accessorial_charges,load_status,booking_type
•	FROM loads
•	
•	SELECT AVG(revenue) as 'Avg Revenue'
•	FROM loads
•	
•	SELECT*
•	FROM Customers
•	
•	SELECT customer_type,account_status
•	FROM Customers
•	WHERE customer_type = 'Dedicated'
•	
•	SELECT customer_type,account_status
•	FROM Customers
•	WHERE customer_type = 'Contract'
•	
•	SELECT customer_type,account_status
•	FROM Customers
•	WHERE customer_type = 'spot'
•	
•	SELECT Top 10 load_id
•	FROM loads
•	ORDER BY (load_date) DESC
•	
•	SELECT incident_id,trip_id,truck_id,driver_id,incident_type,location_city,claim_amount,preventable_flag
•	FROM [Safety incidents]
•	
•	SELECT COUNT (preventable_flag)
•	FROM [Safety incidents]
•	WHERE preventable_flag = '1'
•	
•	SELECT SUM (claim_amount) as 'Total Claim'
•	FROM [Safety incidents]
•	
•	SELECT maintenance_id,truck_id,maintenance_type,total_cost,facility_location,downtime_hours
•	FROM [Maintenance records]
•	
•	SELECT AVG (downtime_hours)
•	FROM [Maintenance records]
•	
•	SELECT driver_id
•	FROM Drivers
•	WHERE years_experience >10
•	
•	SELECT COUNT (load_type)
•	FROM loads
•	
•	SELECT SUM (revenue+fuel_surcharge+accessorial_charges) as 'Total Revenue'
•	FROM loads
•	
•	SELECT event_id,load_id,trip_id,event_type,facility_id,actual_datetime,detention_minutes,on_time_flag,location_city
•	FROM [Delivery events]
•	WHERE event_type = 'Delivery'
•	
•	SELECT event_id,load_id,trip_id,event_type,facility_id,actual_datetime,detention_minutes,on_time_flag,location_city
•	FROM [Delivery events]
•	WHERE event_type = 'Pickup'
•	
•	SELECT AVG (CAST(on_time_flag AS decimal(5,2)))*100 as 'OnTime Delivery %'
•	FROM [Delivery events]
•	
•	SELECT Top 10 driver_id,claim_amount
•	FROM [Safety incidents]
•	ORDER BY 'claim_amount' DESC
•	
•	SELECT SUM (claim_amount)
•	FROM [Safety incidents]

