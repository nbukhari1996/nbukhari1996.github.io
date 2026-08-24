## Hader Review

Phone: Samsung Galaxy A06(SM-A065F/DS)

Android Version: 16

One UI version: 8.0

Application Language: English

### Severity Legend
**[High]**
**[Medium]**
**[Low]**
**[Bug]**


## General notes

- **[High]** Confusing & unclear UI/UX
- **[High]** Design scheme inconsistencies
- **[High]** Address selection process needs work
- **[High]** Missing cart functionality
- **[High]** Missing thorough data validations
- **[High]** Lack of trust-building elements
- **[High]** Overflow at the bottom on almost every screen

### App-start
- **[Low]** 3 onboarding screens with generic text, no app-specific information, no value
- **[Medium]** Missing language setting early on. Users who speak only Arabic will have to go through the full registration + address + navigating to language settings flows in English

### Browse as guest
- **[Medium]** Unable to view information about service offerings

### Login

### Sign-up screen
- **[Medium]** Too many required fields before a user can access the application
- Phone
	- **[Bug]** Field not restricted to 9 digits
	- **[Possible Bug]** Users able to change area code to non-KSA number
- National ID
	- **[High]** Asking for National ID without providing a disclosure in the privacy policy is possibly in violation of Play Store compliance.
 		- "Google's User Data policy requires you to be transparent about how your app handles personal and sensitive user data. You must disclose what data you collect, how you use it, and who it's shared with. You must provide a valid privacy policy, obtain user consent, and handle data securely. Additionally, you must offer users a way to delete their accounts and associated data" - https://support.google.com/googleplay/android-developer/answer/10144311?hl=en
	- **[High]** Also possibly violates KSA's Personal Data Protection Law (PDPL) Article 11(3)
		- "The content of the Personal Data shall be appropriate and limited to the minimum amount necessary to achieve the purpose of the Collection"
		- National ID number is not necessary for single-visit home cleaning services
- City
	- **[Medium]** Mentions non-service locations, eg. Abu Dhabi
	- **[Low]** Duplicates & incorrect spelling
- District
	- **[Medium]** Doesn't filter to city that was picked
	- **[Medium]** Shows districts from non-service locations, eg. Abu Dhabi
	- **[Low]** Duplicates & incorrect spelling
- **[Medium]** Fields required that could be unnecessary for signing up:
	- Work sector
	- Nationality
	- Gender

<img width="250" height="555" alt="Screenshot_20260823_143626" src="https://github.com/user-attachments/assets/7200e8a8-66b9-47f2-9f35-9bd4fcc6a3e4" />
<img width="250" height="555" alt="Screenshot_20260823_143552" src="https://github.com/user-attachments/assets/92374f4a-1f3c-49b6-b0f0-93c6c4930a1a" />

- **[Medium]** Overflows at bottom
- **[Low]** Inconsistent design schemes for success/failure messages. Success has a white transparent background with a green line on the side, while the failure message has a red background.

<img width="250" height="555" alt="Pasted image 20260823145748" src="https://github.com/user-attachments/assets/390316cb-4785-417a-8701-d48401b3b066" />

- **[Low]** Fields are unappealing grey boxes with text, and no styling/icons or visual indicators
- **[Low]** After verifying the OTP 2 popups appear: Registration successful & OTP verified. Could show a single popup instead. 

#### Add Address
- **[Low]** Requires name, number, city, district again. Doesn't prefill using the information already provided
	- **[Medium]** Filling in city doesn't filter the districts
		- **[Medium]** Shows districts from non-service locations, eg. Abu Dhabi
- **[Bug]** No validation on address
- **[Low]** Unskippable, requires user to add an address now instead of allowing them to add address later
- Validation issues:
	- **[Low]** Empty fields don't show an error immediately when a user interacts with a field and leaves without inputting data
	- **[Low]** Field-level validation only appears after pressing "Proceed to Pin Location," and a popup appears too repeating the same information
		- **[Bug]** Able to enter a 3-digit phone number and it gets validated

