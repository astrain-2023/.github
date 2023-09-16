# Overview

## Inspiration

Time is our most valuable asset and spending time in traffic jams is not just bad for you, but also bad for the environment. As users of the Swiss road system and as admirers of the beautiful environment of Switzerland, we have a deep desire to make an impact to improve the current situation.

## What it does

Drivers on Swiss roads spend endless hours in traffic jams. Existing Map apps from Google or Apple lack the data and featuers do properly fight congestions in areas with high traffic peaks and limited options for alternative routes. Often, rerouting traffic even creates additional traffic jams in areas that were not built for high throghput.

Our app uses sensor data from inductive loop detectors and road cameras to get a more comprehensive view of the road state and combine it with GPS data of individual drivers in real-time. With gamification and our own reward system we incentivise the drivers to follow our recommended action and therefore help to avoid congestion all-together.

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

