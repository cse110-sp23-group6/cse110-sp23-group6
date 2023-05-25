# Meeting 11 + Date: 05/24/23
## Attendance
- [X] Haven Ahn
- [X] Amit Namburi
- [X] Fayaz Shaik
- [X] Brian Ton
- [X] Vasil bogdev
- [X] Jose Arreguin
- [X] Botao Zhang
- [X] Prisha Anand
- [ ] Bao Thy Nguyen
- [ ] Wilson Nguyen

## Agenda
 - review sprint 2 
 - assign tasks for next sprint
 - delegate retrospective, sprint review, and video assignments 

## Sprint 2 Review 
 
### CI/CD Update: Amit, Prisha 
- Currently using Super-Linter, JSDocs 
- JSDocs still needs to be set up to output files 
- Video explaining GitHub Actions
- Need to figure out how to deploy (intially thought we would need GitHub pro, but seems that we can simply make the repo public) 

### New Profile Page Update: Jose
- Added functionality where you can not select the submit button until all profile fields are filled out 
- Validate input (can not have "nonsense" input, such as words in the date fields) 
- Sends all information to the live server (storage) 
- Need to add this same functionality to emotions1 and emotions2 page, so that users can only go to the next page if they click one of the buttons 

### Scaling & Standardization: Vasil
- General Readings Page got scaled 
- Need to add some javascript code that makes sure reading's text is always sized to fit inside the box (respective to length of the reading) 
- Standardization Doucment --> not applicable to every page so we might need to reformat it or scrap it all together, one possible idea is to look at the figma and ensure that sizing remains the same even if you zoom in and out and resize the browser 

### Welcome Page: Botao 
- Resolved the welcome page to use JS instead of JQuery for the animation 

### Emotions1 Update: Prisha 
- Each button corresponds to the correct emotion, while still being randomly generated within the set 
- Cleaned up old code so that image sets are stored in array 
- Send the clicked on button to local storage 

### Emotions2 Update: Haven
- Added navigation to emotions2 
- Added date functionality

### Previous Fortunes Update: Haven
- Added button for new reading (each time a user gets one generated, it shows up in the log of past readings) 
- Ability to open each reading (expand contents) so that the entire text is visible, and contracts back to preview size
- Can also delete fortunes from the log (CRUD functions!) 

### General Reading Update: Brian
- Navigation between all pages
- Take info from emotions1 and emotions2 and display corresponding gif image on general reading 
- Added quotes and image links into JSON file to have cleaner code

## General Rules Discussed: 
- Make sure to use tabs instead of spaces 
- Fix linter locally (using feedback from the branch) and then create pull requests

## Sprint 3 Roles: 
- Testing Team (Jest, Pupetteer): Brian, Vasil, Fayaz
- Status Video: Wilson, Bao (add more people if needed) 
- Sprint Review & Retrospective: Amit, Prisha 
- Next-Button Validation Emotions1 & Emotions2: Jose
- General Reading JS (changing font size): Vasil 
- GitHub Pages Deployment: Botao
- Finalize CRUD Functionality on Profile Page: Haven
- @everyone: if you finish your tasks early, add to the JSON for more general readings 
- @everyone: add comments in JSDocs style, fix linter issues, clean code! 
- @everyone: add more detail into your github issues 

## Main Goals: 
- GitHub pages runs & deploys 
- Skeleton walk thru of project
- Priortize making github issues more detailed 