<img width="250" height="555" alt="Pasted image 20260823155124" src="https://github.com/user-attachments/assets/8e2b733f-5e41-46d5-8cb6-b57667432166" />

- **[Low]** Overflow at bottom

#### Map Pin
- **[Medium]** Shows a polygon on the map. Different from what most users would expect, which is being able to pin a location and retrieve their full address eg. Noon or HungerStation
- **[Low]** Asks for city and district again
	- **[Low]** Filling in city doesn't filter the districts
		- **[Low]** Shows districts from non-service locations, eg. Abu Dhabi
- **[Bug]** Bugged districts, all of the districts open some shape in the specified city even if the district is not in Khobar
- **[Bug]** Unable to get my location when pressing the "Current location" button
- **[Bug]** When trying to save an address, popup appears saying "The additional direction field is required"
	- Unclear that this field has to be filled in the previous screen
		- Validation didn't occur on the previous screen for this field
	- **[Bug]** Popup appears repeatedly
 
<img width="250" height="555" alt="Screenshot 2026-08-23 155508" src="https://github.com/user-attachments/assets/a15848b9-bae7-494b-ab5e-3570fa9a673f" />

- **[Bug]** Overflow at bottom

### Home
- **[Low]** "Add your address" at the top despite having just entered my address while signing up. This is because it didn't set the entered address as the default address
- **[Medium]** All 3 service buttons, the topbar, and the best offers section have different design schemes(different color schemes, icons, typography, structure/theme of elements, etc) applied to them
- **[Low]** Support icon is greyed out

<img width="250" height="555" alt="Screenshot 2026-08-23 160045 1" src="https://github.com/user-attachments/assets/9917b38a-eca0-4117-b76f-bae786bab4e7" />

- **[Medium]** All 3 service offering screens have different design schemes

<img width="250" height="555" alt="Screenshot_20260823_144555" src="https://github.com/user-attachments/assets/00c896f9-42f6-47ee-84a5-ce0ed1f1e035" />

<img width="250" height="555" alt="Screenshot_20260823_144602" src="https://github.com/user-attachments/assets/875c119e-f7e5-4f6b-b4b0-ea504f18c6b3" />

<img width="250" height="555" alt="Screenshot_20260823_144559" src="https://github.com/user-attachments/assets/353ff4e4-ee08-4978-8598-bfeb1a864474" />


### Hourly Services

- **[Medium]** Options fade in, pressing options adds interactivity. Inconsistent design

#### Hader Hourly

- **[Medium]** Does not explain what service is being purchased, what is included, or how the service works or what precisely occurs during "Hader Hourly"

<img width="250" height="555" alt="Screenshot_20260823_140411" src="https://github.com/user-attachments/assets/82afad7f-195f-45ed-8cba-126fd96881fb" />

- **[Bug]** Pressing the "Address" pin at the top redirects to the previous page
- **[Low]** Unclear button at top saying "Monthly package" monthly what? WHAT IS BEING PROVIDED TO ME? No further details on the Monthly Package screen either
- **[Low]** Why is there a button to "Select shift" and "Visit period" for only 4 options? Why not display all 4 options for the user together?
	- Possible solution: Users should be able to select precise timings for service, unsure if this is logistically possible
- **[Medium]** "Arrival Time" text box provides contradictory information and it's unclear what it is trying to say. Why is there a different arrival time from what the user is selecting? Does 8 AM to 12 PM mean a cleaner will work for 4 hours? Or will they work 2/1 hours 30 minutes as specified in the text box?  The user doesn't know when they will get their cleaning service provided and the "Arrival Time" text confuses them even further!
- **[Low]** Spelling mistakes

<img width="250" height="555" alt="Screenshot_20260824_090616" src="https://github.com/user-attachments/assets/076a2508-35ad-4306-b1be-0545be18e172" />

