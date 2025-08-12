# Formula 1 Sponsorship Relevance Ranking Tool

This project was completed as a Case Study for DS3010.

# Business Problem
The F1 has 10 different teams with different drivers each season. How should companies decide who is the most ideal to sponsor?

# Our Solution
We take in a sponsor's interests and match them with the perfect ambassador. Our tool:
- Utilize Twitter data and external datasets
- Takes in interests and what type of company/sponsor they are
- Scores drivers based on various factors (popularity, relevance, nationality, etc.)
- Provides a final ranking and composite score

# Sample Example: British Golf Company
*This demo/example reflects the 2022 season*

## Company Interests:
- popular driver
- engaged with golf
- British driver

## Part 1: Popularity

Taken from an external dataset of the most popular driver this season, the most popular drivers in the 2022 season were Lewis Hamilton, Max Verstappen, and Lando Norris.

<img width="664" height="126" alt="image" src="https://github.com/user-attachments/assets/dd24a5e8-5f3f-4e9b-991d-c8def309b4f5" />

## Part 2: Golf engagement

Using the keyword "golf" on Twitter, the most relevant drivers are Carlos Sainz (0.644), Nicholas Latifi (0.561), and Lando Norris (0.329)

<img width="652" height="73" alt="image" src="https://github.com/user-attachments/assets/5128708e-5fa4-48e8-9a4e-7b0832a49b2c" />

## Part 3: Nationality

Drivers who are British are George Russell, Lando Norris, and Lewis Hamilton.

<img width="462" height="140" alt="image" src="https://github.com/user-attachments/assets/02df2cb6-d3ca-49bc-b194-9fbe682bda02" />

## Result
We had to normalize the scores before creating composite scores as Tweet density is much smaller than numbers like popularity or nationality alignment.

final_score = normal_golf + normal_popularity + normal_nationality

<img width="467" height="228" alt="image" src="https://github.com/user-attachments/assets/cd83b4ab-0b36-488e-8ff5-4990760eedc7" />

## Top 3 (Score):
1. Lando Norris (1.39)
2. Lewis Hamilton (1.23)
3. George Russell (0.91)


