# Meeting 3 + 04/26/23
## Attendance
- [X] Haven Ahn
- [X] Amit Namburi
- [ ] Fayaz Shaik
- [X] Brian Ton
- [X] Vasil bogdev
- [X] Jose Arreguin
- [X] Botao Zhang
- [X] Prisha Anand
- [X] Bao Thy Nguyen
- [X] Wilson Nguyen

## Agenda
 - brainstorm ideas for fortune telling project
 - vote on favortie ones

### Unfinished Business
 - continue brainstorming at next meeting (on sat meeting) 
 - think more about ideas / elaborate current ones
 - create mock UI design (using figma) 

## Today's Topics
 
#### General Brainstorm of Ideas: 
  * 1. spotify wrapped inspired fortune telling: generate user aura that mixes different colors based on emotion, corresponding fortune
  * 2. spotify api w/facial recognition: discussed Amit's earlier project which looks at facial expression through camera to detect emotion, then geneates playlist of 10 songs based on that
  * → idea to use some sort of facial recognition to detect emotion in project? ask TA about feasability and guidelines for this  
  * 3. birthday based timeline: user inputs their birthday and fortune teller generates a timeline of important predicted events in their life, can also include life graph
  * 4. dice throwing: roll dice and have some randomized fortune output 
  * 5. astrology based fortune: ask for information (ie: birthday) from the user, generate personalized fortune based on birthday
  * → can group into 12 zodiac signs and have fortune tailor to characteristics of each sun sign 
  * 6. taro card reading: can have user choose random cards, can have animation of parakeets choose cards (parakeet astrology) and output reading based on that 
  * 7. fake ouija board 
  * 8. ancient turtle shell fortune telling: remove shell of the turtle, add fire to shell, and divine fortune based on marks 
 
#### MVP Idea: 
Combine idea of using aura & emotions with birthday based astrology. 
General Design: 
1. Give user a set of colors / pictures that they can choose which allows us to determine their emotions (and aura). 
   - can branch off after first choice for second choice
   - ask chat gpt to aid with image & color generation 
   - 5 basic emotions: joy, sad, anger, fear, disgust 
   - bank of 5 different questions (minimim), but user only gets asked two questions out of the 5 
<img width="704" alt="Pasted Graphic" src="https://user-images.githubusercontent.com/60487925/234729955-2051b363-c86a-440f-a8ca-318364158398.png">

2. Ask user to input their birthday. 
   - group based on zodiac signs 
3. User gets to ask question which we generate an answer using emotion & birthday OR give a general fortune / reading based on computed emotion & birthday. 

- Case Study Idea: can ask Haven's roommate to test the accuracy of the fortune teller, in terms of astrology, since she is a witch 
- Cool Features: 
- → can show friends current mood / aura 
- → can show major events in their fortune 

## Scheduling
 - next meeting @2-4pm Saturday (scheduled meeting time) 
