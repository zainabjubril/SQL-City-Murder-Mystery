# SQL City Murder Mystery

## Table of Contents 

## Introduction

We have a mission to solve the SQL Murder Mystery case!

The database has 9 tables,namely;

1. crime_scene_report
2. drivers_license
3. person
4. facebook_event_checkin
5. interview
6. get_fit_now_member
7. get_fit_now_check_in
8. income
9. solution


# Data Cleaning & Preparation

We start by importing python packages such as: numpy and pandas

<img width="596" height="71" alt="Screenshot 2025-11-21 at 00 48 11" src="https://github.com/user-attachments/assets/633e56fc-3503-4ab0-8be8-45016984f924" />

- Now let us view the layout of the first table which could enable us get leads to solve this case

<img width="599" height="125" alt="Screenshot 2025-11-21 at 13 08 52" src="https://github.com/user-attachments/assets/97b8576e-47e7-4797-a63a-8d5859dba1d8" />

-This is the result:

<img width="529" height="256" alt="Screenshot 2025-11-21 at 12 49 06" src="https://github.com/user-attachments/assets/233466b1-ae1f-4b9b-a1e5-920937e929f0" />


  - Since we are interested in SQL City in this case, we will filter out the table to return information about SQL City only.

<img width="600" height="199" alt="Screenshot 2025-11-21 at 13 10 29" src="https://github.com/user-attachments/assets/0de39336-0ec0-48cd-a627-cf00cb0f1157" />


<img width="698" height="392" alt="Screenshot 2025-11-21 at 13 04 55" src="https://github.com/user-attachments/assets/fc79d2d0-bf70-46b4-8960-72e92c34017e" />


- From the table, we have been able to gather a lead which shows that there were two witnesses at the murder scene in SQL city, now let us find these witnesses!

<img width="598" height="167" alt="Screenshot 2025-11-21 at 13 16 59" src="https://github.com/user-attachments/assets/8286e364-e75b-44a3-b54c-f702222d9632" />


<img width="547" height="41" alt="Screenshot 2025-11-21 at 13 19 26" src="https://github.com/user-attachments/assets/4b6651a6-a54b-48a4-8e5f-4dfb6d632823" />

- The first witness has been identified as: Morty Schapiro. Now let us find the second witness.

<img width="605" height="127" alt="Screenshot 2025-11-21 at 13 28 00" src="https://github.com/user-attachments/assets/6b152738-14cf-48f4-8ab0-b23e5d41a632" />

<img width="548" height="44" alt="Screenshot 2025-11-21 at 13 29 13" src="https://github.com/user-attachments/assets/16ee198d-935b-4174-be16-122a111a653b" />

- The Second witness is: Annabel Miller.


<img width="602" height="130" alt="Screenshot 2025-11-21 at 14 37 09" src="https://github.com/user-attachments/assets/95e5eaf3-7257-4196-8022-e18574efdc44" />



<img width="701" height="105" alt="Screenshot 2025-11-21 at 14 38 01" src="https://github.com/user-attachments/assets/bed4caec-4490-4805-ab24-babd88e7045b" />


- From the witness interviews, we got the following information:


1. The killer had a 'Get Fit Now Gym' bag, and the membership number on the bag started with '48Z'
2. We also know the membership status of the suspect or of the owner of the bag he was carrying.
3. The license plate number of his car also had the characters, "H42W"
4. The second witness confirmed the killer is indeed a gym member and checked in at the gym on January 9.



