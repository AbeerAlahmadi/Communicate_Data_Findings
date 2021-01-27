
# US Commericial Flights


## Dataset
- The dataset Name is Flights(From Udacity)
- Source - https://www.transtats.bts.gov/Fields.asp?Table_ID=236
- The dataset contains 36 Feartures. Description all the features is mentioned below -

1. Year - Year of Data record
2. Quarter - Contains values from 1-4
3. Day-of-week - 1(Monday) to 7(Sunday)
4. DepTime - actual departure time (local, hhmm)
5. ArrTime - actual arrival time (local, hhmm)
6. Flights - Number of Flights
7. Distance - Distance between airports (miles)
8. DestAirportID,OriginAirportID - Destination and Origin Airport, Airport ID. An identification number assigned by US DOT to identify a unique airport.
9. DestAirportSeqID,OriginAiportID - Destination and Origin Airport, Airport Sequence ID. An identification number assigned by US DOT to identify a unique airport.
10. DestCityMarketID - Destination Airport, City Market ID. City Market ID is an identification number assigned by US DOT to identify a city market.
11. Dest,Origin - Destination Airport and Origin Airport
12. DestCityName, OriginCityName - Destination Airport and Origin Airport, City Name
13. Cancelled - was the flight cancelled?
14. CancellationCode - reason for cancellation (A = carrier, B = weather, C = NAS, D = security)
15. CarrierDelay - in minutes
16. LateAircraftDelay - in minutes
17. SecurityDelay - in minutes
18. NASDelay - in minutes
19. WeatherDelay - in minutes
20. ArrDelay - Difference in minutes between scheduled and actual arrival time. Early arrivals show negative numbers.
21. DepDelay - Difference in minutes between scheduled and actual departure time. Early departures show negative numbers.

*Created Features from dataset*
1. time - Divided the DepartureTime(hh.mm) in to 5 categories named(Morning, Early-morning, Noon, Night, Late-Night)
2. distance - Distance Between two states has been categorized in to 5 section(0-500,500-1k,1k-2k,....)



## Summary of Findings
- The data consists of flight arrival and departure details for all commercial flights within the USA and contains around 607K records. 
- The data record contains data from January 2020, Quarter-1.

*Flights*
- Highest number of flights is from Day 5(Friday) and 4(Thursday) which is 35% of the data .
- Lowest numer of flights is from Day 6(Saturday) which is 10% of overall records.
- Maximum Flights got cancelled on 5th(friday) and 6th(saturday) day. It's obious that the max number of flights is from friday so max number of flight cancelled can be from that day too.

*Most Frequent Flights* 
- Flight from New York(NY) and Chicago(IL) is the most frerquent flight.
- Maximum 250 flights a day has been recorded between these cities.

* How often do flights got cancelled?
- 7K flights got cancelled from 600K records which is only 1.1% of total records

* Reason Behind flight cancelled!
- Mostly due to weather ⛈
- Two Flights got cancelled due to security reason, I am very curious to know what could be the issue? 🤔 but unfortunately we dont have that type of records.

* Number of late nights flights are very few whereas number of Morning and late mornings flights are almost 60% of total flights.

* Distance between origin and destination
- The shortest Distant flight is of 31 Miles between Wrangell,AK and Pestersburg,AK.
- The largest Distnace flight if 5095 Miles between Honolulu, HI Boston, MA.

* which states has Max number of flight a day?
- Flight from New York(NY) and Chicago(IL) has max number of flights followed by Boston(MA).



## Key Insights for Presentation
one of the key thread from exploration is flight delay delay.

* Have you ever been stuck in an airport because your flight was delayed or cancelled and wondered if you could have predicted it if you'd had more data? This is your chance to find out.
- Maximum number of arrival and departer deplay is 2500 Minutes(That's a huge number, right!).
- Many flights arrives/departes early and maximum early departure time is 60 minutes. 
- Sometimes, some flights cover more distance in less time which results in to early arrival of flight. Thus some flights got depated on-time but arrived early than expected.
- Carrier and Late flight delays are main reasons behind all greater delays. Weather delays are very small compared to them.
- Security delays are tend to 0 which shows that there's rare 1 or 2 security delay.

* When is the best time of day of week/time of year to fly to minimise delays?
- Wednesday has least delay of all days.
- Noon time which is between 4-7 PM has lowest delay time.
- Whereas maximum delays are during mornings.

*Patterns from line and box plots*
- Carrier delays occurs most frequently where as weather delays are rare.
- The straight upline at the end of every graph indicates that Higher delays are rare in any category of delays.
- As carrier delay has smooth curve at the end which shows carrier delays has highest number of longer delays.
