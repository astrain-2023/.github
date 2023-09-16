# Overview

## Inspiration

Time is our most valuable asset and spending time in traffic jams is not just bad for you, but also bad for the environment. As users of the Swiss road system and as admirers of the beautiful environment of Switzerland, we have a deep desire to make an impact to improve the current situation.

## What it does

Drivers on Swiss roads spend endless hours in traffic jams. Existing Map apps from Google or Apple lack the data and features do properly fight congestions in areas with high traffic peaks and limited options for alternative routes. Often, rerouting traffic even creates additional traffic jams in areas that were not built for high throughput.

Our app uses sensor data from inductive loop detectors and road cameras to get a more comprehensive view of the road state and combine it with GPS data of individual drivers in real-time. With gamification and our own reward system we incentivize the drivers to follow our recommended action and therefore help to avoid congestion all-together.

## How we built it

As a team we spent the first hours brainstorming the problem statement and possible solutions. We clustered our ideas and set the focus, selecting the most impactful use cases. Using a lean gamification canvas we identified how to incentivize drivers to adopt better behaviors.

After creating a joint plan for success, we have split the work into UI, backend and platform development, while continuing to research possible optimization in traffic management.

Our presentation layer is a progressive web app running on the users phone, serving the end user and feeding back GPS data. It is built with Next.js and deployed to the Vercel edge.

Our data platform uses Apache Kafka in combination with stream processing. It is based on Confluent Cloud which enables us to run at massive scale and achieve the throughput and latency we would need to make recommendation that are actually based on real-time data. 

![Architecture Chart](../assets/architecture.png)
(JamHero target architecture)

## What we learned
Real-time data streaming is at the heart our our application. Prediction is useful to get an approximation of a future state but any system that is based on patterns of the past is fragile to the unpredictability of the future.

As part of our use case discussion we have worked out cases that build on top of prediction models, but have rated them as less impactful compared to any real-time decision making. Eventually, the goal is to combine the best of both worlds.

## What's next for AstrAIn
Building a solution that scales to hundreds of devices and manages to make meaningful recommendations that can potentially eliminate human-induced traffic jams is a truly exciting endeavor.

We think there is a lot of potential in using sensor data in real-time. We also think there are problems to solve that go beyond data and AI that require more research.

Nevertheless, we would love to see the next generation of traffic management on our phones soon.

> Written by a real human.

## Built With
coffee, confluent, golang, java, kafka, love, nextjs, typescript

