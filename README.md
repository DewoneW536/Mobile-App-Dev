# Know Your Government

Know Your Government is a mobile application that allows for US citizens to get involved with their local political cabinet in a
way that is both user friendly and informative. The application was created as a final project for an Android Development course.


## Features Implemented:
- Implemented Google Civic APIs to update app with current list of Politicians via scrollable recyclerView, based on user location 
  or the zip code manually entered by user through the search bar.
- Executed Location Services and Internet Services to automatically request user location at startup, else default to MountainView, CA
  - In all activities, a location bar is shown that corresponds with user's local/requested city, state, or zip.
- Utilized the Picasso Image Library API to display available recent images of politicians via the Google Civic API, using URL 
  listed in the JSONArray for each government official the user taps/shows interest in.
- TextView Links are executed in Official Activity to take users to other applications based on information provided when pressed:
  - Address Link: Displays Politician's last known address and opens Google Maps with the address already located/displayed.
  - Phone Link: Provides the Official's listed phone number and pressing it will take users to native phone app to call said politician.
  - Website Link: Creates a link to the Politician's website, where the user can find out more about the politician shown in Official Activity.
- Background for Official Activity Corresponds to Politician's listed party allegiance:
  - If Democratic, background will be Colored Blue.
  - If Republican, Red.
  - Background Defaults to black if politician is non-partisan.
- ImageButtons are utilized as clickables for enhanced user experience; this includes allowing the user to learn more about the political parties
  and finding the listed social media accounts of all politicians via the Google Civic API (FaceBook, Twitter, YouTube,etc).
    - If a user already has the listed applications installed on their phone, the Know Your Government app will take user's straight to
      the application using the given username of requested politician.
    - If not, user will be taken to different social medias using Google Chrome.
