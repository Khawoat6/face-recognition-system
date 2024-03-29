# Face Recognition System Using in School Entrance and Notification to Line application

Meta-repo for Face Recognition project 

<img width="1251" alt="Screenshot 2019-10-29 04 50 47" src="https://user-images.githubusercontent.com/31565676/67720918-dd897900-fa07-11e9-9069-a6e5f8ed3f7a.png">


This is senior project under Computer Engineering department, Kasetsart University Sriracha Campus

**Team Members:**
- Chalinee Traiyapanjawit 5930300216
- Phattaraphon Chomchaiyaphum 

**Advisor**:  Dr. Natthapon Pannurat

**Co-advisor**:  Dr.-Ing.Priyakorn Pusawiro 

*Full final project report can be found on Google Doc [here](https://docs.google.com/document/d/1gWH9sYNLsZDmwzqlUDPdA8zF_A7fs7ESvtMaZ215cVQ/edit?usp=sharing)*

*Final presentation slide can be found on Google Doc [here](https://drive.google.com/file/d/1IcE0Jiu9RihASdZLOm9YXGftqSogpq6P/view?usp=sharing)*

## What is Face Recognition?

We want to using interactive technology to express difficult quantum computing concept in a easy way.
We focus on youth, but aim to use universal design for everyone

## Objectives

1. Attendees **experience** quantum computing concept in a tangible way.
2. Attendees **enjoy** it as a piece of art.
3. Attendees **realise** the potential that quantum computing could bring in the near future.

## Story

These are basic concept of quantum computing that we covered:

![Story](https://i.imgur.com/jHxRYOb.jpg)

1. Intro: Quantum computing was invented because of classical computer limitation
2. The qubit: Qubit have more dimension when compared to classical bit and it can be represented as a sphere.
3. Quantum gates: Quantum gates are used to change the qubit state and it can be visualized as a rotation on sphere.
4. Measurement: Measurement is a indeterministic operation that needed to read qubit value. Pre-measure state effect the probability of getting 0 and 1.
5. Getting further: These knowledges can be used to create quantum algorithms to solve some difficult problems that are more efficient when compare to classical computer.

## Use cases

<img width="1249" alt="Screenshot 2019-10-29 04 55 05" src="https://user-images.githubusercontent.com/31565676/67721100-5092ef80-fa08-11e9-8258-bfd7a276b75a.png">


Quantarium user attendees can interact with quantarium one person at the time in general case. Use case can be splitted into 2 part:
1. Storyteller - We want to explain quantum computing story it in the interesting and friendly way especially for novice user.
2. Qubit composer - We want attendees to experience important mechanics involved with qubit with interactive qubit simulator. They can try adding operation with the qubit and see the consequence simultaneously on the bloch sphere.


## Architecture

<img width="1249" alt="Screenshot 2019-10-29 04 53 16" src="https://user-images.githubusercontent.com/31565676/67721008-0f9adb00-fa08-11e9-9144-1fae365a00ac.png">


Our project consist of 3 main parts:
1. Frontend web appllication on tablet providing user interface for user to follow the storytelling tutorial or controling qubit simulation.
2. Backend server doing qubit simulation according to user actions before respoding back to the tablet and generating graphic for the bloach sphere.
3. Bloach sphere representing the qubit using plastic sphere, fisheye lens, and projector with projection mapping technique.

![Client-Server](https://i.imgur.com/YNHAJ9X.png)
Client-server architecture

![Projection mapping](https://i.imgur.com/39o0Fbd.png)
Projection mapping technique on the bloch sphere

## Example demo



Preview quantum gate effect on qubit



Add gate to the qubit and see the state change


Measure the qubit and see the result
## Using this repo

This is [meta-repo](https://github.com/mateodelnorte/meta) containing following sub-projects:
1. [Quantarium UI](https://github.com/Th1nkK1D/quantarium-ui) - VueJS frontend web application
2. [Quantarium API](https://github.com/Th1nkK1D/quantarium-api) - Koa backend API server
3. [Quantarium QSIM](https://github.com/Th1nkK1D/quantarium-qsim) - Javascript qubit simulation library
4. [2D Bloch Sphere](https://github.com/ifindzandba/2dblochsphere) - Bloch sphere graphic generator with Socket IO and Paper JS

### Set up

1. Clone or download this repo
2. Install required packages (recommended using yarn for cross platform script)
   ```bash
   yarn
   ```
3. **Initialize** all projects
   ```bash
   yarn run init
   ```

### Update, build and run
1. **Update** all projects if there is an update (not needed after init) 
   ```bash
   yarn run update
   ```
2. **Build** projects
   ```bash
   yarn run build
   ```
3. **Start** all services (production)
   ```bash
   yarn run start
   ```
4. **Start** in dev mode
   ```bash
   yarn run dev
   ```
