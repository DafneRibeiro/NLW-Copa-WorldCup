# Copa/WorldCup

NLW World cup a challenge by RocketSeat

## Goals of the project

   * Practice ReactJS
   * Learn more about TypeScrypt
   * Learn Tailwind
   * Create a frontend that works and is responsive
   * Have my first contact with ReactNative
   * To learn and develop my backend skills and my web design skills

This project is a Lab project developed by RocketSeat with the purpose of studying and practicing your skills with the tutors.

## To run it

  * cd on web folder
  * open a terminal and use npm run dev
  * run this command on server folder too.
  * run npm i to install all dependencies

## To run the mobile app:

  * cd on mobile folder
  * Run the command expo start
  * run npm i to install all dependencies
  * I recommend using the app Expo Go, its easy to set up as you only need to scan the QR code to run the application on your mobile.

## To run prisma studio and check the ads created for each game:

  * open a terminal on server folder
  * run npx prisma studio
  * select Ad and check the ads created when you submit a form in the modal

## Tech Stack

  * TypeScrypt
  * Tailwind
  * NodeJs
  * Fastify
  * ReactNative
  * Prisma for queries in DB
  * Figma for the design guidances
  * SQlite

## User Stories

  * Be able to create a pool for specific match during the World Cup 2022
  * Be able to share a code with friends inviting them for the pool created
  * Be able to do authentication with google to login
  * Be able to search and find a pool using the pool code.
  * Be able to visualize the pool the person is currently participating
  * Be able to visualize the match with a date, time and who is playing in the card. 
  * Be able to enter my guess for the result of the match and confirm it placing a bet.
  * Be able to see a Rank for the pools.
  * Be able to see all my bets



## Domain Modelling 

  id        String   @id   @default(cuid()) 
  title     String
  code      String   @unique
  createdAt DateTime @default(now())

### Diagram ERD