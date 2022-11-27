# Definition of the Output Datasets

<em>Obs.: Code available on notebooks</em>  

In this markdown, we will define the schema - with the data type, and names - for the output datasets.

We define as output one dataset per category, i.e., in the end, we will have: yellow taxi, green taxi, he, and fhvhv datasets.

Answering the question of the task:

<em>The input data is spread over several files, including separate files for “Yellow” and “Green” taxis. Does it make sense to merge those input files into one dataset?</em>

It is better to keep than separate, in order to preserve the schema for each dataset, even if they are very similar. To perform further analysis with both, a `join` operation could be applied.



## 1. Yellow Taxi Trip Records

Schema definition:

root

 |-- VendorID: integer (nullable = true)
 
 |-- tpep_pickup_datetime: timestamp (nullable = true)
 
 |-- tpep_dropoff_datetime: timestamp (nullable = true)
 
 |-- passenger_count: integer (nullable = true)
 
 |-- trip_distance: double (nullable = true)
 
 |-- RatecodeID: double (nullable = true)
 
 |-- store_and_fwd_flag: string (nullable = true)
 
 |-- PULocationID: long (nullable = true)
 
 |-- DOLocationID: long (nullable = true)
 
 |-- payment_type: integer (nullable = true)
 
 |-- fare_amount: double (nullable = true)
 
 |-- extra: double (nullable = true)
 
 |-- mta_tax: double (nullable = true)
 
 |-- tip_amount: double (nullable = true)
 
 |-- tolls_amount: double (nullable = true)
 
 |-- improvement_surcharge: double (nullable = true)
 
 |-- total_amount: double (nullable = true)
 
 |-- congestion_surcharge: double (nullable = true)
 
 |-- airport_fee: integer (nullable = true)
 
 |-- tpep_pickup_hour: integer (nullable = true)
 
 |-- tpep_dropoff_hour: integer (nullable = true)
 
 |-- pickup_day: string (nullable = true)
 
 |-- dropoff_day: string (nullable = true)



## 2. Green Taxi Trip Records

Schema definition:

root

 |-- VendorID: integer (nullable = true)
 
 |-- lpep_pickup_datetime: timestamp (nullable = true)
 
 |-- lpep_dropoff_datetime: timestamp (nullable = true)
 
 |-- store_and_fwd_flag: string (nullable = true)
 
 |-- RatecodeID: double (nullable = true)
 
 |-- PULocationID: long (nullable = true)
 
 |-- DOLocationID: long (nullable = true)
 
 |-- passenger_count: integer (nullable = true)
 
 |-- trip_distance: double (nullable = true)
 
 |-- fare_amount: double (nullable = true)
 
 |-- extra: double (nullable = true)
 
 |-- mta_tax: double (nullable = true)
 
 |-- tip_amount: double (nullable = true)
 
 |-- tolls_amount: double (nullable = true)
 
 |-- ehail_fee: integer (nullable = true)
 
 |-- improvement_surcharge: double (nullable = true)
 
 |-- total_amount: double (nullable = true)
 
 |-- payment_type: integer (nullable = true)
 
 |-- trip_type: integer (nullable = true)
 
 |-- congestion_surcharge: double (nullable = true)
 
 |-- lpep_pickup_hour: integer (nullable = true)
 
 |-- lpep_dropoff_hour: integer (nullable = true)
 
 |-- pickup_day: string (nullable = true)
 
 |-- dropoff_day: string (nullable = true)



## 3. For-Hire Vehicle Trip Records (FHV)

Schema definition:

root

 |-- dispatching_base_num: string (nullable = true)
 
 |-- pickup_datetime: timestamp (nullable = true)
 
 |-- dropOff_datetime: timestamp (nullable = true)
 
 |-- PUlocationID: double (nullable = true)
 
 |-- DOlocationID: double (nullable = true)
 
 |-- SR_Flag: integer (nullable = true)
 
 |-- Affiliated_base_number: string (nullable = true)
 
 |-- pickup_hour: integer (nullable = true)
 
 |-- dropOff_hour: integer (nullable = true)
 
 |-- pickup_day: string (nullable = true)
 
 |-- dropoff_day: string (nullable = true)



## 4. High Volume For-Hire Vehicle Trip Records (FHVHV)

Schema definition:

root

 |-- hvfhs_license_num: string (nullable = true)

 |-- dispatching_base_num: string (nullable = true)

 |-- originating_base_num: string (nullable = true)

 |-- request_datetime: timestamp (nullable = true)

 |-- on_scene_datetime: timestamp (nullable = true)

 |-- pickup_datetime: timestamp (nullable = true)

 |-- dropoff_datetime: timestamp (nullable = true)

 |-- PULocationID: long (nullable = true)

 |-- DOLocationID: long (nullable = true)
 
 |-- trip_miles: double (nullable = true)

 |-- trip_time: long (nullable = true)

 |-- base_passenger_fare: double (nullable = true)

 |-- tolls: double (nullable = true)

 |-- bcf: double (nullable = true)

 |-- sales_tax: double (nullable = true)

 |-- congestion_surcharge: double (nullable = true)

 |-- airport_fee: double (nullable = true)

 |-- tips: double (nullable = true)

 |-- driver_pay: double (nullable = true)

 |-- shared_request_flag: string (nullable = true)

 |-- shared_match_flag: string (nullable = true)

 |-- access_a_ride_flag: string (nullable = true)
 
 |-- wav_request_flag: string (nullable = true)
 
 |-- wav_match_flag: string (nullable = true)
 
 |-- pickup_hour: integer (nullable = true)
 
 |-- dropoff_hour: integer (nullable = true)
 
 |-- pickup_day: string (nullable = true)
 
 |-- dropoff_day: string (nullable = true)










