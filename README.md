# Kasagi Labo Programming Challenges

Below is list for software engineer programming challenges for Web, Mobile and Backend development. These challenges are designed to test your problem-solving skills, coding proficiency, and architectural acumen. We aim to provide a comprehensive set of challenges that cover various aspects of software engineering, from basic coding tasks to more advanced topics.  These challenges are designed to test architectural thinking, scalability, performance optimization, and the ability to design robust and maintainable systems.

## Backend Challenges 🚀

These challenges focus on server-side logic, data management, and real-time communication, which are often crucial for game backends or complex application infrastructures. Prefer programing languages like Node.js, Python, Java, C#, or Go.

### Challenge: Scalable Real-time State Synchronization Service

* **Objective:** Design and partially implement a backend service responsible for synchronizing complex game state or application data in real-time across numerous connected clients (players or users).
* **Context (Hypothetical KasagiEngine):** Imagine KasagiEngine is used for multiplayer games or collaborative applications. This service would be the backbone for ensuring all participants have a consistent view of the shared world or document.
* **Key Skills to Test:**
    * **Architecture:** Design a system that can handle a high volume of concurrent connections and frequent state updates. Consider different architectural patterns (e.g., actor model, distributed systems, microservices).
    * **Networking:** Choose and justify appropriate real-time communication protocols (WebSockets, WebRTC data channels, etc.).
    * **Performance:** Implement efficient data serialization/deserialization. Design strategies for delta compression or partial state updates to minimize bandwidth.
    * **Scalability:** Outline how the service would scale horizontally. Discuss potential bottlenecks and how to address them (e.g., load balancing, sharding of game sessions/data).
    * **Resilience & Fault Tolerance:** How would the system handle disconnections, server failures, and data consistency issues?
    * **Internals:** Demonstrate understanding of event loop, concurrency model, and how to avoid blocking operations.
* **Deliverables:**
    * A high-level architectural diagram and design document.
    * A core prototype that demonstrating the chosen communication protocol and basic state synchronization for a simplified data model.
    * A discussion of trade-offs made in the design.
    * A plan for testing the scalability and reliability of the service.

---

## Frontend Development Challenge

This can be done in either web, app, or hybrid.

### Goal

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

### Submission Guidelines

    * Upload your code to GitHub/GitLab.
    * Include a README.md with:
    * Instructions to run the app
    * Any known limitations or trade-offs
    * Your thought process and architecture decisions

### Time Estimate

4–6 hours. You don’t have to complete every feature. Focus on **quality over quantity**.
