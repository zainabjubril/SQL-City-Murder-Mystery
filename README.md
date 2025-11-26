# SQL City Murder Mystery

## Table of Contents 
- [Installation and setup](#installation-and-setup)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Codes and packages](#codes-and-packages)
- [Credits](#credits)
- [License](#license)

## Project Overview

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


# Installation and setup

We start by importing python packages such as: numpy and pandas

<img width="596" height="71" alt="Screenshot 2025-11-21 at 00 48 11" src="https://github.com/user-attachments/assets/633e56fc-3503-4ab0-8be8-45016984f924" />

- Now let us view the layout of the first table which could enable us get leads to solve this case

<img width="599" height="125" alt="Screenshot 2025-11-21 at 13 08 52" src="https://github.com/user-attachments/assets/97b8576e-47e7-4797-a63a-8d5859dba1d8" />

-This is the result:

<img width="529" height="256" alt="Screenshot 2025-11-21 at 12 49 06" src="https://github.com/user-attachments/assets/233466b1-ae1f-4b9b-a1e5-920937e929f0" />


  - Since we are interested in SQL City in this case, we will filter out the table to return information about SQL City only.

<img width="600" height="199" alt="Screenshot 2025-11-21 at 13 10 29" src="https://github.com/user-attachments/assets/0de39336-0ec0-48cd-a627-cf00cb0f1157" />


<img width="698" height="392" alt="Screenshot 2025-11-21 at 13 04 55" src="https://github.com/user-attachments/assets/fc79d2d0-bf70-46b4-8960-72e92c34017e" />


# Exploratory Data Analysis


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


- Let us view the layout of the Get Fit Now Member table.


<img width="598" height="126" alt="Screenshot 2025-11-21 at 14 50 08" src="https://github.com/user-attachments/assets/3567a488-63ed-4c19-8b3d-9c08c4f5e1d6" />

<img width="531" height="133" alt="Screenshot 2025-11-21 at 15 05 36" src="https://github.com/user-attachments/assets/b573b846-4ae0-41c4-b1ae-641ee79db37f" />


- Since we know that the membership id of the suspect starts with "48Z", we can check for members whose membership ids start with 48Z and have a gold membership status.

<img width="606" height="139" alt="Screenshot 2025-11-21 at 15 10 33" src="https://github.com/user-attachments/assets/efdc4144-370a-4f09-a042-bb23408cf4ef" />

<img width="504" height="67" alt="Screenshot 2025-11-21 at 15 12 00" src="https://github.com/user-attachments/assets/2e329bd7-2ea1-45fc-b721-f5a858eb8df8" />


- We have two leads; Joe Germuska and Jeremy Bowers. so now we need to find out which of them checked in at the gym on January 9.


<img width="605" height="141" alt="Screenshot 2025-11-21 at 15 18 27" src="https://github.com/user-attachments/assets/0ce8e653-eb76-46d9-abc9-257cfb4956d0" />


<img width="526" height="135" alt="Screenshot 2025-11-21 at 14 51 07" src="https://github.com/user-attachments/assets/00922340-752b-4a91-b62a-d81ce4ccea2b" />


OOPS! Both suspects checked-in on the 9th of January!

So, since we have another information about the suspect, being his plate number, let us find out which of the suspects have a plate number that has the characters: 'H42W'


<img width="600" height="124" alt="Screenshot 2025-11-21 at 23 01 21" src="https://github.com/user-attachments/assets/6c0c3c1c-ff68-4620-890b-968ec316e7e4" />


<img width="585" height="66" alt="Screenshot 2025-11-21 at 23 12 17" src="https://github.com/user-attachments/assets/5c70e45f-3edd-4db9-8510-ea54363747b9" />


- We have the information, including the license ids of two men who have a plate number that have the characters, 'H42W'

- Now we need to check if either of those two licence ids belong to either Joe or Jeremy.


<img width="697" height="164" alt="Screenshot 2025-11-21 at 23 25 00" src="https://github.com/user-attachments/assets/d6d54e2b-b4ca-4a12-abb1-cb2bcb2f50c1" />


<img width="561" height="43" alt="Screenshot 2025-11-21 at 23 26 30" src="https://github.com/user-attachments/assets/1a47e1c9-616c-411d-9da0-bd0470d6281f" />


Finally! A main lead! Jeremy Bowers! Now let us view his interview transcript...


<img width="603" height="136" alt="Screenshot 2025-11-21 at 23 38 58" src="https://github.com/user-attachments/assets/c12ce8fb-67d5-438f-86b2-dbf1883edd29" />


<img width="699" height="71" alt="Screenshot 2025-11-21 at 23 39 51" src="https://github.com/user-attachments/assets/949afb65-7c3a-4355-b4ff-c41a85f0d148" />



- Now we have to look for the woman who hired Jeremy and we have the following information about her:

1. Her height: either 65" or 67"
2. Hair color: red
3. Car Model: Tesla, Model S
4. Her activities in December 2017: attended 3 SQL Symphony Concerts


- Let us get the suspect's ID using the Drivers License table.


<img width="719" height="187" alt="Screenshot 2025-11-21 at 23 46 55" src="https://github.com/user-attachments/assets/09cc9435-ed95-4cb6-accc-80fcb638457c" />


<img width="590" height="89" alt="Screenshot 2025-11-21 at 23 48 01" src="https://github.com/user-attachments/assets/4ff7fe32-73d3-48a2-ba52-8f43356d160b" />


We have 3 possible suspects and they all fit the description, as their heights are between 65 and 66"


Now, we need to get the names of all 3 suspects, using their license IDs


<img width="671" height="165" alt="Screenshot 2025-11-21 at 23 50 18" src="https://github.com/user-attachments/assets/e727239e-497b-45c5-b7e1-cbfb6ed03f18" />


<img width="558" height="88" alt="Screenshot 2025-11-21 at 23 51 11" src="https://github.com/user-attachments/assets/a96a65d0-236e-49af-9d02-a8ca1a0f732f" />


- Next, we will check which of the 3 suspects attended the SQL Symphony Concert in December 2017.


<img width="717" height="186" alt="Screenshot 2025-11-21 at 23 55 13" src="https://github.com/user-attachments/assets/4f9a89d0-3944-4129-8455-7a9295bdf0d5" />


<img width="363" height="88" alt="Screenshot 2025-11-21 at 23 57 13" src="https://github.com/user-attachments/assets/9cf31309-adae-4df1-943b-b3ea6b6ae584" />


- We have our culprit! The suspect with the id number-99716, who happens to be Miranda Priestly, attended the SQL Symphony Concert thrice in December 2017, which fits the information given by Jeremy Bowers!!

Now for the final stage, let us get her address and make the arrest!


<img width="595" height="138" alt="Screenshot 2025-11-22 at 00 03 09" src="https://github.com/user-attachments/assets/6fbb25ce-529f-4a3e-be13-b54feb6b74c9" />


<img width="600" height="127" alt="Screenshot 2025-11-22 at 00 08 30" src="https://github.com/user-attachments/assets/136f8f47-0ee9-4e8c-9042-20fa33a27e75" />


<img width="560" height="42" alt="Screenshot 2025-11-22 at 00 09 28" src="https://github.com/user-attachments/assets/57e9318e-1d57-4f27-ba23-64d51e2e6684" />


## Codes and packages

- SQL(sqlite3)
- Python(NumPy, Pandas)


## Credits
The SQL Murder Mystery was created by Joon Park and Cathy He while they were Knight Lab fellows. See the GitHub repository for more information. Adapted and produced for the web by Joe Germuska. This mystery was inspired by a crime in the neighboring Terminal City. Web-based SQL is made possible by SQL.js SQL query custom web components created and released to the public domain by Zi Chong Kao, creator of Select Star SQL. Detective illustration courtesy of Vectors by Vecteezy Original code for this project is released under the MIT License Original text and other content for this project is released under Creative Commons CC BY-SA 4.0

## License 
MIT License



# THANK YOU FOR SOLVING THE SQL CITY MURDER MYSTERY CASE WITH ME!!
