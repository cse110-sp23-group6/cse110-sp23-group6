# ADRs (Any decision records)


## Decision Record: Not Using Chat GPT API

### Context and Problem Statement

We needed to decide whether to use the Chat GPT API for our AI chatbot app.

### Considered Options

- Chat GPT API
- Building our own set of responses

### Decision Outcome

We decided not to use the Chat GPT API due to concerns about redundancy and costs:
- Users could just use Chat GPT directly, and using the API would require us to pay for a subscription. 
- Instead, we will store our own responses based on specifc input from the user and mood that we detect from the set of questions asked.