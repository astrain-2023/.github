# Overview

## Inspiration

we are mostly located in CH, some born here
we all drive
we want to make driving a better experience
we want to reduce emissions

## What it does

app that helps the user to make the right decission when driving to avoid congestion
uses incentives to get the user to good behaviour

## How we built it

like pros
long thought process, some figma planning map whatever stuff
look at data, how we can combine etc

![Architecture Chart](../assets/architecture.png)

High level:
- Edge devices providing sensor data (existing, provided by ASTRA)
- App on user devices
- Vercel for edge deployments of the app
- Confluent Cloud for real-time data streaming and processing
- GCP for services and Confluent Cloud deployment (interchangeble with Azure or AWS at this point)


## Challenges we ran into

building a good prediciton model would need more inputs
real-time data would still be needed to get the best results
many discussions, evaluation etc

## Accomplishments that we're proud of

good decision
real-time data streaming
app that shows the gist 


## What we learned

Our use cases mostly build on real-time data streaming, reacting to events that happen on the street, rather than using a prediction model. As part of our use case dicussion we have worked out cases that would build on prediction in combination with real-time data, but have rated those as less useful. To better understand our decision process have a look at our [inception](inception.md) docs.

## What's next for AstAIn
To the moon

## Built With

LOVE, ...

