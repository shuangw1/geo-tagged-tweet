# Geo-tagged tweet during covid-19 - what is the role of "park"?
### :hammer: Process
In this exercise, I used a python crawler to collected twitter data in American using key word ```park```. I would like to explore how people recreate and relax during this special time, it also helps us realize the importance of public green during this time.

Location are bounded to US, and time limit for this crawler is 60 seconds, and I got 36 tweets.
```Python
LOCATIONS = [-124.7771694, 24.520833, -66.947028, 49.384472,  # Contiguous US
             -164.639405, 58.806859, -144.152365, 71.76871,  # Alaska
             -160.161542, 18.776344, -154.641396, 22.878623]  # Hawaii
stream.filter(locations=LOCATIONS)
stream.filter(track=['park'])
```
![park](/assets/park.png)
Like a few other researchers may have found, twitts cluster in densely populated urban areas where there are more twitter users, and with more internet access (perhaps stable internet these days).

### :bulb: Findings
So what people say about ***park***?
- There are people saying about because of the lock down, it is a good way to get some vitamin D. While some others say it is a good day for a hike.
- But there are other irrelevant tweets, such as I am watching Jurrasic Park, or the name of the place is called Park city or Park avenue.
- In order to get more context based tweets, I may need to adjust the web crawler, or run the crawler for a longer time.
