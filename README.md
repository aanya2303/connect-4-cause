# connect-4-cause

## Inspiration
We have realized through the years that there is a gap in the volunteering space. NGOs are constantly hunting for volunteers, and volunteers are constantly hunting for organizations to help out. So, we decided to build a web app that connects the two!

## What it does
<Connect_4_Cause/> is a web app that connects NGOs and volunteers. It allows for registration of both the types of accounts and asks for some basic info such as the time commitment, work interests, and location. On the main search page, it provides 3 options to search: by location, interests, and time commitment.

## How we built it
We built the web app on the Google Firebase platform. It uses the Cloud Firestore as the back-end database and Firebase hosting to host the site on the internet. On the front-end, we used the standard HTML, CSS, JavaScript framework. The search-by-location uses a combination of the Google Maps API and Radar.io to convert US zip codes to LatLng values, and subsequently sort entries by how far they are from the user using the Radar.getDistance() function.

## Challenges we ran into
The biggest challenge we ran into at the very end (that we weren't able to fix) was a tiny bug with variable scope in the Radar.getDistance() function. After our Google Maps API worked correctly, and the Radar.io API also gave correct responses to test values, we faced trouble with the scope of a few LatLng variables. Due to this bug, our location search didn't end up working.

## Accomplishments that we're proud of
We are most proud of our Firebase and Google Cloud integration. It was a massive task in getting those to work with the front-end and writing the Firestore queries.

## What we learned
We learned a lot through the process. We believe the Google Cloud integration was one key takeaway. API integration is a very important skill and we did that over and over again through the project.

## What's next for <Connect_4_Cause/>
Now, the project needs a whole bunch of users! We are planning to promote the project starting in our own community and get people on the platform. We also have plans to scale it up with more features like in-depth searching and addition of more profile options.
