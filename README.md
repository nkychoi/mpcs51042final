# Natalie's MPCS 51042 Final Project Repository

# Week 3: Final Project Proposal:
## My API will help people plan vacations following specific budget, destination, and safety restraints. I've labeled each method I proposed so I can follow along in the to-do timeline. It will have methods to simplify and streamline vacation planning by creating a central, personalized information hub for travelers:
(1) Return potential destinations within a specific set of budget constraints
  - This will take the user’s budget preferences set on a range, as well as the ‘style’ of vacation (city, beach, outdoors) and return potential destinations based on deals on the web like Kayak, Priceline, Skyscanner.

(2) Provide weather forecasts for the selected destination
  - Passing the destination and travel dates, this method will use a weather API to provide weather forecasts

(3) Draft an itinerary of activities suggested at the destination for the user based on the user’s preferences
  - This method will take the destination and the user’s vacation preferences (typical activities they enjoy on vacation) to suggest tourist activities and locations (restaurants, walking tours, cultural monuments, museums) based on online review guides like Yelp, Booking.com, and TripAdvisor

(4) Integrate the proposed itinerary with the user’s Google Calendar
  - Passing the drafted itinerary, my API will generate events for each activity to block time on the calendar using the Google Calendar API

(5) Create a packing list personalized for the user and destination
  - Based on the activities and weather, this will generate a personalized packing list for the user

(6) Return top safety tips (neighborhoods to avoid) and vaccine/medication recommendations for the destination	
  - This method will provide news and health and safety information about the destination by querying news APIs and the CDC’s APIs

# Week 4: Approved Final Project Proposal To-Do List: VacAyPI
## Here's my proposed plan for timing on my final project, VacAyPI
* By Week 4/5:
  - Create a project repository.
  - Set up virtual environment and install required libraries.
  - Finish and push my README with proposed timeline and final approval from TA's and Prof. Troy.
  - Method (1): Research publicly available APIs (Kayak, Priceline, Skyscanner) to fetch travel deals. Implement a method that takes budget, style of vacation, and dates as inputs and returns a list of destinations within the budget range. Error handling for API requests will be conducted (implied as a part of refining each method in my to-do list).

    
* By Week 6:
  - Method (2): Select and integrate a weather API, and build a method that takes the Method (1) selected destination and travel dates as input, and returns the forecast for the suggested dates.
  - Method (2) Refinement: This method will also have a functionality to handle multiple destinations selected as the output of Method (1) in one request.
  - Method (3): Research publicly available APIs for activity recommendations (Yelp, Booking.com, TripAdvisor), and build a method that takes the user preferences (e.g., museums, dining, activity-level) and destination to return activity suggestions.
  - Method (3) Refinement: This method should also have a filtering component that's capable of allowing users to exclude activities based on preferences like party size, handicap/ADA compliance, etc.
    
* By Week 7:
  - Method (4): Integrate my API with the Google Calendar API, so that this method is able to take Method (3) results (itinerary events) into calendar events.
  - Method (5): This method should take in the travel dates, results from Method (2) Weather, and Method (3) Itinerary, to output a proposed packing list.
  - Method (5) Refinement: Question for Prof. Troy/TA's: Is this too ambitious? I'm kind of pulling at straws here, I'm worried, that this actually wouldn't be very helpful because it's not like I'm integrating this with some sort of fashion (?) API... If I do do this, I'd like users to also be able to personalize the final list by going through articles of clothing in the initial output and manually removing/adding from the packing list.
  
* By Week 8:
  - Method (6): Research and select a publicly available API for safety and health information by travel destination (CDC? New/travel APIs TripAdvisor?) and implement this method to fetch medication and vaccination requirements, as well as safety travel advisories for Method (1) output destinations.
  
* By Week 9:
  - Now that the project is completed with fully refined functionality, I'll film the video walk-through component and submit the project in accordance with the GoogleDoc Final Project instructions.
