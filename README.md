# Transavia_Flight

#1 
Scenario: To search for a flight (General)
Given: Homepage of Transavia "https://www.transavia.com/en-NL/home/"
When: All the fields are filled with correct values.(from / to / Depart on / Return on / Who will be travelling? )
And: Check the option 'Show Prices in Flying Blue Miles' and Search button is used
Then: A page 'Book a Flight' with flight options and Flying Blue Login window should open
But : If the option 'Show Prices in Flying Blue Miles' is not marked then 'Book a Flight' page should not have 'Flying Blue Login' window

#2
Scenario: Advance search for a flight 
Given: Homepage of Transavia "https://www.transavia.com/en-NL/home/"
When: All the fields are filled with correct values.(from / to / Depart on / Who will be travelling? )
And:  Advance Search option is used
Then: A page 'Book a Flight' should open with 'Select your Wishes' window

#3
Scenario: The airport names should appear in dropdown list in 'from/to' fields
Given: Homepage of Transavia "https://www.transavia.com/en-NL/home/"
When: User clicks on From/To field
Then: A dropdown containing the name of Airports should appear
But: The same airport name in From/To field should give an eror

#4
Scenario: To check the calendar
Given: Homepage of Transavia ("https://www.transavia.com/en-NL/home/")
And: Depart on/ Return on field for searching of a flight
When: User clicks on 'Depart on/Return on' field
Then: A calendar should open with today onwards date
And: User should be able to select another month or year in future
But: The past dates must not be selected

#5
Scenario:To test inspiration button 'Enojoy Europes nicest islands'
Given:  Homepage of Transavia ("https://www.transavia.com/en-NL/home/")
When: User clicks on Enojoy Europes nicest islands
Then: A page with information on islands should open from where flights can also be booked

#6
Scenario:To check if the dropdown is working according to its function
Given : Homepage of Transavia ("https://www.transavia.com/en-NL/home/")
And: Menu bar of homepage
When: User click on <text>   (text= Plan and book/ Manage your booking/ Service)
Then: Corresponding <text> dropdown should open
And: User must be able to choose any of the given options from the dropdown

#7
Scenario: To check if the links are working according to the functionality
Given: Homepage of Transavia ("https://www.transavia.com/en-NL/home/")
When: User clicks on <link>  (link= any link on the page)
Then : Corresponding <link> Page should open either on same page or in new tab depending on user selection
And: Social networking sites*(available on the webpage)  (*Facebook/Twitter/Instagram/Whatsaap/Youtube/Google Plus) should open in new tab.

#8
Scenario: To search for a flight when any one field or both fields(from/to) are missing
Given:Homepage of Transavia ("https://www.transavia.com/en-NL/home/")
When: User clicks on Search button without selecting 'a destination or origin point or both'
Then: It should show error.

#9 
Scenario: To check Newsletter Subscription Functionality
Given: Homepage of Transavia ("https://www.transavia.com/en-NL/home/") > Newsletter Subscription
When: User enter a correct email id and click on Subscribe Button
Then: An acknowlegement statement should appear that 'the confirmation link has been sent to the given e-mail.'


