# MeetOut

##Project description
This project is a serverless, progressive web application (PWA) with React using a test-driven development (TDD) technique.
##How to get the project running

##Project dependencies 

## API -
The application uses the Google Calendar API to fetch upcoming events.

## User stories-

**FEATURE 1:** FILTER EVENTS BY CITY
**Scenario 1:** When a user hasn’t searched for a city, show upcoming events from all cities.
**Story1:** As a user,
 I should be able to view a list of events when loading the page.
So that I receive information about events.

Given- The page has been loaded and no search was performed yet.
When - The page is loaded by the user’s browser.
Then- The events element will show upcoming events from all cities.

**Scenario 2:** User should see a list of suggestions when they search for a city.
**Story2:** As a user,
 I should be able to see a list of suggestions when searching for a city,
So that I can find my city quicker.
Given- User has searched for a specific city.
When-After a user is typing in the search bar.
Then- The user will be shown a list of suggestions.

**Scenario 3:** User can select a city from the suggested list.
**Story 3:** As a user,
 I should be able to choose a city from the suggested list
So that I can choose my city without having to type the whole name.
Given-App has loaded and the search input box appears on the page.
When-User  clicks the empty input box.
Then- A dropdown list of recommended cities will appear below the input box.


**FEATURE 2:** SHOW/HIDE AN EVENT’S DETAILS
**Scenario 1:** An event element is collapsed by default.
**Story 1:** As a user,
 I should be able to first see an event without extra details
So that I’ll be presented with a view that’s not overwhelming with data.
Given- A collapsed event element containing events is shown on the page.
When- the user loads the page and performs no action.
Then- The event element contains a button to expand and show the events.

**Scenario 2**: User can expand an event to see its details.
**Story 2:** As a user,
 I should be able to expand an event to see more details
So that I can learn more about an event that interests me.
Given-  The event element has been expanded.
When- The user clicks on  a show details button in the event element.
Then- The event element will expand to show details about the specific event chosen.

**Scenario 3:** User can collapse an event to hide its details.
**Story 3:** As a user,
 I should be able to hide an events details
So that I have control over which events details I can see.
Given- The event element has expanded, a show details button expanded the elements to show details of a specific event.
When- The hide details button is clicked on the event element.
Then- The expanded event will show details of a specific event.



**FEATURE 3:** SPECIFY NUMBER OF EVENTS
**Scenario 1:** When a user hasn’t specified a number, 32 is the default number.
**Story 1:** As a user,
 I should be able to see a set number of events
So that I can see the events without needing to set a default number.
Given- A user has yet to set a number of events.
When- A user loads the website and expands the events element.
Then- The events element will show 32 events as a default.

**Scenario 2:** User can change the number of events they want to see.
**Story 2:** As a user,
 I should be able to change the number of events shown
So that I can adjust it to my preference.
Given-The app and the events element have been loaded. 
When-The user expands the events element and sets an input of desired events to be shown.
Then-The event elements will show the number of events set by the user.



**FEATURE 4:** USE THE APP WHEN OFFLINE
**Scenario 1:** Show cached data when there’s no internet connection.
**Story 1:** As a user,
 I should be able to use the app when offline
So that I wouldn’t be dependent on an internet connection to have access to the app.
Given-The user didn’t connect to the internet and opened the app.
When-The user uses the app while offline.
Then-App will show data saved in the user cache from when the user was online on the website.


**Scenario 2:** Show error when user changes the settings (city, time range).
**Story 2:** As a user,
 I should be able to know when an action can’t be performed
So that I understand what is possible to do with the app when offline.
Given-User has been using the app offline.
When-User is trying to change a setting.
Then-User will be presented with an error- “Action unavailable while offline”.

**FEATURE 5:** DATA VISUALIZATION
**Scenario 1:** Show a chart with the number of upcoming events in each city.
**Story 1:** As a user,
 I should be able to see a chart showing the number of upcoming events in each city
So that I have a clear visual representation of the upcoming events.

Given-User has chosen a city.
When-The events element for a specific city is loaded.
Then-Chart displaying the number of upcoming events in the chosen city will be shown.

