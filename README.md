# Kasagi Labo Coding Challenges
![Cover Image](https://storage.googleapis.com/anime-images-001/cat_coding.png)

Welcome to the [Kasagi Labo](https://www.kasagilabo.com/) coding challenges! These challenges cover a wide range of topics and will test your programming skills.These programming challenges cover for Web, Mobile and/or Backend development. These challenges are designed to test your problem-solving skills, coding proficiency, and architectural acumen. We aim to provide a comprehensive set of challenges that cover various aspects of software engineering, from basic coding tasks to more advanced topics.  These challenges are designed to test architectural thinking, scalability, performance optimization, and the ability to design robust and maintainable systems.

## 🚀 Backend Challenges 

These challenges focus on server-side logic, data management, and real-time communication, which are often crucial for game backends or complex application infrastructures. Prefer programing languages like Node.js, Python, Java, C#, or Go.


### Objective 
**Challenge: Scalable Real-time State Synchronization Service**

Design and partially implement a backend service responsible for synchronizing complex game state or application data in real-time across numerous connected clients (players or users).

Imagine a hypothetical game engine called KasagiEngine is used for multiplayer games or collaborative applications. This service would be the backbone for ensuring all participants have a consistent view of the shared world or document.

### Requirements

1. Architecture
    * Design a system that can handle a high volume of concurrent connections and frequent state updates. 
    * Consider different architectural patterns (e.g., actor model, distributed systems, microservices).

2. Networking
    * Choose and justify appropriate real-time communication protocols (WebSockets, WebRTC data channels, etc.).

3. Performance 
    * Implement efficient data serialization/deserialization. 
    * Design strategies for delta compression or partial state updates to minimize bandwidth.

4. Scalability 
    * Outline how the service would scale horizontally. 
    * Discuss potential bottlenecks and how to address them (e.g., load balancing, sharding of game sessions/data).

5. Resilience & Fault Tolerance
    * How would the system handle disconnections, server failures, and data consistency issues?

6. Internals 
    * Demonstrate understanding of event loop, concurrency model, and how to avoid blocking operations.

### Deliverables
   * A high-level architectural diagram and design document.
   * A core prototype that demonstrating the chosen communication protocol and basic state synchronization for a simplified data model.
   * A discussion of trade-offs made in the design.
   * A plan for testing the scalability and reliability of the service.



## 🌐 Frontend Development Challenge 
This can be done in either web, app, or hybrid.

### Objective

Build a simplified “Anime Explorer” app that lists anime, lets users view details, mark favorites, and filter by genre. This will evaluate your skills in:

* Frontend architecture
* Navigation
* API consumption
* State management
* Component design
* Basic animations or interactions

### Requirements

1. Anime List Screen

    * Fetch data from the [Jikan API](https://docs.api.jikan.moe/#tag/anime) (e.g., https://api.jikan.moe/v4/anime).
    * Show a list of anime with image, title, and score.
    * Implement pagination (infinite scroll or “Load More”).

2. Anime Detail Screen

    * When a user taps an anime, navigate to a detail screen.
    * Show synopsis, genres, score, and other relevant info.

3. Favorites Feature

    * Allow users to “favorite” an anime.
    * Store favorites locally (using AsyncStorage or MMKV).
    * Favorites persist on app reload.
    * Optional: Provide a Favorites tab to view saved items.

4. Filter by Genre

    * Add a dropdown/filter component to filter anime by genre.
    * Use the Jikan API genre filtering if possible, or do client-side filtering.

5. Basic Styling and UX

    * Responsive design for different screen sizes.
    * Use placeholder/loading UI states.
    * Handle API errors gracefully.

### Bonus Points (Optional)
* Use TypeScript / React Native / React JS.
* Add animations (e.g., favoriting with a heart animation).
* Use a state manager (Zustand, Redux Toolkit, or React Context).
* Write basic unit tests (Jest) or integration tests (React Native Testing Library).
* Implement deep linking or share functionality.
* Code-splitting and performance optimization.

### Tools You Can Use
* React Navigation
* Axios or Fetch
* React Native Reanimated or LayoutAnimation (for animations)
* Any component library or styling approach (Tailwind, Styled Components, etc.)

## 🗄️⚙️ Data Engineer

### Objective
This assessment evaluates your logical reasoning and ability to handle unstructured problems by completing three data engineering challenges, with an optional bonus.

### Challenge 1: Data Generation
Build a program that creates a 10MB text file. This file must contain a continuous stream of random objects, with each object separated by a comma. The stream should be a random mix of four data types:
- Alphabetical strings: Containing only letters.
- Integers: Whole numbers.
- Real numbers: Numbers with a decimal point.
- Alphanumeric strings: A combination of letters and numbers. These must also have a random number of leading and trailing spaces, totaling no more than 10 spaces.
The final output should be a single, comma-separated file.

### Challenge 2: Data Processing
Develop a program that ingests the file created in Challenge 1. The program should then parse each individual object, identify its data type, and print the object along with its type to the console. For the alphanumeric strings, you must first remove any leading or trailing spaces.

### Challenge 3: Anime Data Pipeline
Construct a program that executes a full data pipeline from extraction to loading:
- Extract: Scrape data from an anime-focused wiki or similar site. The program should be able to collect at least three key data points for a list of anime titles, such as the release date, number of episodes, and main studio.
- Transform: Clean and refine the scraped data. This involves handling missing values, standardizing studio names, and creating a new calculated column—like years since release—based on the scraped date.
- Load: Store the cleaned and transformed data into a structured format of your choice, such as a CSV file or a SQLite database.

### Bonus Challenge
You can optionally demonstrate your architectural skills by designing a reusable code base from Challenge 1 and 2 that can also be applied to solve aspects of Challenge 3.

## Submission Guidelines
* Upload your code to GitHub/GitLab.
* Include a README.md with:
* Instructions to run the app
* Any known limitations or trade-offs
* Your thought process and architecture decisions

## Time Estimate

4–6 hours. You don’t have to complete every feature. Focus on **quality over quantity**.