- **[Bug]** Overflow at the bottom
- **[Low]** Design inconsistency, picked date turns blue instead of a theme color

<img width="250" height="555" alt="Screenshot_20260824_091403" src="https://github.com/user-attachments/assets/c2b4595c-5f76-476b-9351-9f12c738ba2c" />

- **[Low]** Why are users then asked to select "Days" in the sliding day selection AFTER selecting it in the calendar? Why not allow users to just select the dates they want a visit in the calendar view? Confusing!
	- **[Bug]** When selecting a start date in the calendar, then selecting a date after that in the sliding day selector, I am able to deselect the original date. But it doesn't update in the "Start Date."
- **[Low]** Price at the bottom does not update instantly
- **[Low]** Days of visit is unclear in the "package details" section, it just repeats the days and not the date. What happens when a user wants to book 2 consecutive Sundays? It just says Sunday/Sunday, whereas showing the dates instead would convey more information
- **[Low]** The "package details" section is completely redundant, it only shows the information within the screen the user is already on

#### Order Summary

<img width="250" height="555" alt="Screenshot_20260824_092355" src="https://github.com/user-attachments/assets/5cbf261f-eb70-4482-bcc2-02d409eedc53" />

- **[Low]** Colors/styles change once again
- **[Low]** Inconsistent & confusing wording(eg. Uses "Experts" instead of "Staff" which was used in the previous screen. Why does it say "From" instead of "Nationality"?)
- **[Medium]** Pressing the edit icon on "Address" doesn't do anything

#### Monthly Package

- **[Low]** Wording issue, button says "Monthly package" but the title of the screen is "Monthly contract"

<img width="250" height="555" alt="Screenshot_20260823_134809" src="https://github.com/user-attachments/assets/7de5c739-4b6c-4b58-8ef1-3bc96b0ff735" />

-  **[Bug]** Address at top gets cleared
-  **[Medium]** Pressing the address at the top goes back to the previous screen and all progress is lost
-  **[Low]** Contract Duration says "Months" in parentheses but it also displays weeks without any order
-  **[Medium]** Doesn't clarify how many visits per contract. Doesn't clarify any information! What is this visit even about? What will happen? No steps are provided. Will I receive a confirmation? Will I get a call before a service? Will it be the same time/cleaner each week/day?
-  **[High]** No cart. Going to a previous page loses all progress

#### Hospitality

-  **[Bug]** Pressing the address icon up top goes back
-  **[Low]** Unclear what this service is. Meaningless description, cut off text
-  **[Bug]** When picking an unavailable start date, the error message is nonsensical

#### Hourly babysitter service

-  **[Low]** No meaningful information in description, repeats title

#### Hader extra hourly

-  **[Low]** Unclear what this is. How is this different from Hader Hourly?


### Live-in service

-  **[Low]** Inconsistent design again. Different buttons from the rest of the app/service screens.
-  **[Low]** Is engineering professions a valid offering?
-  **[Low]** Service offerings are unclear. Live-in is not clarified. It is not clear that this requires signing a contract and is a long commitment
-  **[Low]** Inconsistent packages, displays packages in Arabic instead of English
-  **[Low]** No logical sorting of packages, not sorted by duration of time, or pricing
-  **[Low]** Wording issues, uses installment "tenor" which might be an industry term, and not something a user would easily understand
-  **[Low]** "Select preferred due day of month" what is this for? No clue! Why is it a dropdown saying "Day 1" "Day 2" etc.? Surely a cleaner solution is possible

<img width="250" height="555" alt="Screenshot_20260823_141502" src="https://github.com/user-attachments/assets/43c51eac-3d28-4725-a803-1cfe725039e0" />

-  **[Bug]** Overflow at bottom
-  **[Medium]** Calculation for monthly payments greater than 1 year seems incorrect because the numbers don't add up

