## Review

Phone: Samsung Galaxy A06(SM-A065F/DS)

Android Version: 16

One UI version: 8.0

### App-start
- Splash screen
- Notification permission request
- Another splash screen(Different one?)
- 3 onboarding screens with generic text

- Missing language setting early on. Users who speak only Arabic will have to go through the full registration + address + navigating to language settings flows in English
### Browse as guest
- Unable to view any information about service offerings
### Login

### Sign-up screen
- Too many required fields before a user can access the application
	- Phone
		- Field not restricted to 9 digits
		- Users able to change area code to non-KSA number
	- Asking for National ID without providing a disclosure in the privacy policy likely breaks Play Store compliance. 
		- Also likely breaks KSA's Personal Data Protection Law (PDPL) Article 11(3)
			- "The content of the Personal Data shall be appropriate and limited to the minimum amount necessary to achieve the purpose of the Collection"
			- National ID number is not necessary for single-visit home cleaning services
	- City
		- Mentions non-service locations, eg. Abu Dhabi
		- Duplicates & incorrect spelling
	- District
		- Doesn't filter to city that was picked
		- Shows districts from non-service locations, eg. Abu Dhabi
		- Duplicates & incorrect spelling
	- Fields that seem not as important as a requirement for signing up:
		- Work sector
		- Nationality
		- Gender

Send OTP modal overflows at bottom of screen

Fields are unappealing grey boxes with text, and no styling/icons or visual indicators

<img width="348" height="773" alt="Pasted image 20260823145748" src="https://github.com/user-attachments/assets/390316cb-4785-417a-8701-d48401b3b066" />

After verifying the OTP 2 popups appear:

Registration successful & OTP verified. Could show a single modal instead. 

#### Add Address
- Requires name, number, city, district again. Doesn't prefill using the information already provided
	- Filling in city doesn't filter the districts
		- Shows districts from non-service locations, eg. Abu Dhabi
- No validation on address
- Unskippable, requires user to add an address now instead of allowing them to add address later
- Opening an address to edit it makes it blank (INCOMPLETE)
- Validation issues:
	- Empty fields don't show an error immediately when a user interacts with a field and leaves without inputting data
	- Field-level validation only appears after pressing "Proceed to Pin Location," and a popup appears too repeating the same information
		- Able to enter a 3-digit phone number and it gets validated

<img width="348" height="773" alt="Pasted image 20260823155124" src="https://github.com/user-attachments/assets/8e2b733f-5e41-46d5-8cb6-b57667432166" />

- Overflow at bottom
#### Map Pin
- Shows a polygon on the map. Different from what most users would expect, which is being able to pin a location and retrieve their full address eg. Noon or HungerStation
- Asks for city and district again
	- Filling in city doesn't filter the districts
		- Shows districts from non-service locations, eg. Abu Dhabi
- Possibly bugged districts, all of the districts open some shape in the specified city even if the district is not in Khobar
- Unable to get my location when pressing the "Current location" button
- When trying to save an address, popup appears saying "The additional direction field is required"
	- Unclear that this field has to be filled in the previous screen
		- Validation didn't occur on the previous screen for this field
	- Bug: Popup appears repeatedly

<img width="348" height="773" alt="Screenshot 2026-08-23 155508" src="https://github.com/user-attachments/assets/a15848b9-bae7-494b-ab5e-3570fa9a673f" />

- Overflow at bottom
### Home
- "Add your address" at the top despite having just entered my address while signing up. This is because it didn't set the entered address as the default address
- All 3 service buttons, the topbar, and the best offers section have different design schemes applied to them

- <img width="348" height="773" alt="Screenshot 2026-08-23 160045 1" src="https://github.com/user-attachments/assets/9917b38a-eca0-4117-b76f-bae786bab4e7" />

	- Meaning different color schemes, icons, typography, structure/theme of elements, etc.
- Support icon is greyed out
