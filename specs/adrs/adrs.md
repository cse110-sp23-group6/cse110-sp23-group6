# ADRs (Architectural Decision Records)

## Decision 1: Using Local Responses (04/26/23)

### Context and Problem Statement

How to generate resposnes for each fortune? 
How to ensure the responses are somewhat unique? 

### Considered Options

* Chat GPT API
* Creating our own set of local responses

### Decision Outcome

Chosen Outcome: Utilize a finite set of local responses as fortunes (see below). 

### Pros and Cons of the Options

### Locally Generated Responses 
* Good, because we can decide what exactly to have in each response 
* Good, because locally sourced so no issue with third-parties 
* Good, because can get responses almost immediately
* Good, because works offline
* Bad, because we can only have a finite set of responses so their will be redundancy
* Bad, because users can not input their own questions or emotions and must choose from five options 

### Chat GPT API
* Good, because can generate a different unique response each time
* Good, because users can ask specific questions
* Bad, because we would need to pay for the API (extra cost)
* Bad, because would not provide anything different from Chat GPT itself (users might want to just use it directly)
* Bad, because can cause problems if API gets cancelled or bugs are found (dependency) 
* Bad, because can take time to send request to Chat GPT and then send back response to our app 
* Bad, because may not work properly offline

# Decision 2: Documentation with JSDocs (in progress)

### Context and Problem Statement 

How can we best automate creating document for our JavaScript code? 

### Considered Options 

* JSDocs 
* TypeScript

### Decision Outcome

Chosen Outcome: Utilize JSDocs in our CI/CD pipeline in order to document JS code. 

### Pros and Cons of the Options 

### JSDocs 
* Good, because explains functions header using @description tags. 
* Good, because easier to learn and has collapsable comments
* Good, because hovering over a function/variable gives context
* Bad, because fewer tools for maintenance

### TypeScript
* Good, because far more tools for maintenance and testing 
* Good, because has type names for variables 
* Bad, because harder for beginners to learn 
* Bad, because does not match our function description convention
* Bad, because of example in lecture of TypeScript being tedious

# Descision 3: Storing Animations Using .gif (05/21/23) 
## Initial Decision: Store Animations Using .mp4 (04/30/23)

### Context and Problem Statment

How can we best store and display animated images on our webpage using html? 

### Considered Options 

* .gif Image Format
* .mp4 Video Format
* Replicate animation through html and css

### Decision Outcome

Chosen Outcome: Ensure animated images are in the .mp4 video format. (04/30/23)

*Update: Ensure animated imageas are done in the .gif format. (05/20/23) *


### Pros and Cons of the Options

### .mp4 Video Format
* Good, because better compatability with html than image
* Good, because less storage space (5 second animation) 
* Bad, because might not play immediately and not consistent with previous pages that use images 
* *Update (05/21/23): Bad, because does not play on display, sometimes does not play at all. Issues with rendering*

### .gif Image Format
* Good, because can maintain consistency with other images and display everything as images 
* *Update (05/21/23): Good, because format allows playing immediately on display.*
* Bad, because html has a history of lagging and erroring with this format 
* Bad, because sometimes gets stored as a sequence of 100 images (too much space)

### Replicating animation using html and css 
* Good, because do not need to worry about .gif and .mp4 issues 
* Bad, because hard to maintain consisteny in animation for each image
* Bad, because would need to import specific font and animation style and alter existing design (more time)

### Futher Notes

This decision is subject to change as we try out the video format and discover potential issues. (TBD) 

*Update: We decided during the meeting on 05/20/23 to change from using .mp4 display format to .gif format.* 

# Decision 4: Category is Stored in URL, Local Storage for the Rest (05/20/23) 

### Context and Problem Statment

How can we best store which category the user selected through the fortune? 
How can we best store the images and quote selections made by the user? 

### Considered Options 

* Use the URL to store the states 
* Use local storage 

## Decision Outcome: 

Utilize the URL to store the current category, and for images and quotes, utlize the local storage. 

### Pros and Cons of the Options 

### Using the URL 
* Good, because can easily see the state you are in through the link itself, which is unique. 
* Good, because allows you to have multiple tabs open within the same device. 
* Bad, because might take longer to implement since class labs focused on using local storage. 

### Using Local Storage 
* Good, because can't be user edited. 
* Good, because can store in .JSON file. 
* Bad, because can't have multiple tabs upon without state changing across tabs. 

### Further Notes 
* Since the four possible categories that the user can select are only one-word each, it is reasonable to use the URL. Additionally, we do not mind if the user can manually edit the category by changing the name within the link, since it would be the same as if they went back home or selected the back button. This way, the user will be able to have multiple tabs open, each consisting of different categories. This is a crucial function for our app since users can benefit from being able to get fortunes from different categories at the same time. 
* In regards to the image and quote selection, which determines the users emotional aura, we decided using local storage would be better. This is because the user is not supposed to know which images/quotes correspond to which emotions, and having the name of the emotion display in the URL would defeat the purpose as they would be able to easily edit the links to have whatever they want, rather than what corresponds to the image/quote they selected. Additionally, we can use a .JSON file to store the list of generated responses, which are multiple sentences so it is reasonable for them to have their own file. Moreover, we want to implement a functionality that only allows a user (one device) to be able to acess each category once a day, so there is no need for being able to have multiple tabs within the same category to be open. 
*Subject to change as we find further pros and cons during implementation (TBD).*