<img width="250" height="555" alt="Screenshot_20260824_100033" src="https://github.com/user-attachments/assets/25f9bef9-e746-4e25-8eda-a70fd04666b9" />

-  **[Bug]** Overflow at bottom
-  **[Low]** Experience = 2.5 what? Years? Months?
-  **[Low]** CV Doesn't list skills or any other information. Repeats the information in the app
-  **[Bug]** Selecting address at the top goes back to the previous screen
-  **[Medium]** Going back loses progress, no cart

<img width="250" height="555" alt="Screenshot_20260824_100255" src="https://github.com/user-attachments/assets/62a0988e-257d-409e-8565-1e0b3475cc0e" />

-  **[Bug]** Overflow at bottom
-  **[Medium]** Missing Mada & Tamara payment options

### Additional Services

<img width="250" height="555" alt="Screenshot_20260823_144602" src="https://github.com/user-attachments/assets/875c119e-f7e5-4f6b-b4b0-ea504f18c6b3" />
-  **[Low]** Baby sitter service says coming soon but it's available in "Hader Hourly" screen

### Booking History
-  **[Medium]** Different design scheme again. Buttons with black border are not used elsewhere. Calendar has a different design scheme
-  **[Bug?]** Can't press the filter button
-  **[Bug]** Filters don't behave as expected. Why does it "Select" a filter when I press a button of a filter but only view it and don't select it?

### Notifications
-  **[Low]** Can't remove/delete notifications

### Profile

<img width="250" height="555" alt="Screenshot_20260824_102727" src="https://github.com/user-attachments/assets/bc096535-c7e1-4a38-a3b4-0b519b645ef4" />

-  **[Low]** Different design scheme once again. This is the cleanest one so far, but the rest of the app doesn't follow it

#### Booking History

-  **[Low]** Repeats information already present in the Bookings tab

#### Wallet

-  **[Low]** Inconsistent design, different from the rest of the app

#### Invoices

-  **[Low]** Doesn't lead anywhere

#### Favorites

-  **[Low]** Didn't see an option to set Favorites while exploring SPs, but see it here. How does one set a SP as favorite?

#### Terms & Conditions
-  **[Low]** Says payment are due upon completion, but we ask for payment upfront

#### FAQ

<img width="250" height="555" alt="Screenshot_20260824_103209" src="https://github.com/user-attachments/assets/4ada3f44-59bb-4916-8509-50ba5d55eee7" />

-  **[Low]** Incorrect FAQ information:
	- It lists cleaning services we do not offer. Hader only offers 1 standard cleaning service, either as a one-time visit or a recurring visit
	- Booking a cleaning service option is not supposed to have email option
	- Cleaning service pricing does not depend on these factors
	- Is a person supposed to be there? Unsure. Other cleaning apps require not only a person but specifically a woman to be a home during cleaning time

#### Edit Address

-  **[Bug]** When pressing "Edit" on an address, all previous information about the address is cleared and an empty form is presented
-  **[Bug]** Missing phone validations, able to save a 3-digit phone number
-  **[Bug]** Editing address makes the success popup appear repeatedly

<img width="250" height="555" alt="Screenshot_20260824_083735" src="https://github.com/user-attachments/assets/12ae8461-7329-4594-a1f7-132df3328c22" />
<img width="250" height="555" alt="Screenshot_20260824_083713" src="https://github.com/user-attachments/assets/f968ee77-4c59-4ca9-9ef8-dae88ba2ceb9" />
<img width="250" height="555" alt="Screenshot_20260823_143812" src="https://github.com/user-attachments/assets/f8703cef-232d-40a0-82d1-2199b4325391" />

-  **[Bug]** Overflow at bottom

#### Language

-  **[Bug?]** Selecting the language that is already set in the "Language" setting changes the language of the app again momentarily before it realizes the language was already selected! Only applies for Arabic

---
