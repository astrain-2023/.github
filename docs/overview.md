# Overview

## Inspiration

As a multi-national team, some born and some living in Switzerland

TBD

## What it does
TBD

## How we built it
TBD

## Challenges we ran into
TBD

## Accomplishments that we're proud of
yeah

## What we learned
a lot

## What's next for AstAIn
To the moon

## Built With

LOVE

## Challenge

## Architecture

![Architecture Chart](../assets/architecture.png)

High level:
- Edge devices providing sensor data (existing, provided by ASTRA)
- App on user devices
- Vercel for edge deployments of the app
- Confluent Cloud for real-time data streaming and processing
- GCP for services and Confluent Cloud deployment (interchangeble with Azure or AWS at this point)



## Further considerations

Our use cases mostly build on real-time data streaming, reacting to events that happen on the street, rather than using a prediction model. As part of our use case dicussion we have worked out cases that would build on prediction in combination with real-time data, but have rated those as less useful. To better understand our decision process have a look at our [inception](inception.md) docs.