# Brainstorming Meeting 1: Notes

[linktodoc](https://docs.google.com/document/d/1klrnNY1uZ5jQyEJwxwEzivSLW8Xp1ZItC2MGmhDGODU/edit?usp=sharing)
## General ideas
- Spotify API
- Looks at facial expression and playlist of 10 songs
- Songs that you add could form a sentence
- Ask a question and give a song that is the fortune
- Spotify Wrapped aura
- Colors can give different things

## MVP Ideas
- Aura & emotions OR birthday-based astrology
- Would we have problems with facial recognition? (big reach, ask TA)
- Palmistry using image recognition?
- Hand shape, finger analysis
- Major and minor lines
  - Give colors & pictures to determine aura
  - Branch off
  - Can ask Chat GPT
  - Emotions: joy, sad, anger, fear, disgust
  - 5 different questions, user only gets 2
- Input birthday
  - Split based on zodiac signs
- Ask a question & tells you what to do OR can get a general reading
  - Case study: test app on Haven’s roommate witch

## Features
- See friends' fortunes
- See friends' aura as well
- Astrology
  - Analyze upcoming planetary influences
  - Provide daily predictions for each zodiac sign based on current astrological influences
- Personalized report based on relationship, career, etc.
- Social media platform sharing
- User profile that stores previous results

## Next meeting
- Saturday at 2
- Think about more ideas
- Mock draft for Saturday

## Meeting 2: Process
- Ask the user what kind of question they want to ask and have the user pick a category (relationship, food, career, etc.)
- Make the user pick from 5 pictures (or quotes or whatever) → use the chart from above
- Ask the user for birthday/occupation: student or working (cater responses according to their occupation?)
- Give a general reading for the month
- Can include what emotions they are based on answers to picture questions
- Reading based on category & current emotion (ex: do we give more positive reading if the person is sad?)
- User can ask a question (only with Chat GPT)
- Give answer
- Prompt Chat GPT (important)
- Bunch of generic ones (200-300)
- Repeat steps 4 and 5

## Concerns
- Need a storage system: local storage to keep track of previous historical fortunes (like Chat GPT having sidebars with all the previous chats)

## Other features
- Create user profile
- Share with friends

## Functionality
- Keyword → generative context
- Different people can use the app and why would they use it? (restaurant? big life decision?)

## Meeting with TA
- Leave the APIs (too ambitious, also why not just use Chat GPT instead of our app if just plugging in values)
- Need full CRUD functionality

## Meeting 3: CRUD functionality
- **Create fortune**
-**Read past fortune**
- **Update profile (mood, name, relationship status, etc.)**
- **Delete past fortune**

## Extra features
- Regenerate fortune – choose a new one
- New profile accessible from the main homepage or when a new fortune is generated
- Focus on general reading instead of user asking questions

## Possible General Reading Images (depending on the emotion chart on the first page)
- Some inspiration from Spotify
- Created example: Ecstasy (joy & joy)
- Moving text → which animation gives more the sense of ‘thinking’
- Which one looks best lol & any feedback?

## Extra features
- **Create profile**
- **Share with friend**
- Multiple tabs open?
- **Storing answers**
- Spotify playlist
