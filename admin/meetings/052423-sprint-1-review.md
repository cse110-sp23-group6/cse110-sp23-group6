# Meeting 11 (Sprint 1 Review) + Date: 05/24/23

## Attendance
- [X] Haven Ahn
- [X] Amit Namburi
- [X] Fayaz Shaik
- [X] Brian Ton
- [X] Vasil bogdev
- [X] Jose Arreguin
- [X] Botao Zhang
- [X] Prisha Anand
- [ ] Bao Thy Nguyen - excused
- [ ] Wilson Nguyen

## Sprint 1 Review 
 
### CI/CD Update: Amit, Prisha 
- Currently using Super-Linter, JSDocs 
- JSDocs still needs to be set up to output files 
- Video explaining GitHub Actions
- Need to figure out how to deploy (intially thought we would need GitHub pro, but seems that we can simply make the repo public) 
- <img width="1187" alt="image" src="https://github.com/cse110-sp23-group6/cse110-sp23-group6/assets/60487925/72de7cab-79c8-474f-984d-f811cd57ca1b">

### New Profile Page Update: Jose
- Added functionality where you can not select the submit button until all profile fields are filled out 
- Validate input (can not have "nonsense" input, such as words in the date fields) 
- Sends all information to the live server (storage) 
- Need to add this same functionality to emotions1 and emotions2 page, so that users can only go to the next page if they click one of the buttons 
- <video src="https://github.com/cse110-sp23-group6/cse110-sp23-group6/assets/60487925/15b5a4f4-fc37-444d-ace6-3295eebab2a6" controls="controls" style="max-width: 730px;"> </video>

### Scaling & Standardization: Vasil
- General Readings Page got scaled 
- Need to add some javascript code that makes sure reading's text is always sized to fit inside the box (respective to length of the reading) 
- Standardization Doucment --> not applicable to every page so we might need to reformat it or scrap it all together, one possible idea is to look at the figma and ensure that sizing remains the same even if you zoom in and out and resize the browser 

### Welcome Page: Botao, Fayaz 
- Resolved the welcome page to use JS instead of JQuery for the animation 
- Add navigation buttons and standardize the text
- <video src="https://github.com/cse110-sp23-group6/cse110-sp23-group6/assets/60487925/e5107189-c3c3-429f-bb2b-9cafca5cc212" controls="controls" style="max-width: 730px;"> </video>

### Emotions1 Update: Prisha 
- Each button corresponds to the correct emotion, while still being randomly generated within the set 
- Cleaned up old code so that image sets are stored in array 
- Send the clicked on button to local storage 
- <img width="1187" alt="image" src="https://github.com/cse110-sp23-group6/cse110-sp23-group6/assets/60487925/9323c8ab-3f91-4ba0-bf12-5254fb03b21a">

### Emotions2 Update: Haven
- Added navigation to emotions2 
- Added date functionality

### Previous Fortunes Update: Haven
- Added button for new reading (each time a user gets one generated, it shows up in the log of past readings) 
- Ability to open each reading (expand contents) so that the entire text is visible, and contracts back to preview size
- Can also delete fortunes from the log (CRUD functions!) 
- <img width="1187" alt="image" src="https://github.com/cse110-sp23-group6/cse110-sp23-group6/assets/60487925/29c0a127-b8d1-47c2-bb07-f3e4f5bbe466">
- <img width="1187" alt="image" src="https://github.com/cse110-sp23-group6/cse110-sp23-group6/assets/60487925/06a0cd80-4386-438f-ac74-c3c69513d2f4">

### General Reading Update: Brian
- Navigation between all pages
- Take info from emotions1 and emotions2 and display corresponding gif image on general reading 
- Added quotes and image links into JSON file to have cleaner code
