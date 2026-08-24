## Hader Review

Phone: Samsung Galaxy A06(SM-A065F/DS)

Android Version: 16

One UI version: 8.0

Application Language: English

### Legend
**[High]**
**[Medium]**
**[Low]**
**[Bug]**

### App-start
- **[Low]** 3 onboarding screens with generic text
- **[Medium]** Missing language setting early on. Users who speak only Arabic will have to go through the full registration + address + navigating to language settings flows in English

### Browse as guest
- **[Medium]** Unable to view any information about service offerings

### Login

### Sign-up screen
- **[Medium]** Too many required fields before a user can access the application
- Phone
	- Field not restricted to 9 digits
	- Users able to change area code to non-KSA number
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
	- **[Medium]** Duplicates & incorrect spelling
- **[Medium]** Fields that are unnecessary for signing up:
	- Work sector
	- Nationality
	- Gender

**[Medium]** Send OTP modal overflows at bottom of screen

**[Low]** Fields are unappealing grey boxes with text, and no styling/icons or visual indicators

<img width="250" height="555" alt="Pasted image 20260823145748" src="https://github.com/user-attachments/assets/390316cb-4785-417a-8701-d48401b3b066" />

**[Low]** After verifying the OTP 2 popups appear: Registration successful & OTP verified. Could show a single popup instead. 

#### Add Address
- **[Medium]** Requires name, number, city, district again. Doesn't prefill using the information already provided
	- **[Medium]** Filling in city doesn't filter the districts
		- **[Medium]** Shows districts from non-service locations, eg. Abu Dhabi
- **[Medium]** No validation on address
- **[Low]** Unskippable, requires user to add an address now instead of allowing them to add address later
- Opening an address to edit it makes it blank (INCOMPLETE)
- Validation issues:
	- Empty fields don't show an error immediately when a user interacts with a field and leaves without inputting data
	- Field-level validation only appears after pressing "Proceed to Pin Location," and a popup appears too repeating the same information
		- Able to enter a 3-digit phone number and it gets validated

<img width="250" height="555" alt="Pasted image 20260823155124" src="https://github.com/user-attachments/assets/8e2b733f-5e41-46d5-8cb6-b57667432166" />

- **[Low]** Overflow at bottom

#### Map Pin
- Shows a polygon on the map. Different from what most users would expect, which is being able to pin a location and retrieve their full address eg. Noon or HungerStation
- Asks for city and district again
	- Filling in city doesn't filter the districts
		- Shows districts from non-service locations, eg. Abu Dhabi
- Bugged districts, all of the districts open some shape in the specified city even if the district is not in Khobar
- Unable to get my location when pressing the "Current location" button
- When trying to save an address, popup appears saying "The additional direction field is required"
	- Unclear that this field has to be filled in the previous screen
		- Validation didn't occur on the previous screen for this field
	- Bug: Popup appears repeatedly
 
<img width="250" height="555" alt="Screenshot 2026-08-23 155508" src="https://github.com/user-attachments/assets/a15848b9-bae7-494b-ab5e-3570fa9a673f" />

- Overflow at bottom

### Home
- "Add your address" at the top despite having just entered my address while signing up. This is because it didn't set the entered address as the default address
- All 3 service buttons, the topbar, and the best offers section have different design schemes(different color schemes, icons, typography, structure/theme of elements, etc) applied to them
- Support icon is greyed out

<img width="250" height="555" alt="Screenshot 2026-08-23 160045 1" src="https://github.com/user-attachments/assets/9917b38a-eca0-4117-b76f-bae786bab4e7" />

- All 3 service offering screens have different design schemes

<img width="250" height="555" alt="Screenshot_20260823_144555" src="https://github.com/user-attachments/assets/00c896f9-42f6-47ee-84a5-ce0ed1f1e035" />

<img width="250" height="555" alt="Screenshot_20260823_144602" src="https://github.com/user-attachments/assets/875c119e-f7e5-4f6b-b4b0-ea504f18c6b3" />

<img width="250" height="555" alt="Screenshot_20260823_144559" src="https://github.com/user-attachments/assets/353ff4e4-ee08-4978-8598-bfeb1a864474" />


### Hourly Services






### Profile

#### Edit Address

- When pressing "Edit" on an address, all previous information about the address is cleared and an empty form is presented
- Missing field-level validations
- Editing address makes the success popup appear repeatedly

<img width="250" height="555" alt="Screenshot_20260823_143812" src="https://github.com/user-attachments/assets/f8703cef-232d-40a0-82d1-2199b4325391" />
<img width="250" height="555" alt="Screenshot_20260824_083735" src="https://github.com/user-attachments/assets/12ae8461-7329-4594-a1f7-132df3328c22" />
<img width="250" height="555" alt="Screenshot_20260824_083713" src="https://github.com/user-attachments/assets/f968ee77-4c59-4ca9-9ef8-dae88ba2ceb9" />

- Overflow at bottom
